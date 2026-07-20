---
{"dg-publish":true,"permalink":"/universidad/3er-semestre/matematicas-discretas/unidad-4-recurrencia-y-algoritmos/04-analisis-de-algoritmos-fundamentos-y-funciones-matematicas/","dg-note-properties":{}}
---

# 📈 Análisis de Algoritmos I — Fundamentos y Funciones Matemáticas

## 🎯 Introducción

> [!info] 💡 ¿Por qué medir la eficiencia de un algoritmo?
> 
> El **análisis de algoritmos** estudia cuántos recursos (principalmente tiempo) consume un algoritmo a medida que crece el tamaño de la entrada $n$. En lugar de medir tiempo real (que depende de la máquina), se usa **notación asintótica** para describir el crecimiento de forma independiente del hardware.
> 
> - Las **cotas asintóticas** ($\mathcal{O}$, $\Omega$, $\Theta$) describen el comportamiento de un algoritmo cuando $n$ es grande.
> - Esta nota es la **primera de dos partes**: aquí se cubren las definiciones formales y cómo obtener $\mathcal{O}$, $\Omega$ y $\Theta$ a partir de una **función matemática** ya dada (ejercicios de "estudiar $f(n)$"). La segunda parte, [[Universidad/3er Semestre/Matemáticas Discretas/Unidad 4 - Recurrencia y Algoritmos/05 - Análisis de Algoritmos - Pseudocódigo y Tiempo Real\|05 - Análisis de Algoritmos - Pseudocódigo y Tiempo Real]], cubre cómo obtenerlas **contando operaciones en pseudocódigo**, y la sección de tiempo real, errores comunes, ejercicios de repaso y metas de aprendizaje.
> - Se conecta con [[Universidad/3er Semestre/Matemáticas Discretas/Unidad 4 - Recurrencia y Algoritmos/03 - Pseudocódigo y Algoritmos\|03 - Pseudocódigo y Algoritmos]] y con [[Universidad/3er Semestre/Matemáticas Discretas/Unidad 4 - Recurrencia y Algoritmos/01 - Relaciones de Recurrencia\|01 - Relaciones de Recurrencia]] / [[Universidad/3er Semestre/Matemáticas Discretas/Unidad 4 - Recurrencia y Algoritmos/02 - Recurrencia Homogénea\|02 - Recurrencia Homogénea]] para el análisis de algoritmos recursivos, que se retoma en la segunda parte.
> 
> **Contexto histórico:**
> 
> La notación $\mathcal{O}$ no nació en ciencias de la computación: la introdujo el matemático **Paul Bachmann** en 1894 para teoría de números, y la popularizó **Edmund Landau** poco después — por eso también se le llama _notación de Landau_. Fue **Donald Knuth**, en _The Art of Computer Programming_ (1968), quien la adaptó al análisis formal de algoritmos, estableciendo el estándar que se usa hoy. Antes de esto, comparar algoritmos dependía de cronometrar ejecuciones en una máquina específica — poco confiable, porque el mismo algoritmo corre distinto según el hardware. La notación asintótica resolvió esto al abstraerse por completo de la máquina.
> 
> **Analogía del mundo real:**
> 
> Comparar dos algoritmos por su notación asintótica es como comparar dos corredores no por la distancia que recorrieron en una carrera específica, sino por qué tan rápido crece su tiempo de llegada a medida que la carrera se hace más y más larga.
> 
> ```mermaid
> graph TD
>     A[Análisis de<br/>Algoritmos] --> B[Cotas Asintóticas<br/>O, Ω, Θ]
>     B --> P1[Esta nota<br/>Funciones Matemáticas]
>     B --> P2[Nota II<br/>Pseudocódigo y Tiempo Real]
>     P1 --> P1a[Regla del grado<br/>polinomios y racionales]
>     P1 --> P1b[Demostración con<br/>c₁, c₂, n₀]
>     P1 --> P1c[Acotación por<br/>desigualdades]
> 
>     style B fill:#e1f5ff
>     style P1 fill:#e1ffe1
>     style P2 fill:#fff4e1
> ```
> 
> |Tema|Idea central|
> |---|---|
> |**$\mathcal{O}$**|Cota superior: "no crece más rápido que"|
> |**$\Omega$**|Cota inferior: "no crece más lento que"|
> |**$\Theta$**|Cota estrecha: $\mathcal{O}$ y $\Omega$ a la vez|
> |**Esta nota**|Obtener las cotas a partir de una fórmula $f(n)$ ya dada|
> |**Nota II**|Obtener las cotas contando operaciones en pseudocódigo|

