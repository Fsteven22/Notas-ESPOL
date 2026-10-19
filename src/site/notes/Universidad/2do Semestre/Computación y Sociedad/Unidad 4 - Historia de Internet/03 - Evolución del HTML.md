---
{"dg-publish":true,"permalink":"/universidad/2do-semestre/computacion-y-sociedad/unidad-4-historia-de-internet/03-evolucion-del-html/","dg-note-properties":{}}
---

# 📄 Evolución del HTML: de lo Estático a lo Dinámico

## 🎯 Introducción

> [!info] 💡 Nota: tema de investigación adicional
> 
> A diferencia de las otras notas de esta unidad, este tema no vino directamente de los videos vistos en clase — quedó planteado como una **investigación aparte** sobre lo estático vs. lo dinámico. Esta nota es un punto de partida con el panorama general; conviene ampliarla con las fuentes específicas que pida el profesor.
>

> [!info] 💡 ¿Por qué importa la evolución de HTML?
> 
> HTML (HyperText Markup Language) es el lenguaje que estructura el contenido de cualquier página web. Su evolución —de un lenguaje simple para enlazar documentos de texto, a una plataforma capaz de soportar aplicaciones completas— explica en buena parte cómo fue posible el salto de la [[Universidad/2do Semestre/Computación y Sociedad/Unidad 4 - Historia de Internet/02 - Evolución de la Web\|Web 1.0 estática a la Web 2.0+ dinámica]].
> 
> <svg id="my-svg" width="100%" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" style="max-width: 1190px; background-color: white;" viewBox="100 -61 1190 547" role="graphics-document document" aria-roledescription="timeline"><style>#my-svg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;fill:#333;}@keyframes edge-animation-frame{from{stroke-dashoffset:0;}}@keyframes dash{to{stroke-dashoffset:0;}}#my-svg .edge-animation-slow{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 50s linear infinite;stroke-linecap:round;}#my-svg .edge-animation-fast{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 20s linear infinite;stroke-linecap:round;}#my-svg .error-icon{fill:#552222;}#my-svg .error-text{fill:#552222;stroke:#552222;}#my-svg .edge-thickness-normal{stroke-width:1px;}#my-svg .edge-thickness-thick{stroke-width:3.5px;}#my-svg .edge-pattern-solid{stroke-dasharray:0;}#my-svg .edge-thickness-invisible{stroke-width:0;fill:none;}#my-svg .edge-pattern-dashed{stroke-dasharray:3;}#my-svg .edge-pattern-dotted{stroke-dasharray:2;}#my-svg .marker{fill:#333333;stroke:#333333;}#my-svg .marker.cross{stroke:#333333;}#my-svg svg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;}#my-svg p{margin:0;}#my-svg .edge{stroke-width:3;}#my-svg .section--1 rect,#my-svg .section--1 path,#my-svg .section--1 circle,#my-svg .section--1 path{fill:hsl(240, 100%, 76.2745098039%);}#my-svg .section--1 text{fill:#ffffff;}#my-svg .node-icon--1{font-size:40px;color:#ffffff;}#my-svg .section-edge--1{stroke:hsl(240, 100%, 76.2745098039%);}#my-svg .edge-depth--1{stroke-width:17;}#my-svg .section--1 line{stroke:hsl(60, 100%, 86.2745098039%);stroke-width:3;}#my-svg .lineWrapper line{stroke:#ffffff;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:hsl(80, 100%, 96.2745098039%);}#my-svg .disabled text{fill:#aaaa33;}#my-svg .section-0 rect,#my-svg .section-0 path,#my-svg .section-0 circle,#my-svg .section-0 path{fill:hsl(60, 100%, 73.5294117647%);}#my-svg .section-0 text{fill:black;}#my-svg .node-icon-0{font-size:40px;color:black;}#my-svg .section-edge-0{stroke:hsl(60, 100%, 73.5294117647%);}#my-svg .edge-depth-0{stroke-width:14;}#my-svg .section-0 line{stroke:hsl(240, 100%, 83.5294117647%);stroke-width:3;}#my-svg .lineWrapper line{stroke:black;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:hsl(80, 100%, 96.2745098039%);}#my-svg .disabled text{fill:#aaaa33;}#my-svg .section-1 rect,#my-svg .section-1 path,#my-svg .section-1 circle,#my-svg .section-1 path{fill:hsl(80, 100%, 76.2745098039%);}#my-svg .section-1 text{fill:black;}#my-svg .node-icon-1{font-size:40px;color:black;}#my-svg .section-edge-1{stroke:hsl(80, 100%, 76.2745098039%);}#my-svg .edge-depth-1{stroke-width:11;}#my-svg .section-1 line{stroke:hsl(260, 100%, 86.2745098039%);stroke-width:3;}#my-svg .lineWrapper line{stroke:black;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:hsl(80, 100%, 96.2745098039%);}#my-svg .disabled text{fill:#aaaa33;}#my-svg .section-2 rect,#my-svg .section-2 path,#my-svg .section-2 circle,#my-svg .section-2 path{fill:hsl(270, 100%, 76.2745098039%);}#my-svg .section-2 text{fill:#ffffff;}#my-svg .node-icon-2{font-size:40px;color:#ffffff;}#my-svg .section-edge-2{stroke:hsl(270, 100%, 76.2745098039%);}#my-svg .edge-depth-2{stroke-width:8;}#my-svg .section-2 line{stroke:hsl(90, 100%, 86.2745098039%);stroke-width:3;}#my-svg .lineWrapper line{stroke:#ffffff;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:hsl(80, 100%, 96.2745098039%);}#my-svg .disabled text{fill:#aaaa33;}#my-svg .section-3 rect,#my-svg .section-3 path,#my-svg .section-3 circle,#my-svg .section-3 path{fill:hsl(300, 100%, 76.2745098039%);}#my-svg .section-3 text{fill:black;}#my-svg .node-icon-3{font-size:40px;color:black;}#my-svg .section-edge-3{stroke:hsl(300, 100%, 76.2745098039%);}#my-svg .edge-depth-3{stroke-width:5;}#my-svg .section-3 line{stroke:hsl(120, 100%, 86.2745098039%);stroke-width:3;}#my-svg .lineWrapper line{stroke:black;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:hsl(80, 100%, 96.2745098039%);}#my-svg .disabled text{fill:#aaaa33;}#my-svg .section-4 rect,#my-svg .section-4 path,#my-svg .section-4 circle,#my-svg .section-4 path{fill:hsl(330, 100%, 76.2745098039%);}#my-svg .section-4 text{fill:black;}#my-svg .node-icon-4{font-size:40px;color:black;}#my-svg .section-edge-4{stroke:hsl(330, 100%, 76.2745098039%);}#my-svg .edge-depth-4{stroke-width:2;}#my-svg .section-4 line{stroke:hsl(150, 100%, 86.2745098039%);stroke-width:3;}#my-svg .lineWrapper line{stroke:black;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:hsl(80, 100%, 96.2745098039%);}#my-svg .disabled text{fill:#aaaa33;}#my-svg .section-5 rect,#my-svg .section-5 path,#my-svg .section-5 circle,#my-svg .section-5 path{fill:hsl(0, 100%, 76.2745098039%);}#my-svg .section-5 text{fill:black;}#my-svg .node-icon-5{font-size:40px;color:black;}#my-svg .section-edge-5{stroke:hsl(0, 100%, 76.2745098039%);}#my-svg .edge-depth-5{stroke-width:-1;}#my-svg .section-5 line{stroke:hsl(180, 100%, 86.2745098039%);stroke-width:3;}#my-svg .lineWrapper line{stroke:black;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:hsl(80, 100%, 96.2745098039%);}#my-svg .disabled text{fill:#aaaa33;}#my-svg .section-6 rect,#my-svg .section-6 path,#my-svg .section-6 circle,#my-svg .section-6 path{fill:hsl(30, 100%, 76.2745098039%);}#my-svg .section-6 text{fill:black;}#my-svg .node-icon-6{font-size:40px;color:black;}#my-svg .section-edge-6{stroke:hsl(30, 100%, 76.2745098039%);}#my-svg .edge-depth-6{stroke-width:-4;}#my-svg .section-6 line{stroke:hsl(210, 100%, 86.2745098039%);stroke-width:3;}#my-svg .lineWrapper line{stroke:black;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:hsl(80, 100%, 96.2745098039%);}#my-svg .disabled text{fill:#aaaa33;}#my-svg .section-7 rect,#my-svg .section-7 path,#my-svg .section-7 circle,#my-svg .section-7 path{fill:hsl(90, 100%, 76.2745098039%);}#my-svg .section-7 text{fill:black;}#my-svg .node-icon-7{font-size:40px;color:black;}#my-svg .section-edge-7{stroke:hsl(90, 100%, 76.2745098039%);}#my-svg .edge-depth-7{stroke-width:-7;}#my-svg .section-7 line{stroke:hsl(270, 100%, 86.2745098039%);stroke-width:3;}#my-svg .lineWrapper line{stroke:black;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:hsl(80, 100%, 96.2745098039%);}#my-svg .disabled text{fill:#aaaa33;}#my-svg .section-8 rect,#my-svg .section-8 path,#my-svg .section-8 circle,#my-svg .section-8 path{fill:hsl(150, 100%, 76.2745098039%);}#my-svg .section-8 text{fill:black;}#my-svg .node-icon-8{font-size:40px;color:black;}#my-svg .section-edge-8{stroke:hsl(150, 100%, 76.2745098039%);}#my-svg .edge-depth-8{stroke-width:-10;}#my-svg .section-8 line{stroke:hsl(330, 100%, 86.2745098039%);stroke-width:3;}#my-svg .lineWrapper line{stroke:black;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:hsl(80, 100%, 96.2745098039%);}#my-svg .disabled text{fill:#aaaa33;}#my-svg .section-9 rect,#my-svg .section-9 path,#my-svg .section-9 circle,#my-svg .section-9 path{fill:hsl(180, 100%, 76.2745098039%);}#my-svg .section-9 text{fill:black;}#my-svg .node-icon-9{font-size:40px;color:black;}#my-svg .section-edge-9{stroke:hsl(180, 100%, 76.2745098039%);}#my-svg .edge-depth-9{stroke-width:-13;}#my-svg .section-9 line{stroke:hsl(0, 100%, 86.2745098039%);stroke-width:3;}#my-svg .lineWrapper line{stroke:black;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:hsl(80, 100%, 96.2745098039%);}#my-svg .disabled text{fill:#aaaa33;}#my-svg .section-10 rect,#my-svg .section-10 path,#my-svg .section-10 circle,#my-svg .section-10 path{fill:hsl(210, 100%, 76.2745098039%);}#my-svg .section-10 text{fill:black;}#my-svg .node-icon-10{font-size:40px;color:black;}#my-svg .section-edge-10{stroke:hsl(210, 100%, 76.2745098039%);}#my-svg .edge-depth-10{stroke-width:-16;}#my-svg .section-10 line{stroke:hsl(30, 100%, 86.2745098039%);stroke-width:3;}#my-svg .lineWrapper line{stroke:black;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:hsl(80, 100%, 96.2745098039%);}#my-svg .disabled text{fill:#aaaa33;}#my-svg .section-root rect,#my-svg .section-root path,#my-svg .section-root circle{fill:hsl(240, 100%, 46.2745098039%);}#my-svg .section-root text{fill:#ffffff;}#my-svg .icon-container{height:100%;display:flex;justify-content:center;align-items:center;}#my-svg .edge{fill:none;}#my-svg .eventWrapper{filter:brightness(120%);}#my-svg .node .neo-node{stroke:#9370DB;}#my-svg [data-look="neo"].node rect,#my-svg [data-look="neo"].cluster rect,#my-svg [data-look="neo"].node polygon{stroke:#9370DB;filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#my-svg [data-look="neo"].swimlane.cluster rect{filter:none;}#my-svg [data-look="neo"].node path{stroke:#9370DB;stroke-width:1px;}#my-svg [data-look="neo"].node .outer-path{filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#my-svg [data-look="neo"].node .neo-line path{stroke:#9370DB;filter:none;}#my-svg [data-look="neo"].node circle{stroke:#9370DB;filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#my-svg [data-look="neo"].node circle .state-start{fill:#000000;}#my-svg [data-look="neo"].icon-shape .icon{fill:#9370DB;filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#my-svg [data-look="neo"].icon-shape .icon-neo path{stroke:#9370DB;filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#my-svg :root{--mermaid-font-family:"trebuchet ms",verdana,arial,sans-serif;}</style><g/><g/><defs><marker id="my-svg-arrowhead" refX="5" refY="2" markerWidth="6" markerHeight="4" orient="auto"><path d="M 0,0 V 4 L6,2 Z"/></marker></defs><g class="taskWrapper" transform="translate(200, 50)"><g class="timeline-node section--1"><g><path id="my-svg-node-0" class="node-bkg node-undefined" d="M0 62.8 v-57.8 q0,-5,5,-5 h180 q5,0,5,5 v62.8 H0 Z"/><line class="node-line--1" x1="0" y1="67.8" x2="190" y2="67.8"/></g><g transform="translate(95, 10)"><text dy="1em" alignment-baseline="middle" dominant-baseline="middle" text-anchor="middle"><tspan x="0" dy="1em">1991</tspan></text></g></g></g><g class="lineWrapper"><line x1="295" y1="117.8" x2="295" y2="435.9999938964844" stroke-width="2" stroke="black" marker-end="url(#my-svg-arrowhead)" stroke-dasharray="5,5"/></g><g class="eventWrapper" transform="translate(200, 250)"><g class="timeline-node section--1"><g><path id="my-svg-node-1" class="node-bkg node-undefined" d="M0 60.39999847412109 v-55.39999847412109 q0,-5,5,-5 h180 q5,0,5,5 v60.39999847412109 H0 Z"/><line class="node-line--1" x1="0" y1="65.39999847412109" x2="190" y2="65.39999847412109"/></g><g transform="translate(95, 10)"><text dy="1em" alignment-baseline="middle" dominant-baseline="middle" text-anchor="middle"><tspan x="0" dy="1em">HTML   1.0   (Tim</tspan><tspan x="0" dy="1.1em">Berners-Lee,   CERN)</tspan></text></g></g></g><g class="taskWrapper" transform="translate(400, 50)"><g class="timeline-node section-0"><g><path id="my-svg-node-2" class="node-bkg node-undefined" d="M0 62.8 v-57.8 q0,-5,5,-5 h180 q5,0,5,5 v62.8 H0 Z"/><line class="node-line-0" x1="0" y1="67.8" x2="190" y2="67.8"/></g><g transform="translate(95, 10)"><text dy="1em" alignment-baseline="middle" dominant-baseline="middle" text-anchor="middle"><tspan x="0" dy="1em">1997</tspan></text></g></g></g><g class="lineWrapper"><line x1="495" y1="117.8" x2="495" y2="435.9999938964844" stroke-width="2" stroke="black" marker-end="url(#my-svg-arrowhead)" stroke-dasharray="5,5"/></g><g class="eventWrapper" transform="translate(400, 250)"><g class="timeline-node section-0"><g><path id="my-svg-node-3" class="node-bkg node-undefined" d="M0 77.99999694824218 v-72.99999694824218 q0,-5,5,-5 h180 q5,0,5,5 v77.99999694824218 H0 Z"/><line class="node-line-0" x1="0" y1="82.99999694824218" x2="190" y2="82.99999694824218"/></g><g transform="translate(95, 10)"><text dy="1em" alignment-baseline="middle" dominant-baseline="middle" text-anchor="middle"><tspan x="0" dy="1em">HTML   4.0   —   soporte</tspan><tspan x="0" dy="1.1em">oficial   de   CSS   y</tspan><tspan x="0" dy="1.1em">JavaScript</tspan></text></g></g></g><g class="taskWrapper" transform="translate(600, 50)"><g class="timeline-node section-1"><g><path id="my-svg-node-4" class="node-bkg node-undefined" d="M0 62.8 v-57.8 q0,-5,5,-5 h180 q5,0,5,5 v62.8 H0 Z"/><line class="node-line-1" x1="0" y1="67.8" x2="190" y2="67.8"/></g><g transform="translate(95, 10)"><text dy="1em" alignment-baseline="middle" dominant-baseline="middle" text-anchor="middle"><tspan x="0" dy="1em">2000</tspan></text></g></g></g><g class="lineWrapper"><line x1="695" y1="117.8" x2="695" y2="435.9999938964844" stroke-width="2" stroke="black" marker-end="url(#my-svg-arrowhead)" stroke-dasharray="5,5"/></g><g class="eventWrapper" transform="translate(600, 250)"><g class="timeline-node section-1"><g><path id="my-svg-node-5" class="node-bkg node-undefined" d="M0 77.99999694824218 v-72.99999694824218 q0,-5,5,-5 h180 q5,0,5,5 v77.99999694824218 H0 Z"/><line class="node-line-1" x1="0" y1="82.99999694824218" x2="190" y2="82.99999694824218"/></g><g transform="translate(95, 10)"><text dy="1em" alignment-baseline="middle" dominant-baseline="middle" text-anchor="middle"><tspan x="0" dy="1em">XHTML   —   reglas   más</tspan><tspan x="0" dy="1.1em">estrictas   basadas   en</tspan><tspan x="0" dy="1.1em">XML</tspan></text></g></g></g><g class="taskWrapper" transform="translate(800, 50)"><g class="timeline-node section-2"><g><path id="my-svg-node-6" class="node-bkg node-undefined" d="M0 62.8 v-57.8 q0,-5,5,-5 h180 q5,0,5,5 v62.8 H0 Z"/><line class="node-line-2" x1="0" y1="67.8" x2="190" y2="67.8"/></g><g transform="translate(95, 10)"><text dy="1em" alignment-baseline="middle" dominant-baseline="middle" text-anchor="middle"><tspan x="0" dy="1em">2014</tspan></text></g></g></g><g class="lineWrapper"><line x1="895" y1="117.8" x2="895" y2="435.9999938964844" stroke-width="2" stroke="black" marker-end="url(#my-svg-arrowhead)" stroke-dasharray="5,5"/></g><g class="eventWrapper" transform="translate(800, 250)"><g class="timeline-node section-2"><g><path id="my-svg-node-7" class="node-bkg node-undefined" d="M0 113.19999389648437 v-108.19999389648437 q0,-5,5,-5 h180 q5,0,5,5 v113.19999389648437 H0 Z"/><line class="node-line-2" x1="0" y1="118.19999389648437" x2="190" y2="118.19999389648437"/></g><g transform="translate(95, 10)"><text dy="1em" alignment-baseline="middle" dominant-baseline="middle" text-anchor="middle"><tspan x="0" dy="1em">HTML5</tspan><tspan x="0" dy="1.1em">(W3C/WHATWG)   —</tspan><tspan x="0" dy="1.1em">multimedia   nativa,</tspan><tspan x="0" dy="1.1em">APIs,   diseño</tspan><tspan x="0" dy="1.1em">responsivo</tspan></text></g></g></g><text x="245" font-size="4ex" font-weight="bold" y="20">Evolución de HTML</text><g class="lineWrapper"><line x1="150" y1="167.8" x2="1240" y2="167.8" stroke-width="4" stroke="black" marker-end="url(#my-svg-arrowhead)"/></g></svg>

---

## 📋 Las Versiones de HTML

> [!note] 📋 HTML 1.0 (1991) — El origen
> 
> Creado por Tim Berners-Lee junto con la propia Web ([[Universidad/2do Semestre/Computación y Sociedad/Unidad 4 - Historia de Internet/01 - Historia de Internet y Cómo Funciona\|01 - Historia de Internet y Cómo Funciona]]). Solo permitía estructurar **texto y enlaces** (hipertexto básico): títulos, párrafos, y la posibilidad de conectar un documento con otro mediante hipervínculos.
> 
> - El contenido era **estático**: no cambiaba a menos que alguien editara el archivo manualmente y lo volviera a subir al servidor.
>

> [!note] 📋 HTML 4.0 (1997) — Llega el diseño y la interactividad
> 
> Un punto de inflexión importante: introdujo soporte oficial para dos tecnologías que cambiarían todo:
> 
> - **CSS (Cascading Style Sheets):** permitió separar el **contenido** (HTML) del **diseño visual** (colores, tipografía, layout), en vez de mezclar estilo y estructura en el mismo documento.
> - **JavaScript:** agregó la posibilidad de que la página **reaccionara** a acciones del usuario (clics, formularios, validaciones) sin depender exclusivamente del servidor.
> 
> Este fue el inicio real del salto de páginas estáticas a páginas con comportamiento dinámico.
>

> [!note] 📋 XHTML (2000) — El intento más estricto
> 
> Buscaba aplicar las reglas rígidas de XML a HTML, exigiendo sintaxis más consistente (etiquetas siempre cerradas, anidamiento correcto, etc.) para lograr mayor uniformidad entre navegadores.
> 
> - Resultó **demasiado rígido** para el uso práctico: un solo error de sintaxis podía romper toda la página. Los desarrolladores prefirieron la flexibilidad de HTML tradicional, y XHTML nunca reemplazó a HTML.
>

> [!note] 📋 HTML5 (finalizado en 2014) — La plataforma de aplicaciones
> 
> Desarrollado por WHATWG (Web Hypertext Application Technology Working Group) y adoptado formalmente por el W3C. Es la versión que consolidó a la Web como una **plataforma de aplicaciones**, no solo de documentos.
> 
> - **Elementos semánticos:** etiquetas que describen el significado de una sección (como encabezado, artículo, navegación), mejorando estructura y accesibilidad.
> - **Multimedia nativa:** soporte directo de audio y video sin depender de plugins externos como Flash.
> - **APIs nuevas:** geolocalización, almacenamiento offline, arrastrar y soltar (drag-and-drop), entre otras.
> - **Diseño responsivo:** mejor soporte para que una misma página se adapte a distintos tamaños de pantalla (móvil, tablet, escritorio).

---

## 🔀 Contenido Estático vs. Contenido Dinámico

> [!success] ✅ La distinción clave del tema
> 
> - **Contenido estático:** el HTML que recibe el navegador es siempre el mismo, sin importar quién lo pida ni cuándo. Es como una hoja impresa: igual para todos los que la lean.
> - **Contenido dinámico:** el servidor genera o modifica el HTML en el momento, según datos, usuario o interacción (ej. tu feed de una red social, resultados de una búsqueda, un carrito de compras que cambia según lo que agregas).
> 
> El contenido dinámico se logra combinando HTML con lenguajes del **lado del servidor** (que generan el HTML antes de enviarlo, como PHP) y del **lado del cliente** (que modifican la página ya cargada en el navegador, como JavaScript).
>

> [!example]- 🟢 Ejemplo comparativo
> 
> - **Página estática:** un archivo `about.html` con la historia de una empresa. Todos los visitantes ven exactamente el mismo texto e imágenes, sin importar quién sean o cuándo entren.
> - **Página dinámica:** la página de inicio de una red social. Cada usuario ve un contenido distinto (sus propias publicaciones, las de sus contactos), generado en el momento según quién inició sesión.

---

## ⚠️ Errores Comunes

> [!warning] ⚠️ HTML por sí solo no hace nada "dinámico"
> 
> HTML sigue siendo, en esencia, un lenguaje de **estructura** (marcado), no de lógica o comportamiento. Lo que hace posible el contenido dinámico es la combinación de HTML con otras tecnologías (CSS para diseño, JavaScript para interactividad, y lenguajes del servidor para generar contenido personalizado) — no un cambio en la naturaleza del propio HTML.
>

> [!warning] ⚠️ XHTML no fue "una versión de HTML5"
> 
> Es un error común mezclar el orden: XHTML (2000) es anterior a HTML5 (2014) y fue, en la práctica, un experimento que no prosperó por su rigidez, no un paso intermedio necesario hacia HTML5.

---

## 📝 Ejercicios Progresivos

> [!question] 🟩 Nivel 1 — Básico
> 
> 1. ¿Qué podía hacer HTML 1.0 y qué no podía hacer, en comparación con el HTML actual?
> 2. Define con tus propias palabras "contenido estático" y "contenido dinámico".
> 3. ¿Qué dos tecnologías introdujo oficialmente HTML 4.0 en 1997?
>

> [!question] 🟨 Nivel 2 — Intermedio
> 
> 4. Explica por qué XHTML no logró reemplazar a HTML, a pesar de buscar mayor consistencia.
> 5. Da un ejemplo propio (distinto al de la nota) de una página estática y una dinámica, explicando por qué cada una encaja en esa categoría.
>

> [!question] 🟥 Nivel 3 — Avanzado
> 
> 6. Compara HTML 1.0 con HTML5: ¿qué cambió en términos de contenido estático vs. dinámico, y qué tecnologías hicieron posible ese cambio?
> 7. Explica por qué se dice que "HTML por sí solo sigue siendo un lenguaje de estructura", incluso después de HTML5, que se asocia tanto con aplicaciones dinámicas.
>

> [!success]- ✅ Respuestas
> 
> **Nivel 1:**
> 
> 8. HTML 1.0 solo podía estructurar texto y crear enlaces entre documentos (hipertexto básico). No podía separar diseño de contenido (no existía CSS aún) ni reaccionar a acciones del usuario (no existía JavaScript), por lo que las páginas eran completamente estáticas.
> 9. Contenido estático es aquel que se muestra igual a todos los usuarios sin cambiar, como un documento fijo. Contenido dinámico es aquel que el servidor genera o modifica según el usuario, sus datos o sus acciones en el momento.
> 10. CSS (para separar diseño de contenido) y JavaScript (para agregar interactividad).
> 
> **Nivel 2:**
> 
> 11. Porque exigía una sintaxis demasiado estricta (basada en reglas de XML), donde un solo error rompía toda la página. Los desarrolladores prefirieron la flexibilidad de HTML tradicional, que tolera mejor los errores de sintaxis sin dejar de renderizar la página.
> 12. Respuesta abierta — ejemplo válido: una página estática sería un currículum en HTML simple que no cambia para nadie; una dinámica sería un buscador de vuelos, donde los resultados que ves dependen de la fecha y destino que ingresaste.
> 
> **Nivel 3:**
> 
> 13. HTML 1.0 solo estructuraba texto y enlaces; el contenido era fijo y no cambiaba sin editar el archivo manualmente (estático). HTML5, apoyado en CSS (diseño), JavaScript (interactividad) y comunicación con servidores, permite que el contenido se genere o actualice en tiempo real según el usuario o sus acciones (dinámico) — por ejemplo, cargar nuevo contenido sin recargar la página completa.
> 14. Porque la función de HTML sigue siendo describir la estructura y el significado del contenido (títulos, párrafos, secciones), no ejecutar lógica ni tomar decisiones. Lo "dinámico" de las aplicaciones modernas viene de JavaScript (comportamiento) y de lenguajes del lado del servidor (generación de contenido personalizado) trabajando junto con HTML, no de un cambio en lo que HTML en sí mismo hace.

---

## 🎯 Metas de Aprendizaje

> [!success] ✅ Nivel Básico
> 
> - [ ] Puedo ordenar cronológicamente las versiones principales de HTML (1.0, 4.0, XHTML, HTML5).
> - [ ] Puedo definir contenido estático y contenido dinámico.
>

> [!success] ✅ Nivel Intermedio
> 
> - [ ] Entiendo qué aportó cada versión de HTML (CSS/JS en 4.0, rigidez de XHTML, multimedia/APIs en HTML5).
> - [ ] Puedo dar ejemplos propios de páginas estáticas y dinámicas.
>

> [!success] ✅ Nivel Avanzado
> 
> - [ ] Puedo explicar por qué HTML sigue siendo un lenguaje de estructura aunque soporte aplicaciones dinámicas.
> - [ ] Puedo relacionar la evolución de HTML con la evolución de la Web ([[Universidad/2do Semestre/Computación y Sociedad/Unidad 4 - Historia de Internet/02 - Evolución de la Web\|02 - Evolución de la Web]]).

---

## 📚 Referencias y Conexiones

> [!quote] 📖 Fuentes consultadas
> 
> [1] Investigación complementaria — Unidad 4: Internet, Computación y Sociedad (tema no cubierto directamente en los videos de clase). [2] World Wide Web Consortium (W3C) / WHATWG — historial de especificaciones de HTML5.
>

> [!quote] 🔗 Conexiones
> 
> - [[Universidad/2do Semestre/Computación y Sociedad/Unidad 4 - Historia de Internet/01 - Historia de Internet y Cómo Funciona\|01 - Historia de Internet y Cómo Funciona]] — contexto de cuándo y por qué se creó HTML junto con la Web.
> - [[Universidad/2do Semestre/Computación y Sociedad/Unidad 4 - Historia de Internet/02 - Evolución de la Web\|02 - Evolución de la Web]] — cómo los cambios en HTML habilitaron el salto de Web 1.0 a las generaciones posteriores.

---

**Tags:** #computacion-y-sociedad #internet #html #html5 #contenido-dinamico #unidad4