## 🔵 Cotas Asintóticas Fundamentales

> [!note] 🔵 Definiciones formales (como las plantea la clase)
> 
> Sea $f(n)$ el número de operaciones de un algoritmo. La definición exacta que usa el profesor Pineda usa **valor absoluto** y la frase "excepto una cantidad finita de valores de $n$" (equivalente a "$\forall n \geq n_0$", pero así aparece en la diapositiva — por eso la reproducimos igual):
> 
> - **Cota superior $\mathcal{O}$:** $f(n) = \mathcal{O}(g(n))$ si existe una constante $C_1>0$ tal que $|f(n)| \leq C_1|g(n)|$, para todo $n \in \mathbb{N}$, excepto una cantidad finita de valores de $n$.
>     
> - **Cota inferior $\Omega$:** $f(n) = \Omega(g(n))$ si existe una constante $C_2>0$ tal que $|f(n)| \geq C_2|g(n)|$, para todo $n \in \mathbb{N}$, excepto una cantidad finita de valores de $n$.
>     
> - **Cota estrecha $\Theta$:** $f(n) = \Theta(g(n))$ si $f(n) = \mathcal{O}(g(n))$ **y** $f(n) = \Omega(g(n))$.
>     
> 
> > [!tip] 📌 Intuición rápida
> > 
> > - $\mathcal{O}$ → cota máxima ("a lo sumo crece así")
> > - $\Omega$ → cota mínima ("al menos crece así")
> > - $\Theta$ → crecimiento exacto ("crece exactamente así")
> 
> Estas tres definiciones son las mismas sin importar si $f(n)$ viene de una fórmula matemática o de contar líneas de pseudocódigo — lo único que cambia es **cómo consigues $f(n)$** en primer lugar. Eso es justo lo que separan las dos partes siguientes.

> [!example]- 🟢 Ejemplo canónico de la clase — $f(n) = 60n^2+5n+1$
> 
> **Cota superior:** para $n\geq1$, $5n \leq 5n^2$ y $1 \leq n^2$, entonces
> 
> $$60n^2+5n+1 \leq 60n^2+5n^2+n^2 = 66n^2, \quad \forall n \in \mathbb{N}$$
> 
> Tomando $g(n)=n^2$ y $C_1=66$: $f(n) = \mathcal{O}(n^2)$.
> 
> **Cota inferior:** de forma trivial (quitando los términos positivos $5n+1$),
> 
> $$60n^2+5n+1 \geq 60n^2, \quad \forall n \in \mathbb{N}$$
> 
> Tomando $g(n)=n^2$ y $C_2=60$: $f(n) = \Omega(n^2)$.
> 
> **Conclusión:** como $f(n)=\mathcal{O}(n^2)$ y $f(n)=\Omega(n^2)$ simultáneamente, $f(n) = \Theta(n^2)$.
> 
> Este mismo resultado se reutiliza más adelante: si un algoritmo toma $60n^2+5n+1$ unidades de tiempo en el peor caso, ese peor caso es directamente $\Theta(n^2)$.

---

## 📊 Órdenes de Crecimiento Comunes

> [!note] 📋 Tabla comparativa — de menor a mayor crecimiento
> 
> |Notación|Nombre|Ejemplo típico|¿Cómo se ve en código?|
> |---|---|---|---|
> |$\mathcal{O}(1)$|Constante|Acceder a `lista[i]`|Sin ciclos dependientes de $n$|
> |$\mathcal{O}(\log n)$|Logarítmica|Búsqueda binaria|Se descarta la mitad del problema en cada paso|
> |$\mathcal{O}(n)$|Lineal|Recorrer una lista una vez|Un `for` simple de tamaño $n$|
> |$\mathcal{O}(n \log n)$|Linearítmica|Mergesort, Quicksort (caso promedio)|Dividir y combinar|
> |$\mathcal{O}(n^2)$|Cuadrática|Bubble sort, dos `for` anidados|Ciclo dentro de otro ciclo, ambos de tamaño $n$|
> |$\mathcal{O}(n^3)$|Cúbica|Multiplicación de matrices (algoritmo ingenuo)|Tres `for` anidados|
> |$\mathcal{O}(2^n)$|Exponencial|Fuerza bruta sobre subconjuntos|Recursión que se ramifica en 2 por cada elemento|
> |$\mathcal{O}(n!)$|Factorial|Fuerza bruta sobre permutaciones (viajante)|Probar todas las ordenaciones posibles|
> 
> > [!warning]- ⚠️ Error común: "más rápido en la práctica" no es lo mismo que "mejor orden de crecimiento"
> > 
> > Un algoritmo $\mathcal{O}(n^2)$ puede ser **más rápido en la práctica** que uno $\mathcal{O}(n \log n)$ si $n$ es pequeño y las constantes ocultas del segundo son grandes. La notación asintótica solo garantiza superioridad cuando $n$ crece **lo suficiente** — no dice nada sobre valores pequeños de $n$.

---

## 🧮 Cómo Obtener las Cotas en Funciones Matemáticas

> [!info] 📐 ¿Qué distingue a esta parte?
> 
> Aquí el punto de partida es una **fórmula $f(n)$ ya dada explícitamente** (como $f(n) = 2n^2-5n+3$) y el trabajo es puramente algebraico: identificar el término dominante, y si se pide demostrar, exhibir $c$ y $n_0$. No hay pseudocódigo ni que contar líneas — es análisis de funciones, igual que en cálculo.

### 🟢 Análisis Asintótico de Funciones Comunes

> [!tip] 🟢 Casos frecuentes
> 
> |Función|Comportamiento asintótico|
> |---|---|
> |Polinomio de grado $k$: $p(n)$|$p(n) = \Theta(n^k)$|
> |Suma aritmética: $\sum_{i=1}^{n} i$|$\dfrac{n(n+1)}{2} = \Theta(n^2)$|
> |Factorial logarítmico: $\log n!$|$\Theta(n\log n)$|
> 
> > [!example]- ¿Por qué $\log n! = \Theta(n\log n)$?
> > 
> > La demostración completa y rigurosa está en la subsección "🎓 Cotas Asintóticas de Logaritmos" más abajo. Intuición rápida: por Stirling, $n! \approx \sqrt{2\pi n}\left(\frac{n}{e}\right)^n$, y al aplicar logaritmo, $\log n! \approx n\log n - n$, cuyo término dominante es $n\log n$.

### 🎓 Técnica: Demostrar $\mathcal{O}$, $\Omega$ y $\Theta$ para Polinomios y Funciones Racionales

> [!note] 📋 Regla rápida (atajo)
> 
> Si $p(n) = a_k n^k + a_{k-1}n^{k-1} + \cdots + a_0$ con $a_k > 0$, entonces $p(n) = \Theta(n^k)$: el grado del polinomio determina directamente la cota estrecha. Para una **función racional** $\dfrac{p(n)}{q(n)}$, se comparan los grados de numerador y denominador: $\Theta!\left(n^{\deg p - \deg q}\right)$.
> 
> Este atajo es válido y rápido para responder, pero cuando el ejercicio pide **"estudiar" o "demostrar"** la función (no solo dar la respuesta), hay que exhibir $c_1$, $c_2$ y $n_0$ explícitos — igual que exige el principio de verificación formal visto más abajo.

> [!example]- 🟢 Ejemplo completo — Estudiar $f(n) = 2n^2 - 5n + 3,\ \forall n \in \mathbb{N}$
> 
> **Objetivo:** demostrar que $f(n) = \Theta(n^2)$, exhibiendo $c_1$, $c_2$ y $n_0$.
> 
> **Paso 1 — Cota superior ($\mathcal{O}$):**
> 
> Para $n \geq 1$, se cumple $3 \leq 3n^2$, entonces:
> 
> $$f(n) = 2n^2 - 5n + 3 \leq 2n^2 + 3 \leq 2n^2 + 3n^2 = 5n^2$$
> 
> Es decir, $f(n) \leq 5n^2$ para todo $n \geq 1$ → $f(n) = \mathcal{O}(n^2)$ con $c_1 = 5$, $n_0 = 1$.
> 
> **Paso 2 — Cota inferior ($\Omega$):**
> 
> Buscamos $c_2$ tal que $f(n) \geq c_2 n^2$. Probamos con $c_2 = 1$:
> 
> $$2n^2 - 5n + 3 \geq n^2 \iff n^2 - 5n + 3 \geq 0$$
> 
> Resolviendo $n^2-5n+3=0$ con la fórmula general, las raíces son $n = \dfrac{5\pm\sqrt{13}}{2} \approx 0{,}70$ y $4{,}30$. La parábola es positiva fuera de ese intervalo, así que para todo entero $n \geq 5$ se cumple $n^2-5n+3\geq 0$.
> 
> Por lo tanto, $f(n) \geq n^2$ para todo $n \geq 5$ → $f(n) = \Omega(n^2)$ con $c_2 = 1$, $n_0 = 5$.
> 
> **Paso 3 — Conclusión:**
> 
> Como ambas cotas valen simultáneamente a partir de $n_0 = 5$:
> 
> $$n^2 \leq f(n) \leq 5n^2 \quad \text{para todo } n \geq 5 \quad\implies\quad f(n) = \Theta(n^2) \quad \blacksquare$$
> 
> > [!tip]- 💡 Truco para elegir $c_1$ rápido
> > 
> > En la cota superior, basta con **sobreestimar** cada término negativo o de menor grado por un múltiplo del término dominante (aquí, acotamos $3 \leq 3n^2$ para $n\geq1$). No hace falta encontrar la constante más ajustada — cualquier $c_1$ que funcione es válida.

> [!success]- ✅ Corrección: los coeficientes líderes negativos NO son un problema
> 
> En una versión anterior de esta nota advertíamos que $\Theta$ "no aplicaría" si el coeficiente líder es negativo (como en $f(n)=-4n^3+n^2-5n$). **Eso estaba mal.** El teorema real, tal como lo enuncia la clase, es:
> 
> > **Teorema.** Cualquier polinomio en $n$ de grado $k$ es $\Theta(n^k)$, **aun cuando algunos de sus coeficientes sean negativos**.
> 
> La razón es que la definición formal usa **valor absoluto**: $|f(n)| \leq C_1|g(n)|$. Aunque $f(n)=-4n^3+n^2-5n$ se vuelve negativa para $n$ grande, $|f(n)|$ se comporta como $4n^3$, así que $f(n)=\Theta(n^3)$ **sin ninguna salvedad**. Los ejercicios 1 y 2 de abajo (con coeficiente líder negativo) son válidos y rigurosos tal cual están, no solo "regla mecánica".

### ✏️ Ejercicios de Clase — Notación Θ de Polinomios

> [!question] 📋 Encuentra la notación Θ para cada función (clase del 16/07, Ebner Pineda)
> 
> **1.** $f(n) = -4n^3 + n^2 - 5n,\ \forall n \in \mathbb{N}$
> 
> **2.** $f(n) = -\dfrac{5}{3}n^2 + 7n + 8,\ \forall n \in \mathbb{N}$
> 
> **3.** $f(n) = \dfrac{3}{4}n^3 - 4n^2 - 7n,\ \forall n \in \mathbb{N}$
> 
> **4.** $f(n) = \dfrac{5n^3 + 3\log n}{2 + 7n}$

> [!success]- ✅ Respuestas (regla rápida)
> 
> **1.** $\Theta(n^3)$ — el término dominante es $-4n^3$; es válido y riguroso pese al signo (ver corrección sobre coeficientes negativos arriba).
> 
> **2.** $\Theta(n^2)$ — el término dominante es $-\frac{5}{3}n^2$.
> 
> **3.** $\Theta(n^3)$ — el término dominante es $\frac{3}{4}n^3$.
> 
> **4.** $\Theta(n^2)$ — en el numerador, $5n^3$ domina a $3\log n$ (todo polinomio crece más rápido que cualquier logaritmo), así que el numerador es $\Theta(n^3)$. En el denominador, $7n$ domina a $2$, así que el denominador es $\Theta(n)$. Dividiendo los grados: $\Theta(n^3)/\Theta(n) = \Theta(n^{3-1}) = \Theta(n^2)$.
> 
> > [!tip]- 🖥️ Demostración rigurosa del ejercicio 3 (con $c_1$, $c_2$ explícitos)
> > 
> > Para $f(n) = \frac{3}{4}n^3 - 4n^2 - 7n$: cota superior con $n\geq1$: $4n^2+7n \leq 11n^2 \leq 11n^3$, entonces $f(n) \leq \frac{3}{4}n^3 + 11n^3 < 12n^3$ → $c_1=12$. Cota inferior: para $n$ suficientemente grande (puedes verificar con $n_0=20$), $\frac{3}{4}n^3 - 4n^2 - 7n \geq \frac{1}{2}n^3$ → $c_2=\frac{1}{2}$. Concluye $f(n)=\Theta(n^3)$.

### 🎓 Técnica Alternativa: Acotación Término a Término (Desigualdades)

> [!note] 📋 La idea
> 
> En vez de despejar $c$ algebraicamente, esta técnica **reemplaza cada término** de $f(n)$ por una expresión más simple que sea mayor o igual (para $\mathcal{O}$) o menor o igual (para $\Omega$), encadenando desigualdades hasta llegar a $c \cdot g(n)$. Es el método que verás más seguido en clase para sumas y funciones racionales.
> 
> **Regla de dirección — la parte que más se presta a confusión:**
> 
> |Quieres...|En el numerador...|En el denominador...|
> |---|---|---|
> |Cota superior ($\mathcal{O}$)|**Agranda** cada término (sobreestima)|**Achica** (usa una cota inferior del denominador)|
> |Cota inferior ($\Omega$)|**Achica** cada término (subestima, sin pasar de 0)|**Agranda** (usa una cota superior del denominador)|
> 
> Achicar el denominador agranda la fracción completa, y viceversa — por eso la dirección se invierte entre numerador y denominador.

> [!tip] 📌 Desigualdad útil: logaritmos
> 
> $$\log x \leq x - 1, \quad \forall x \geq 1$$
> 
> Sustituyendo $x=n$ con $n \in \mathbb{N}$: $\log n \leq n-1$. Esta desigualdad es la herramienta estándar para **acotar por arriba** cualquier término logarítmico y reemplazarlo por algo polinomial, mucho más fácil de manejar en una cadena de desigualdades.

> [!example]- 🟢 Ejemplo 1 — Función racional: $f(n) = \dfrac{5n^3+3\log n}{2+7n}$ (Notación $\Omega$)
> 
> **Objetivo:** encontrar $\Omega$, siguiendo la regla de dirección: para una cota inferior, **achicamos** el denominador (lo agrandamos, ya que queremos $\Omega$... revisa la tabla: para $\Omega$ el denominador se **agranda**).
> 
> **Paso 1 — Acotar el denominador por arriba:** para $n \geq 1$, $2 \leq 2n$, entonces:
> 
> $$2 + 7n \leq 2n + 7n = 9n$$
> 
> Como el denominador real es **menor o igual** que $9n$, dividir entre el denominador real da un resultado **mayor o igual** que dividir entre $9n$:
> 
> $$f(n) = \frac{5n^3+3\log n}{2+7n} \geq \frac{5n^3+3\log n}{9n}$$
> 
> **Paso 2 — Acotar el numerador por abajo:** como $\log n \geq 0$ para $n\geq 1$, quitar ese término solo puede achicar el numerador:
> 
> $$\frac{5n^3+3\log n}{9n} \geq \frac{5n^3}{9n} = \frac{5}{9}n^2$$
> 
> **Conclusión:** $f(n) \geq \frac{5}{9}n^2$ para todo $n\geq 1$ → $f(n) = \Omega(n^2)$ con $c_2 = \frac{5}{9}$, $n_0=1$.
> 
> Como en el Ejercicio 4 ya habíamos obtenido $f(n) = \mathcal{O}(n^2)$ con la regla rápida (numerador $\Theta(n^3)$ entre denominador $\Theta(n)$), y ahora tenemos $\Omega(n^2)$ de forma rigurosa:
> 
> $$f(n) = \mathcal{O}(n^2) \ \text{y} \ f(n) = \Omega(n^2) \quad\implies\quad f(n) = \Theta(n^2) \quad\blacksquare$$
> 
> > [!tip]- 💡 La cota $\mathcal{O}(n^2)$ de forma rigurosa (con la misma técnica)
> > 
> > Para $\mathcal{O}$, ahora el numerador se **agranda** y el denominador se **achica**. Numerador: usando $\log n \leq n-1 \leq n \leq n^3$ (para $n\geq1$), $5n^3+3\log n \leq 5n^3+3n^3 = 8n^3$. Denominador: $2+7n \geq 7n$ (cota inferior trivial, se quita la constante positiva). Entonces $f(n) \leq \dfrac{8n^3}{7n} = \dfrac{8}{7}n^2$ → $f(n)=\mathcal{O}(n^2)$ con $c_1=\frac{8}{7}$, $n_0=1$.

> [!example]- 🟢 Ejemplo 2 — Suma aritmética: $f(n) = 1+2+\cdots+n$
> 
> **Cota superior ($\mathcal{O}$):** cada uno de los $n$ términos de la suma es **como mucho** $n$, así que:
> 
> $$f(n) = 1+2+\cdots+n \leq \underbrace{n+n+\cdots+n}_{n \text{ términos}} = n\cdot n = n^2, \quad \forall n \in \mathbb{N}$$
> 
> Esto es, $f(n) = \mathcal{O}(n^2)$.
> 
> **Cota inferior ($\Omega$):** cada término es **como mínimo** $1$, así que:
> 
> $$f(n) = 1+2+\cdots+n \geq \underbrace{1+1+\cdots+1}_{n \text{ veces}} = n$$
> 
> Por lo que $f(n) = \Omega(n)$.
> 
> > [!warning] ⚠️ Aquí **todavía no** se puede concluir una $\Theta$ para $f$
> > 
> > Tenemos $f(n) = \mathcal{O}(n^2)$ y $f(n) = \Omega(n)$ — pero para concluir $\Theta$, **ambas cotas deben usar la misma función** $g(n)$. Aquí una dice "$n^2$" y la otra dice "$n$": hay una brecha entre ellas, así que estas dos desigualdades **por sí solas** no bastan.
> > 
> > Para cerrar la brecha hace falta una cota más ajustada (o usar la fórmula cerrada $f(n) = \frac{n(n+1)}{2}$, que ya vimos en la tabla de "Análisis Asintótico de Funciones Comunes" y que sí da directamente $\Theta(n^2)$). La lección: **acotar por arriba y por abajo no garantiza $\Theta$ automáticamente** — solo lo garantiza cuando ambas cotas coinciden en el mismo orden de crecimiento.

> [!example]- 🟢 Cerrando la brecha — cota $\Omega(n^2)$ ajustada para $1+2+\cdots+n$
> 
> Retomando el Ejemplo 2: ya sabíamos $f(n)=\mathcal{O}(n^2)$ y $f(n)=\Omega(n)$, con una brecha entre $n$ y $n^2$. Para cerrarla, agrupamos la suma de otra forma: independientemente de si $n$ es par o impar,
> 
> $$1+2+\cdots+n \geq n + (n-1) + \cdots + \left\lceil \frac{n}{2} \right\rceil$$
> 
> (es decir, solo la "mitad superior" de los términos). Como cada uno de esos términos es **al menos** $\left\lceil \frac{n}{2} \right\rceil$:
> 
> $$1+2+\cdots+n \geq \underbrace{\left\lceil \frac{n}{2} \right\rceil + \left\lceil \frac{n}{2} \right\rceil + \cdots + \left\lceil \frac{n}{2} \right\rceil}_{\left\lceil \frac{n+1}{2} \right\rceil \text{ términos}}$$
> 
> Multiplicando el número de términos por el valor de cada uno:
> 
> $$1+2+\cdots+n \geq \left\lceil \frac{n+1}{2} \right\rceil \cdot \left\lceil \frac{n}{2} \right\rceil \geq \frac{n}{2}\cdot\frac{n}{2} = \frac{n^2}{4}, \quad \forall n \in \mathbb{N}$$
> 
> Así, $f(n) = \Omega(n^2)$. Combinando con la cota superior $f(n)=\mathcal{O}(n^2)$ del Ejemplo 2:
> 
> $$f(n) = 1+2+\cdots+n = \Theta(n^2) \quad \blacksquare$$
> 
> Esta es la técnica que hay que usar cuando tu primera cota inferior "obvia" no alcanza: en vez de subestimar **todos** los términos por el más chico (que da una cota demasiado floja), subestimas solo la **mitad superior** de los términos por el más chico de esa mitad — mucho más ajustado.

### 🎓 Cotas Asintóticas de Logaritmos

> [!tip] 📌 Propiedad clave
> 
> $$\log n < n, \quad \forall n \in \mathbb{N}$$
> 
> (aquí $\log n$ denota $\log_2 n$, la convención estándar en análisis de algoritmos). Esta desigualdad es la herramienta base para acotar por arriba cualquier término logarítmico.

> [!example]- 🟢 Ejemplo — $f(n) = 2n + 3\log n$
> 
> **Cota superior:** por $\log n < n$,
> 
> $$2n+3\log n < 2n+3n = 5n, \quad \forall n \in \mathbb{N} \quad\implies\quad f(n) = \mathcal{O}(n)$$
> 
> **Cota inferior:** de forma trivial (quitando el término positivo $3\log n$),
> 
> $$2n+3\log n \geq 2n, \quad \forall n \in \mathbb{N} \quad\implies\quad f(n) = \Omega(n)$$
> 
> **Conclusión:** $f(n) = \Theta(n)$.

> [!example]- 🟢 Demostración completa — $\log n! = \Theta(n\log n)$
> 
> **Parte 1 — Cota superior:** por propiedades del logaritmo, $\log n! = \log n + \log(n-1) + \cdots + \log 1$. Como $\log$ es creciente, cada término es a lo sumo $\log n$:
> 
> $$\log n! \leq \underbrace{\log n + \log n + \cdots + \log n}_{n \text{ términos}} = n\log n, \quad \forall n \in \mathbb{N}$$
> 
> Esto es, $\log n! = \mathcal{O}(n\log n)$.
> 
> **Parte 2 — Cota inferior (para $n\geq4$):** usando la misma idea de "quedarse con la mitad superior" que en el ejemplo de la suma aritmética,
> 
> $$\log n! \geq \log n + \log(n-1) + \cdots + \log\left\lceil\frac{n}{2}\right\rceil \geq \left\lceil\frac{n+1}{2}\right\rceil\log\left\lceil\frac{n}{2}\right\rceil \geq \frac{n}{2}\log\left(\frac{n}{2}\right) = \frac{n}{2}(\log n - \log 2)$$
> 
> Para $n \geq 4$ se cumple $\frac{n}{2}(\log n - \log 2) \geq \frac{n}{4}\log n$, de modo que $\log n! = \Omega(n\log n)$.
> 
> **Conclusión:** $\log n! = \Theta(n\log n) \quad \blacksquare$
> 
> > [!tip]- 💡 Nota: también se puede intuir con Stirling
> > 
> > La aproximación de Stirling, $n! \approx \sqrt{2\pi n}\left(\frac{n}{e}\right)^n$, da la misma conclusión de forma más rápida pero menos elemental: $\log n! \approx n\log n - n$, cuyo término dominante es $n\log n$. La demostración de arriba es la que usa la clase porque no requiere conocer Stirling.

---

---

## ➡️ Continúa en la Nota II

> [!success] 📋 Siguiente paso
> 
> Ya viste cómo obtener $\mathcal{O}$, $\Omega$ y $\Theta$ a partir de una función matemática. El siguiente paso es aprender a obtenerlas **a partir de pseudocódigo** (contando operaciones en ciclos, recursión, mejor/peor/promedio caso), además de la sección de tiempo real, errores comunes, ejercicios de repaso general y metas de aprendizaje — todo eso está en [[Universidad/3er Semestre/Matemáticas Discretas/Unidad 4 - Recurrencia y Algoritmos/05 - Análisis de Algoritmos - Pseudocódigo y Tiempo Real\|05 - Análisis de Algoritmos - Pseudocódigo y Tiempo Real]].

## 🔗 Conexiones

> [!note] 📋 Temas relacionados
> 
> - [[Universidad/3er Semestre/Matemáticas Discretas/Unidad 4 - Recurrencia y Algoritmos/05 - Análisis de Algoritmos - Pseudocódigo y Tiempo Real\|05 - Análisis de Algoritmos - Pseudocódigo y Tiempo Real]] — segunda parte de esta nota.
> - [[Universidad/3er Semestre/Matemáticas Discretas/Unidad 4 - Recurrencia y Algoritmos/03 - Pseudocódigo y Algoritmos\|03 - Pseudocódigo y Algoritmos]] — la sintaxis de los algoritmos que se analizan en la Nota II.
> - [[Universidad/3er Semestre/Matemáticas Discretas/Unidad 2 - Funciones y Relaciones/04 - Sucesiones y Cadenas\|04 - Sucesiones y Cadenas]] — la notación $\Sigma$ usada en las técnicas de acotación.

## 📚 Referencias

> [!quote] 📖 Fuentes consultadas
> 
> [1] E. Pineda, _Análisis de Algoritmos_, clase MATG1051, ESPOL, jul. 2026.
> 
> [2] K. H. Rosen, _Discrete Mathematics and Its Applications_, 8th ed. New York, USA: McGraw-Hill, 2019, pp. 185–210.
> 
> [3] R. Johnsonbaugh, _Discrete Mathematics_, 8th ed. Hoboken, NJ, USA: Pearson, 2018, pp. 249–268.

---

**Tags:** #analisisdealgoritmos #notacionasintotica #bigO #complejidad #MATG1051 #unidad4 #ESPOL