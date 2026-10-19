---
{"dg-publish":true,"permalink":"/universidad/1er-semestre/calculo-de-una-variable/unidad-05-integrales/iv-integrales-impropias-y-avanzadas/01-integrales-impropias/","dg-note-properties":{}}
---


# 🚀 Integrales Impropias

## 📖 Introducción

> [!info] 💡 Concepto Fundamental
> Una **integral impropia** es una integral definida que tiene una o más de las siguientes características:
> - **Límites de integración infinitos** (uno o ambos)
> - **Integrandos con discontinuidades infinitas** en el intervalo de integración
> - **Combinación de ambas** situaciones
> 
> Se evalúan como **límites de integrales definidas** para determinar si **convergen** o **divergen**.
>

> [!tip] 🎯 ¿Por qué son importantes?
> - Permiten calcular **áreas infinitas** bajo curvas
> - Fundamentales en **análisis de series** y **transformadas**
> - Aplicaciones en **probabilidad** (distribuciones continuas)
> - Modelan fenómenos **físicos ilimitados** (campos, ondas)
> - Base teórica para **análisis de Fourier**
> - Esenciales en **ecuaciones diferenciales** avanzadas

## 🔗 Conexiones con Otros Temas

> [!info] 🌐 Temas Relacionados y Conexiones
> 
> **Fundamentos Previos**:
> • **Integrales definidas** - Base conceptual fundamental
> • **Límites** - Herramienta principal para evaluar integrales impropias
> • **Antiderivadas** - Necesarias para calcular las integrales
> • **Continuidad** - Para identificar puntos problemáticos
> • **Teorema Fundamental del Cálculo** - Marco teórico
> 
> **Desarrollos Posteriores**:
> • **Series infinitas** - Criterios de convergencia similares
> • **Transformadas de Laplace** - Aplicación directa
> • **Análisis de Fourier** - Series y transformadas
> • **Distribuciones de probabilidad** - Funciones de densidad
> • **Ecuaciones diferenciales** - Soluciones con condiciones de frontera
> • **Análisis complejo** - Integrales de contorno

<svg id="my-svg" width="100%" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" class="mindmapDiagram" style="max-width: 976.079px; background-color: white;" viewBox="5 5 976.0794677734375 484.8065490722656" role="graphics-document document" aria-roledescription="mindmap"><style>#my-svg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;fill:#333;}@keyframes edge-animation-frame{from{stroke-dashoffset:0;}}@keyframes dash{to{stroke-dashoffset:0;}}#my-svg .edge-animation-slow{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 50s linear infinite;stroke-linecap:round;}#my-svg .edge-animation-fast{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 20s linear infinite;stroke-linecap:round;}#my-svg .error-icon{fill:#552222;}#my-svg .error-text{fill:#552222;stroke:#552222;}#my-svg .edge-thickness-normal{stroke-width:1px;}#my-svg .edge-thickness-thick{stroke-width:3.5px;}#my-svg .edge-pattern-solid{stroke-dasharray:0;}#my-svg .edge-thickness-invisible{stroke-width:0;fill:none;}#my-svg .edge-pattern-dashed{stroke-dasharray:3;}#my-svg .edge-pattern-dotted{stroke-dasharray:2;}#my-svg .marker{fill:#333333;stroke:#333333;}#my-svg .marker.cross{stroke:#333333;}#my-svg svg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;}#my-svg p{margin:0;}#my-svg .edge{stroke-width:3;}#my-svg .section--1 rect,#my-svg .section--1 path,#my-svg .section--1 circle,#my-svg .section--1 polygon,#my-svg .section--1 path{fill:hsl(240, 100%, 76.2745098039%);}#my-svg .section--1 text{fill:#ffffff;}#my-svg .section--1 span{color:#ffffff;}#my-svg .node-icon--1{font-size:40px;color:#ffffff;}#my-svg .section-edge--1{stroke:hsl(240, 100%, 76.2745098039%);}#my-svg .edge-depth--1{stroke-width:17;}#my-svg .section--1 line{stroke:hsl(60, 100%, 86.2745098039%);stroke-width:3;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:lightgray;}#my-svg .disabled text{fill:#efefef;}#my-svg [data-look="neo"].mindmap-node.section--1 rect,#my-svg [data-look="neo"].mindmap-node.section--1 path,#my-svg [data-look="neo"].mindmap-node.section--1 circle,#my-svg [data-look="neo"].mindmap-node.section--1 polygon{fill:hsl(240, 100%, 76.2745098039%);stroke:hsl(240, 100%, 76.2745098039%);stroke-width:1px;}#my-svg [data-look="neo"].section-edge--1{stroke:hsl(240, 100%, 76.2745098039%);}#my-svg [data-look="neo"].mindmap-node.section--1 text{fill:#ffffff;}#my-svg .section-0 rect,#my-svg .section-0 path,#my-svg .section-0 circle,#my-svg .section-0 polygon,#my-svg .section-0 path{fill:hsl(60, 100%, 73.5294117647%);}#my-svg .section-0 text{fill:black;}#my-svg .section-0 span{color:black;}#my-svg .node-icon-0{font-size:40px;color:black;}#my-svg .section-edge-0{stroke:hsl(60, 100%, 73.5294117647%);}#my-svg .edge-depth-0{stroke-width:14;}#my-svg .section-0 line{stroke:hsl(240, 100%, 83.5294117647%);stroke-width:3;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:lightgray;}#my-svg .disabled text{fill:#efefef;}#my-svg [data-look="neo"].mindmap-node.section-0 rect,#my-svg [data-look="neo"].mindmap-node.section-0 path,#my-svg [data-look="neo"].mindmap-node.section-0 circle,#my-svg [data-look="neo"].mindmap-node.section-0 polygon{fill:hsl(60, 100%, 73.5294117647%);stroke:hsl(60, 100%, 73.5294117647%);stroke-width:1px;}#my-svg [data-look="neo"].section-edge-0{stroke:hsl(60, 100%, 73.5294117647%);}#my-svg [data-look="neo"].mindmap-node.section-0 text{fill:black;}#my-svg .section-1 rect,#my-svg .section-1 path,#my-svg .section-1 circle,#my-svg .section-1 polygon,#my-svg .section-1 path{fill:hsl(80, 100%, 76.2745098039%);}#my-svg .section-1 text{fill:black;}#my-svg .section-1 span{color:black;}#my-svg .node-icon-1{font-size:40px;color:black;}#my-svg .section-edge-1{stroke:hsl(80, 100%, 76.2745098039%);}#my-svg .edge-depth-1{stroke-width:11;}#my-svg .section-1 line{stroke:hsl(260, 100%, 86.2745098039%);stroke-width:3;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:lightgray;}#my-svg .disabled text{fill:#efefef;}#my-svg [data-look="neo"].mindmap-node.section-1 rect,#my-svg [data-look="neo"].mindmap-node.section-1 path,#my-svg [data-look="neo"].mindmap-node.section-1 circle,#my-svg [data-look="neo"].mindmap-node.section-1 polygon{fill:hsl(80, 100%, 76.2745098039%);stroke:hsl(80, 100%, 76.2745098039%);stroke-width:1px;}#my-svg [data-look="neo"].section-edge-1{stroke:hsl(80, 100%, 76.2745098039%);}#my-svg [data-look="neo"].mindmap-node.section-1 text{fill:black;}#my-svg .section-2 rect,#my-svg .section-2 path,#my-svg .section-2 circle,#my-svg .section-2 polygon,#my-svg .section-2 path{fill:hsl(270, 100%, 76.2745098039%);}#my-svg .section-2 text{fill:#ffffff;}#my-svg .section-2 span{color:#ffffff;}#my-svg .node-icon-2{font-size:40px;color:#ffffff;}#my-svg .section-edge-2{stroke:hsl(270, 100%, 76.2745098039%);}#my-svg .edge-depth-2{stroke-width:8;}#my-svg .section-2 line{stroke:hsl(90, 100%, 86.2745098039%);stroke-width:3;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:lightgray;}#my-svg .disabled text{fill:#efefef;}#my-svg [data-look="neo"].mindmap-node.section-2 rect,#my-svg [data-look="neo"].mindmap-node.section-2 path,#my-svg [data-look="neo"].mindmap-node.section-2 circle,#my-svg [data-look="neo"].mindmap-node.section-2 polygon{fill:hsl(270, 100%, 76.2745098039%);stroke:hsl(270, 100%, 76.2745098039%);stroke-width:1px;}#my-svg [data-look="neo"].section-edge-2{stroke:hsl(270, 100%, 76.2745098039%);}#my-svg [data-look="neo"].mindmap-node.section-2 text{fill:#ffffff;}#my-svg .section-3 rect,#my-svg .section-3 path,#my-svg .section-3 circle,#my-svg .section-3 polygon,#my-svg .section-3 path{fill:hsl(300, 100%, 76.2745098039%);}#my-svg .section-3 text{fill:black;}#my-svg .section-3 span{color:black;}#my-svg .node-icon-3{font-size:40px;color:black;}#my-svg .section-edge-3{stroke:hsl(300, 100%, 76.2745098039%);}#my-svg .edge-depth-3{stroke-width:5;}#my-svg .section-3 line{stroke:hsl(120, 100%, 86.2745098039%);stroke-width:3;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:lightgray;}#my-svg .disabled text{fill:#efefef;}#my-svg [data-look="neo"].mindmap-node.section-3 rect,#my-svg [data-look="neo"].mindmap-node.section-3 path,#my-svg [data-look="neo"].mindmap-node.section-3 circle,#my-svg [data-look="neo"].mindmap-node.section-3 polygon{fill:hsl(300, 100%, 76.2745098039%);stroke:hsl(300, 100%, 76.2745098039%);stroke-width:1px;}#my-svg [data-look="neo"].section-edge-3{stroke:hsl(300, 100%, 76.2745098039%);}#my-svg [data-look="neo"].mindmap-node.section-3 text{fill:black;}#my-svg .section-4 rect,#my-svg .section-4 path,#my-svg .section-4 circle,#my-svg .section-4 polygon,#my-svg .section-4 path{fill:hsl(330, 100%, 76.2745098039%);}#my-svg .section-4 text{fill:black;}#my-svg .section-4 span{color:black;}#my-svg .node-icon-4{font-size:40px;color:black;}#my-svg .section-edge-4{stroke:hsl(330, 100%, 76.2745098039%);}#my-svg .edge-depth-4{stroke-width:2;}#my-svg .section-4 line{stroke:hsl(150, 100%, 86.2745098039%);stroke-width:3;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:lightgray;}#my-svg .disabled text{fill:#efefef;}#my-svg [data-look="neo"].mindmap-node.section-4 rect,#my-svg [data-look="neo"].mindmap-node.section-4 path,#my-svg [data-look="neo"].mindmap-node.section-4 circle,#my-svg [data-look="neo"].mindmap-node.section-4 polygon{fill:hsl(330, 100%, 76.2745098039%);stroke:hsl(330, 100%, 76.2745098039%);stroke-width:1px;}#my-svg [data-look="neo"].section-edge-4{stroke:hsl(330, 100%, 76.2745098039%);}#my-svg [data-look="neo"].mindmap-node.section-4 text{fill:black;}#my-svg .section-5 rect,#my-svg .section-5 path,#my-svg .section-5 circle,#my-svg .section-5 polygon,#my-svg .section-5 path{fill:hsl(0, 100%, 76.2745098039%);}#my-svg .section-5 text{fill:black;}#my-svg .section-5 span{color:black;}#my-svg .node-icon-5{font-size:40px;color:black;}#my-svg .section-edge-5{stroke:hsl(0, 100%, 76.2745098039%);}#my-svg .edge-depth-5{stroke-width:-1;}#my-svg .section-5 line{stroke:hsl(180, 100%, 86.2745098039%);stroke-width:3;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:lightgray;}#my-svg .disabled text{fill:#efefef;}#my-svg [data-look="neo"].mindmap-node.section-5 rect,#my-svg [data-look="neo"].mindmap-node.section-5 path,#my-svg [data-look="neo"].mindmap-node.section-5 circle,#my-svg [data-look="neo"].mindmap-node.section-5 polygon{fill:hsl(0, 100%, 76.2745098039%);stroke:hsl(0, 100%, 76.2745098039%);stroke-width:1px;}#my-svg [data-look="neo"].section-edge-5{stroke:hsl(0, 100%, 76.2745098039%);}#my-svg [data-look="neo"].mindmap-node.section-5 text{fill:black;}#my-svg .section-6 rect,#my-svg .section-6 path,#my-svg .section-6 circle,#my-svg .section-6 polygon,#my-svg .section-6 path{fill:hsl(30, 100%, 76.2745098039%);}#my-svg .section-6 text{fill:black;}#my-svg .section-6 span{color:black;}#my-svg .node-icon-6{font-size:40px;color:black;}#my-svg .section-edge-6{stroke:hsl(30, 100%, 76.2745098039%);}#my-svg .edge-depth-6{stroke-width:-4;}#my-svg .section-6 line{stroke:hsl(210, 100%, 86.2745098039%);stroke-width:3;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:lightgray;}#my-svg .disabled text{fill:#efefef;}#my-svg [data-look="neo"].mindmap-node.section-6 rect,#my-svg [data-look="neo"].mindmap-node.section-6 path,#my-svg [data-look="neo"].mindmap-node.section-6 circle,#my-svg [data-look="neo"].mindmap-node.section-6 polygon{fill:hsl(30, 100%, 76.2745098039%);stroke:hsl(30, 100%, 76.2745098039%);stroke-width:1px;}#my-svg [data-look="neo"].section-edge-6{stroke:hsl(30, 100%, 76.2745098039%);}#my-svg [data-look="neo"].mindmap-node.section-6 text{fill:black;}#my-svg .section-7 rect,#my-svg .section-7 path,#my-svg .section-7 circle,#my-svg .section-7 polygon,#my-svg .section-7 path{fill:hsl(90, 100%, 76.2745098039%);}#my-svg .section-7 text{fill:black;}#my-svg .section-7 span{color:black;}#my-svg .node-icon-7{font-size:40px;color:black;}#my-svg .section-edge-7{stroke:hsl(90, 100%, 76.2745098039%);}#my-svg .edge-depth-7{stroke-width:-7;}#my-svg .section-7 line{stroke:hsl(270, 100%, 86.2745098039%);stroke-width:3;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:lightgray;}#my-svg .disabled text{fill:#efefef;}#my-svg [data-look="neo"].mindmap-node.section-7 rect,#my-svg [data-look="neo"].mindmap-node.section-7 path,#my-svg [data-look="neo"].mindmap-node.section-7 circle,#my-svg [data-look="neo"].mindmap-node.section-7 polygon{fill:hsl(90, 100%, 76.2745098039%);stroke:hsl(90, 100%, 76.2745098039%);stroke-width:1px;}#my-svg [data-look="neo"].section-edge-7{stroke:hsl(90, 100%, 76.2745098039%);}#my-svg [data-look="neo"].mindmap-node.section-7 text{fill:black;}#my-svg .section-8 rect,#my-svg .section-8 path,#my-svg .section-8 circle,#my-svg .section-8 polygon,#my-svg .section-8 path{fill:hsl(150, 100%, 76.2745098039%);}#my-svg .section-8 text{fill:black;}#my-svg .section-8 span{color:black;}#my-svg .node-icon-8{font-size:40px;color:black;}#my-svg .section-edge-8{stroke:hsl(150, 100%, 76.2745098039%);}#my-svg .edge-depth-8{stroke-width:-10;}#my-svg .section-8 line{stroke:hsl(330, 100%, 86.2745098039%);stroke-width:3;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:lightgray;}#my-svg .disabled text{fill:#efefef;}#my-svg [data-look="neo"].mindmap-node.section-8 rect,#my-svg [data-look="neo"].mindmap-node.section-8 path,#my-svg [data-look="neo"].mindmap-node.section-8 circle,#my-svg [data-look="neo"].mindmap-node.section-8 polygon{fill:hsl(150, 100%, 76.2745098039%);stroke:hsl(150, 100%, 76.2745098039%);stroke-width:1px;}#my-svg [data-look="neo"].section-edge-8{stroke:hsl(150, 100%, 76.2745098039%);}#my-svg [data-look="neo"].mindmap-node.section-8 text{fill:black;}#my-svg .section-9 rect,#my-svg .section-9 path,#my-svg .section-9 circle,#my-svg .section-9 polygon,#my-svg .section-9 path{fill:hsl(180, 100%, 76.2745098039%);}#my-svg .section-9 text{fill:black;}#my-svg .section-9 span{color:black;}#my-svg .node-icon-9{font-size:40px;color:black;}#my-svg .section-edge-9{stroke:hsl(180, 100%, 76.2745098039%);}#my-svg .edge-depth-9{stroke-width:-13;}#my-svg .section-9 line{stroke:hsl(0, 100%, 86.2745098039%);stroke-width:3;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:lightgray;}#my-svg .disabled text{fill:#efefef;}#my-svg [data-look="neo"].mindmap-node.section-9 rect,#my-svg [data-look="neo"].mindmap-node.section-9 path,#my-svg [data-look="neo"].mindmap-node.section-9 circle,#my-svg [data-look="neo"].mindmap-node.section-9 polygon{fill:hsl(180, 100%, 76.2745098039%);stroke:hsl(180, 100%, 76.2745098039%);stroke-width:1px;}#my-svg [data-look="neo"].section-edge-9{stroke:hsl(180, 100%, 76.2745098039%);}#my-svg [data-look="neo"].mindmap-node.section-9 text{fill:black;}#my-svg .section-10 rect,#my-svg .section-10 path,#my-svg .section-10 circle,#my-svg .section-10 polygon,#my-svg .section-10 path{fill:hsl(210, 100%, 76.2745098039%);}#my-svg .section-10 text{fill:black;}#my-svg .section-10 span{color:black;}#my-svg .node-icon-10{font-size:40px;color:black;}#my-svg .section-edge-10{stroke:hsl(210, 100%, 76.2745098039%);}#my-svg .edge-depth-10{stroke-width:-16;}#my-svg .section-10 line{stroke:hsl(30, 100%, 86.2745098039%);stroke-width:3;}#my-svg .disabled,#my-svg .disabled circle,#my-svg .disabled text{fill:lightgray;}#my-svg .disabled text{fill:#efefef;}#my-svg [data-look="neo"].mindmap-node.section-10 rect,#my-svg [data-look="neo"].mindmap-node.section-10 path,#my-svg [data-look="neo"].mindmap-node.section-10 circle,#my-svg [data-look="neo"].mindmap-node.section-10 polygon{fill:hsl(210, 100%, 76.2745098039%);stroke:hsl(210, 100%, 76.2745098039%);stroke-width:1px;}#my-svg [data-look="neo"].section-edge-10{stroke:hsl(210, 100%, 76.2745098039%);}#my-svg [data-look="neo"].mindmap-node.section-10 text{fill:black;}#my-svg .section-root rect,#my-svg .section-root path,#my-svg .section-root circle,#my-svg .section-root polygon{fill:hsl(240, 100%, 46.2745098039%);}#my-svg .section-root text{fill:#ffffff;}#my-svg .section-root span{color:#ffffff;}#my-svg .icon-container{height:100%;display:flex;justify-content:center;align-items:center;}#my-svg .edge{fill:none;}#my-svg .mindmap-node-label{dy:1em;alignment-baseline:middle;text-anchor:middle;dominant-baseline:middle;text-align:center;}#my-svg [data-look="neo"].mindmap-node{filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#my-svg [data-look="neo"].mindmap-node.section-root rect,#my-svg [data-look="neo"].mindmap-node.section-root path,#my-svg [data-look="neo"].mindmap-node.section-root circle,#my-svg [data-look="neo"].mindmap-node.section-root polygon{fill:hsl(240, 100%, 46.2745098039%);}#my-svg [data-look="neo"].mindmap-node.section-root .text-inner-tspan{fill:#ffffff;}#my-svg .node .neo-node{stroke:#9370DB;}#my-svg [data-look="neo"].node rect,#my-svg [data-look="neo"].cluster rect,#my-svg [data-look="neo"].node polygon{stroke:#9370DB;filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#my-svg [data-look="neo"].swimlane.cluster rect{filter:none;}#my-svg [data-look="neo"].node path{stroke:#9370DB;stroke-width:1px;}#my-svg [data-look="neo"].node .outer-path{filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#my-svg [data-look="neo"].node .neo-line path{stroke:#9370DB;filter:none;}#my-svg [data-look="neo"].node circle{stroke:#9370DB;filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#my-svg [data-look="neo"].node circle .state-start{fill:#000000;}#my-svg [data-look="neo"].icon-shape .icon{fill:#9370DB;filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#my-svg [data-look="neo"].icon-shape .icon-neo path{stroke:#9370DB;filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#my-svg :root{--mermaid-font-family:"trebuchet ms",verdana,arial,sans-serif;}</style><g><marker id="my-svg_mindmap-pointEnd" class="marker mindmap" viewBox="0 0 10 10" refX="5" refY="5" markerUnits="userSpaceOnUse" markerWidth="8" markerHeight="8" orient="auto"><path d="M 0 0 L 10 5 L 0 10 z" class="arrowMarkerPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"/></marker><marker id="my-svg_mindmap-pointStart" class="marker mindmap" viewBox="0 0 10 10" refX="4.5" refY="5" markerUnits="userSpaceOnUse" markerWidth="8" markerHeight="8" orient="auto"><path d="M 0 5 L 10 10 L 10 0 z" class="arrowMarkerPath" style="stroke-width: 1; stroke-dasharray: 1, 0;"/></marker><marker id="my-svg_mindmap-pointEnd-margin" class="marker mindmap" viewBox="0 0 11.5 14" refX="11.5" refY="7" markerUnits="userSpaceOnUse" markerWidth="10.5" markerHeight="14" orient="auto"><path d="M 0 0 L 11.5 7 L 0 14 z" class="arrowMarkerPath" style="stroke-width: 0; stroke-dasharray: 1, 0;"/></marker><marker id="my-svg_mindmap-pointStart-margin" class="marker mindmap" viewBox="0 0 11.5 14" refX="1" refY="7" markerUnits="userSpaceOnUse" markerWidth="11.5" markerHeight="14" orient="auto"><polygon points="0,7 11.5,14 11.5,0" class="arrowMarkerPath" style="stroke-width: 0; stroke-dasharray: 1, 0;"/></marker><g class="subgraphs"/><g class="edgePaths"><path d="M508.144,267.683L520.518,269.367C532.892,271.05,557.639,274.418,582.387,277.785C607.134,281.152,631.882,284.52,644.256,286.203L656.629,287.887" id="my-svg-edge_0_1" class="edge-thickness-normal edge-pattern-solid edge section-edge-0 edge-depth-1" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_0_1" data-points="W3sieCI6NTA4LjE0NDI0MjgzOTc3MDIsInkiOjI2Ny42ODI5MjgwNjE0NTY4fSx7IngiOjU4Mi4zODY3OTI0NjgwOTM5LCJ5IjoyNzcuNzg0OTY1MzA1NzgxNn0seyJ4Ijo2NTYuNjI5MzQyMDk2NDE3NSwieSI6Mjg3Ljg4NzAwMjU1MDEwNjQ0fV0=" data-look="classic"/><path d="M686.37,291.821L700.271,293.607C714.173,295.393,741.975,298.965,769.778,302.537C797.581,306.109,825.383,309.682,839.285,311.468L853.186,313.254" id="my-svg-edge_1_2" class="edge-thickness-normal edge-pattern-solid edge section-edge-0 edge-depth-3" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_1_2" data-points="W3sieCI6Njg2LjM3MDA4NzA4NDI1MjYsInkiOjI5MS44MjA5MDQwMzQ0Mjh9LHsieCI6NzY5Ljc3ODA3Mjk0NTU3MSwieSI6MzAyLjUzNzMyNjk4OTk3NTY3fSx7IngiOjg1My4xODYwNTg4MDY4ODk2LCJ5IjozMTMuMjUzNzQ5OTQ1NTIzMzR9XQ==" data-look="classic"/><path d="M674.876,304.523L675.989,309.329C677.102,314.136,679.328,323.749,681.554,333.362C683.78,342.975,686.006,352.588,687.119,357.395L688.232,362.201" id="my-svg-edge_1_3" class="edge-thickness-normal edge-pattern-solid edge section-edge-0 edge-depth-3" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_1_3" data-points="W3sieCI6Njc0Ljg3NjE1MTE1OTQzOSwieSI6MzA0LjUyMjc0MDgzMDY4Nzl9LHsieCI6NjgxLjU1Mzk3MjM4OTU3MjQsInkiOjMzMy4zNjE5OTIxNzU4NzEzfSx7IngiOjY4OC4yMzE3OTM2MTk3MDU5LCJ5IjozNjIuMjAxMjQzNTIxMDU0N31d" data-look="classic"/><path d="M682.783,280.034L687.564,275.853C692.345,271.671,701.908,263.308,711.47,254.945C721.032,246.582,730.594,238.219,735.375,234.038L740.156,229.856" id="my-svg-edge_1_4" class="edge-thickness-normal edge-pattern-solid edge section-edge-0 edge-depth-3" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_1_4" data-points="W3sieCI6NjgyLjc4MzI3NjkwNzUwNDQsInkiOjI4MC4wMzQzODM0NzI4MTk2fSx7IngiOjcxMS40Njk2NzEzNDYzNjYxLCJ5IjoyNTQuOTQ1Mjk1NjgxOTExMzh9LHsieCI6NzQwLjE1NjA2NTc4NTIyNzgsInkiOjIyOS44NTYyMDc4OTEwMDMxMn1d" data-look="classic"/><path d="M482.136,275.7L471.967,284.86C461.798,294.02,441.461,312.34,421.123,330.659C400.785,348.979,380.447,367.299,370.279,376.459L360.11,385.619" id="my-svg-edge_0_5" class="edge-thickness-normal edge-pattern-solid edge section-edge-1 edge-depth-1" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_0_5" data-points="W3sieCI6NDgyLjEzNjEyNjAwNjQwOTIsInkiOjI3NS42OTk4Mjk1NzMxNzIyfSx7IngiOjQyMS4xMjI5MTc3MDA0MTE4LCJ5IjozMzAuNjU5NDM3Nzc2ODEwOH0seyJ4IjozNjAuMTA5NzA5Mzk0NDE0NCwieSI6Mzg1LjYxOTA0NTk4MDQ0OTR9XQ==" data-look="classic"/><path d="M339.523,384.002L335.988,379.638C332.453,375.273,325.383,366.544,318.313,357.815C311.242,349.086,304.172,340.357,300.637,335.993L297.102,331.628" id="my-svg-edge_5_6" class="edge-thickness-normal edge-pattern-solid edge section-edge-1 edge-depth-3" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_5_6" data-points="W3sieCI6MzM5LjUyMzQ3MjI3MzIxNTEsInkiOjM4NC4wMDIyMzk2MDQzMTY2fSx7IngiOjMxOC4zMTI2NzcwNTM2NjQ1LCJ5IjozNTcuODE1MzExMzQ1MzA2OH0seyJ4IjoyOTcuMTAxODgxODM0MTEzOTUsInkiOjMzMS42MjgzODMwODYyOTY5NH1d" data-look="classic"/><path d="M361.907,403.24L368.569,407.143C375.231,411.045,388.555,418.85,401.879,426.655C415.203,434.46,428.526,442.265,435.188,446.167L441.85,450.07" id="my-svg-edge_5_7" class="edge-thickness-normal edge-pattern-solid edge section-edge-1 edge-depth-3" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_5_7" data-points="W3sieCI6MzYxLjkwNzQ2MjQ2NDExNSwieSI6NDAzLjI0MDA5Njc2NTg3Nzd9LHsieCI6NDAxLjg3ODc5MjM3NTkyMDc0LCJ5Ijo0MjYuNjU0ODU0MTE4NzQ5Mzd9LHsieCI6NDQxLjg1MDEyMjI4NzcyNjUsInkiOjQ1MC4wNjk2MTE0NzE2MjEwNH1d" data-look="classic"/><path d="M336.984,404.684L331.553,408.776C326.123,412.867,315.261,421.05,304.4,429.232C293.538,437.415,282.677,445.598,277.246,449.689L271.815,453.781" id="my-svg-edge_5_8" class="edge-thickness-normal edge-pattern-solid edge section-edge-1 edge-depth-3" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_5_8" data-points="W3sieCI6MzM2Ljk4NDA2NzM0MTc5NDQsInkiOjQwNC42ODQxODY4Mjk1ODEzNH0seyJ4IjozMDQuMzk5Njg2ODIxMjYyNiwieSI6NDI5LjIzMjQzNDczMDAwMTl9LHsieCI6MjcxLjgxNTMwNjMwMDczMDgsInkiOjQ1My43ODA2ODI2MzA0MjI0Nn1d" data-look="classic"/><path d="M333.99,394.792L317.826,393.858C301.662,392.923,269.334,391.054,237.006,389.185C204.678,387.315,172.35,385.446,156.186,384.512L140.022,383.577" id="my-svg-edge_5_9" class="edge-thickness-normal edge-pattern-solid edge section-edge-1 edge-depth-3" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_5_9" data-points="W3sieCI6MzMzLjk4OTY0NTIxOTE3MTksInkiOjM5NC43OTI0NTAxOTMyNTg4NH0seyJ4IjoyMzcuMDA1NzUzODI2NDY0ODUsInkiOjM4OS4xODQ2NTk4MzA0MDI4fSx7IngiOjE0MC4wMjE4NjI0MzM3NTc4LCJ5IjozODMuNTc2ODY5NDY3NTQ2N31d" data-look="classic"/><path d="M484.399,253.573L476.966,243.456C469.533,233.34,454.667,213.107,439.8,192.875C424.934,172.642,410.068,152.409,402.634,142.293L395.201,132.177" id="my-svg-edge_0_10" class="edge-thickness-normal edge-pattern-solid edge section-edge-2 edge-depth-1" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_0_10" data-points="W3sieCI6NDg0LjM5OTQ2MTg2ODI5NTIsInkiOjI1My41NzI3NTMwMzA4MTg4Nn0seyJ4Ijo0MzkuODAwMzQxMzkyNjI2OCwieSI6MTkyLjg3NDY0OTg0NDg5ODF9LHsieCI6Mzk1LjIwMTIyMDkxNjk1ODQ1LCJ5IjoxMzIuMTc2NTQ2NjU4OTc3MzR9XQ==" data-look="classic"/><path d="M371.546,117.491L358.629,115.221C345.712,112.95,319.878,108.408,294.044,103.866C268.211,99.324,242.377,94.783,229.46,92.512L216.543,90.241" id="my-svg-edge_10_11" class="edge-thickness-normal edge-pattern-solid edge section-edge-2 edge-depth-3" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_10_11" data-points="W3sieCI6MzcxLjU0NjA1MzY5OTg2NjU1LCJ5IjoxMTcuNDkxNDc0MDc5MDk0MDZ9LHsieCI6Mjk0LjA0NDQzMzI5NTI4MzYsInkiOjEwMy44NjYwOTI1MzUyOTUwMn0seyJ4IjoyMTYuNTQyODEyODkwNzAwNywieSI6OTAuMjQwNzEwOTkxNDk1OTl9XQ==" data-look="classic"/><path d="M384.218,105.237L383.53,100.371C382.842,95.506,381.465,85.775,380.089,76.044C378.712,66.314,377.336,56.583,376.647,51.717L375.959,46.852" id="my-svg-edge_10_12" class="edge-thickness-normal edge-pattern-solid edge section-edge-2 edge-depth-3" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_10_12" data-points="W3sieCI6Mzg0LjIxODQzMDgxNjQwNzY1LCJ5IjoxMDUuMjM2NjMyMDA0NjQ3Mjl9LHsieCI6MzgwLjA4ODc2MTQzODM1MDE2LCJ5Ijo3Ni4wNDQzNzgwODQxMjYxfSx7IngiOjM3NS45NTkwOTIwNjAyOTI3LCJ5Ijo0Ni44NTIxMjQxNjM2MDQ5fV0=" data-look="classic"/><path d="M373.844,128.417L367.923,132.369C362.003,136.321,350.163,144.225,338.322,152.128C326.482,160.032,314.641,167.936,308.721,171.888L302.801,175.84" id="my-svg-edge_10_13" class="edge-thickness-normal edge-pattern-solid edge section-edge-2 edge-depth-3" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_10_13" data-points="W3sieCI6MzczLjg0MzcwOTE2ODQxNjQ3LCJ5IjoxMjguNDE2NzI5NTg0NzMzODR9LHsieCI6MzM4LjMyMjIwMjAyODc5ODM2LCJ5IjoxNTIuMTI4NDY0MTM2NDI0ODR9LHsieCI6MzAyLjgwMDY5NDg4OTE4MDI1LCJ5IjoxNzUuODQwMTk4Njg4MTE1ODN9XQ==" data-look="classic"/><path d="M401.018,117.097L414.571,114.339C428.124,111.581,455.23,106.065,482.336,100.549C509.442,95.032,536.548,89.516,550.101,86.758L563.654,84" id="my-svg-edge_10_14" class="edge-thickness-normal edge-pattern-solid edge section-edge-2 edge-depth-3" style="undefined;;;undefined" data-edge="true" data-et="edge" data-id="edge_10_14" data-points="W3sieCI6NDAxLjAxODE5MzM5MDk3NzEsInkiOjExNy4wOTc0NjQ1MTYxMDcyMX0seyJ4Ijo0ODIuMzM2MTM5MDYwNDc3NTQsInkiOjEwMC41NDg2OTAwNjIyNjA2Mn0seyJ4Ijo1NjMuNjU0MDg0NzI5OTc4LCJ5Ijo4My45OTk5MTU2MDg0MTQwM31d" data-look="classic"/></g><g class="edgeLabels"><g class="edgeLabel"><g class="label" data-id="edge_0_1" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_1_2" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_1_3" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_1_4" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_0_5" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_5_6" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_5_7" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_5_8" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_5_9" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_0_10" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_10_11" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_10_12" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_10_13" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g><g class="edgeLabel"><g class="label" data-id="edge_10_14" transform="translate(0, 0)"><foreignObject width="0" height="0"><div xmlns="http://www.w3.org/1999/xhtml" class="labelBkg" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="edgeLabel"></span></div></foreignObject></g></g></g><g class="nodes"><g class="node mindmap-node section-root section--1" id="my-svg-node_0" data-look="classic" transform="translate(493.2812027478939, 265.660543521544)"><circle class="basic label-container" style="" r="83.72534057083193" cx="0" cy="0"/><g class="label" style="" transform="translate(-72.7421875, -12)"><rect/><foreignObject width="145.484375" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Integrales Impropias</p></span></div></foreignObject></g></g><g class="node mindmap-node section-0" id="my-svg-node_1" data-look="classic" transform="translate(671.4923821882938, 289.9093870900192)"><path id="my-svg-node_1" class="node-bkg node-0" style="" d="M-38.5859375 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h67.171875&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-67.171875&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-38.5859375" y1="17" x2="38.5859375" y2="17"/><g class="label" style="" transform="translate(-18.5859375, -12)"><rect/><foreignObject width="37.171875" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Tipos</p></span></div></foreignObject></g></g><g class="node mindmap-node section-0" id="my-svg-node_2" data-look="classic" transform="translate(868.0637637028484, 315.1652668899321)"><path id="my-svg-node_2" class="node-bkg node-0" style="" d="M-103.015625 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h196.03125&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-196.03125&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-103.015625" y1="17" x2="103.015625" y2="17"/><g class="label" style="" transform="translate(-83.015625, -12)"><rect/><foreignObject width="166.03125" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Tipo I: Límites infinitos</p></span></div></foreignObject></g></g><g class="node mindmap-node section-0" id="my-svg-node_3" data-look="classic" transform="translate(691.615562590851, 376.8145972617234)"><path id="my-svg-node_3" class="node-bkg node-0" style="" d="M-107.8046875 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h205.609375&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-205.609375&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-107.8046875" y1="17" x2="107.8046875" y2="17"/><g class="label" style="" transform="translate(-87.8046875, -12)"><rect/><foreignObject width="175.609375" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Tipo II: Discontinuidades</p></span></div></foreignObject></g></g><g class="node mindmap-node section-0" id="my-svg-node_4" data-look="classic" transform="translate(751.4469605044384, 219.98120427380354)"><path id="my-svg-node_4" class="node-bkg node-0" style="" d="M-106.78125 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h203.5625&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-203.5625&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-106.78125" y1="17" x2="106.78125" y2="17"/><g class="label" style="" transform="translate(-86.78125, -12)"><rect/><foreignObject width="173.5625" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Tipo Mixto: Ambos casos</p></span></div></foreignObject></g></g><g class="node mindmap-node section-1" id="my-svg-node_5" data-look="classic" transform="translate(348.9646326529297, 395.6583320320776)"><path id="my-svg-node_5" class="node-bkg node-0" style="" d="M-58.25 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h106.5&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-106.5&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-58.25" y1="17" x2="58.25" y2="17"/><g class="label" style="" transform="translate(-38.25, -12)"><rect/><foreignObject width="76.5" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Evaluación</p></span></div></foreignObject></g></g><g class="node mindmap-node section-1" id="my-svg-node_6" data-look="classic" transform="translate(287.6607214543993, 319.97229065853594)"><path id="my-svg-node_6" class="node-bkg node-0" style="" d="M-46.03125 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h82.0625&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-82.0625&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-46.03125" y1="17" x2="46.03125" y2="17"/><g class="label" style="" transform="translate(-26.03125, -12)"><rect/><foreignObject width="52.0625" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Límites</p></span></div></foreignObject></g></g><g class="node mindmap-node section-1" id="my-svg-node_7" data-look="classic" transform="translate(454.79295209891177, 457.6513762054211)"><path id="my-svg-node_7" class="node-bkg node-0" style="" d="M-68.0390625 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h126.078125&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-126.078125&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-68.0390625" y1="17" x2="68.0390625" y2="17"/><g class="label" style="" transform="translate(-48.0390625, -12)"><rect/><foreignObject width="96.078125" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Convergencia</p></span></div></foreignObject></g></g><g class="node mindmap-node section-1" id="my-svg-node_8" data-look="classic" transform="translate(259.8347409895955, 462.8065374279262)"><path id="my-svg-node_8" class="node-bkg node-0" style="" d="M-61.7734375 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h113.546875&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-113.546875&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-61.7734375" y1="17" x2="61.7734375" y2="17"/><g class="label" style="" transform="translate(-41.7734375, -12)"><rect/><foreignObject width="83.546875" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Divergencia</p></span></div></foreignObject></g></g><g class="node mindmap-node section-1" id="my-svg-node_9" data-look="classic" transform="translate(125.046875, 382.71098762872793)"><path id="my-svg-node_9" class="node-bkg node-0" style="" d="M-110.046875 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h210.09375&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-210.09375&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-110.046875" y1="17" x2="110.046875" y2="17"/><g class="label" style="" transform="translate(-90.046875, -12)"><rect/><foreignObject width="180.09375" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Criterios de comparación</p></span></div></foreignObject></g></g><g class="node mindmap-node section-2" id="my-svg-node_10" data-look="classic" transform="translate(386.31948003735977, 120.08875616825219)"><path id="my-svg-node_10" class="node-bkg node-0" style="" d="M-64.4921875 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h118.984375&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-118.984375&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-64.4921875" y1="17" x2="64.4921875" y2="17"/><g class="label" style="" transform="translate(-44.4921875, -12)"><rect/><foreignObject width="88.984375" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Aplicaciones</p></span></div></foreignObject></g></g><g class="node mindmap-node section-2" id="my-svg-node_11" data-look="classic" transform="translate(201.76938655320748, 87.64342890233786)"><path id="my-svg-node_11" class="node-bkg node-0" style="" d="M-64.6484375 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h119.296875&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-119.296875&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-64.6484375" y1="17" x2="64.6484375" y2="17"/><g class="label" style="" transform="translate(-44.6484375, -12)"><rect/><foreignObject width="89.296875" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Probabilidad</p></span></div></foreignObject></g></g><g class="node mindmap-node section-2" id="my-svg-node_12" data-look="classic" transform="translate(373.85804283934056, 32)"><path id="my-svg-node_12" class="node-bkg node-0" style="" d="M-71.7890625 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h133.578125&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-133.578125&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-71.7890625" y1="17" x2="71.7890625" y2="17"/><g class="label" style="" transform="translate(-51.7890625, -12)"><rect/><foreignObject width="103.578125" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Transformadas</p></span></div></foreignObject></g></g><g class="node mindmap-node section-2" id="my-svg-node_13" data-look="classic" transform="translate(290.32492402023695, 184.1681721045975)"><path id="my-svg-node_13" class="node-bkg node-0" style="" d="M-85.4140625 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h160.828125&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-160.828125&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-85.4140625" y1="17" x2="85.4140625" y2="17"/><g class="label" style="" transform="translate(-65.4140625, -12)"><rect/><foreignObject width="130.828125" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Física matemática</p></span></div></foreignObject></g></g><g class="node mindmap-node section-2" id="my-svg-node_14" data-look="classic" transform="translate(578.3527980835953, 81.00862395626905)"><path id="my-svg-node_14" class="node-bkg node-0" style="" d="M-72.7734375 12&#10;    v-24&#10;    q0,-5 5,-5&#10;    h135.546875&#10;    q5,0 5,5&#10;    v24&#10;    q0,5 -5,5&#10;    h-135.546875&#10;    q-5,0 -5,-5&#10;    Z"/><line class="node-line-" x1="-72.7734375" y1="17" x2="72.7734375" y2="17"/><g class="label" style="" transform="translate(-52.7734375, -12)"><rect/><foreignObject width="105.546875" height="24"><div xmlns="http://www.w3.org/1999/xhtml" style="display: table-cell; white-space: nowrap; line-height: 1.5; max-width: 200px; text-align: center;"><span class="nodeLabel markdown-node-label"><p>Series infinitas</p></span></div></foreignObject></g></g></g></g><defs><filter id="my-svg-drop-shadow" height="130%" width="130%"><feDropShadow dx="4" dy="4" stdDeviation="0" flood-opacity="0.06" flood-color="#000000"/></filter></defs><defs><filter id="my-svg-drop-shadow-small" height="150%" width="150%"><feDropShadow dx="2" dy="2" stdDeviation="0" flood-opacity="0.06" flood-color="#000000"/></filter></defs></svg>

---

## 📝 Clasificación de Integrales Impropias

> [!note] 🔍 **Definición Formal**
> Una integral $\int_a^b f(x) dx$ es **impropia** si:
> 1. Uno o ambos límites de integración son infinitos
> 2. La función $f(x)$ tiene discontinuidades infinitas en $[a,b]$
> 3. Ambas condiciones se presentan simultáneamente

### Tipo I: Límites de Integración Infinitos

> [!tip] 📊 **Definiciones del Tipo I**
> 
> **Caso 1**: Límite superior infinito
> $$\int_a^{\infty} f(x) dx = \lim_{t \to \infty} \int_a^t f(x) dx$$
> 
> **Caso 2**: Límite inferior infinito
> $$\int_{-\infty}^b f(x) dx = \lim_{t \to -\infty} \int_t^b f(x) dx$$
> 
> **Caso 3**: Ambos límites infinitos
> $$\int_{-\infty}^{\infty} f(x) dx = \int_{-\infty}^c f(x) dx + \int_c^{\infty} f(x) dx$$
> donde $c$ es cualquier número real, y **ambas integrales deben converger**.
>

> [!example] 🧪 **Ejemplo Tipo I - Convergente**
> **Evaluar**: $\int_1^{\infty} \frac{1}{x^2} dx$
> 
> **Solución**:
> $$\int_1^{\infty} \frac{1}{x^2} dx = \lim_{t \to \infty} \int_1^t x^{-2} dx$$
> $$= \lim_{t \to \infty} \left[-x^{-1}\right]_1^t$$
> $$= \lim_{t \to \infty} \left(-\frac{1}{t} + 1\right)$$
> $$= 0 + 1 = 1$$
> 
> **Conclusión**: La integral **converge** a 1.
>

> [!example] 🧪 **Ejemplo Tipo I - Divergente**
> **Evaluar**: $\int_1^{\infty} \frac{1}{x} dx$
> 
> **Solución**:
> $$\int_1^{\infty} \frac{1}{x} dx = \lim_{t \to \infty} \int_1^t x^{-1} dx$$
> $$= \lim_{t \to \infty} [\ln x]_1^t$$
> $$= \lim_{t \to \infty} (\ln t - \ln 1)$$
> $$= \lim_{t \to \infty} \ln t = \infty$$
> 
> **Conclusión**: La integral **diverge**.

### Tipo II: Discontinuidades Infinitas

> [!tip] 📊 **Definiciones del Tipo II**
> 
> **Caso 1**: Discontinuidad en el límite inferior
> Si $f(x)$ tiene discontinuidad infinita en $x = a$:
> $$\int_a^b f(x) dx = \lim_{t \to a^+} \int_t^b f(x) dx$$
> 
> **Caso 2**: Discontinuidad en el límite superior
> Si $f(x)$ tiene discontinuidad infinita en $x = b$:
> $$\int_a^b f(x) dx = \lim_{t \to b^-} \int_a^t f(x) dx$$
> 
> **Caso 3**: Discontinuidad interior
> Si $f(x)$ tiene discontinuidad infinita en $x = c$ donde $a < c < b$:
> $$\int_a^b f(x) dx = \int_a^c f(x) dx + \int_c^b f(x) dx$$
> donde **ambas integrales deben converger**.
>

> [!example] 🧪 **Ejemplo Tipo II - Convergente**
> **Evaluar**: $\int_0^1 \frac{1}{\sqrt{x}} dx$
> 
> **Análisis**: $f(x) = x^{-1/2}$ tiene discontinuidad infinita en $x = 0$
> 
> **Solución**:
> $$\int_0^1 x^{-1/2} dx = \lim_{t \to 0^+} \int_t^1 x^{-1/2} dx$$
> $$= \lim_{t \to 0^+} [2x^{1/2}]_t^1$$
> $$= \lim_{t \to 0^+} (2\sqrt{1} - 2\sqrt{t})$$
> $$= 2 - 0 = 2$$
> 
> **Conclusión**: La integral **converge** a 2.
>

> [!example] 🧪 **Ejemplo Tipo II - Divergente**
> **Evaluar**: $\int_0^1 \frac{1}{x} dx$
> 
> **Análisis**: $f(x) = x^{-1}$ tiene discontinuidad infinita en $x = 0$
> 
> **Solución**:
> $$\int_0^1 x^{-1} dx = \lim_{t \to 0^+} \int_t^1 x^{-1} dx$$
> $$= \lim_{t \to 0^+} [\ln x]_t^1$$
> $$= \lim_{t \to 0^+} (\ln 1 - \ln t)$$
> $$= \lim_{t \to 0^+} (-\ln t) = \infty$$
> 
> **Conclusión**: La integral **diverge**.

### Tipo Mixto: Combinación de Ambos Casos

> [!warning] ⚠️ **Integrales Mixtas**
> Cuando una integral tiene **tanto límites infinitos como discontinuidades**, debe separarse en partes donde cada una tenga solo un tipo de impropiedad.
> 
> **Ejemplo**: $\int_0^{\infty} \frac{1}{\sqrt{x}} dx$
> - Discontinuidad en $x = 0$ (Tipo II)
> - Límite superior infinito (Tipo I)
> 
> **Separación**: $\int_0^{\infty} \frac{1}{\sqrt{x}} dx = \int_0^1 \frac{1}{\sqrt{x}} dx + \int_1^{\infty} \frac{1}{\sqrt{x}} dx$

---

## 🧠 Mnemotecnia para el Estudio Eficaz

> [!success] 🎭 **Método Mnemotécnico: "LÍMITE"**
> 
> Para recordar el proceso de evaluación de integrales impropias:
> 
> **L** - **Localiza** el problema (¿infinito o discontinuidad?)
> **Í** - **Identifica** el tipo (I, II, o mixto)
> **M** - **Modifica** la integral usando límites apropiados
> **I** - **Integra** la función (encuentra la antiderivada)
> **T** - **Toma** el límite hacia el valor problemático
> **E** - **Evalúa** si converge o diverge
>

> [!tip] 💡 **Reglas Nemotécnicas Rápidas**
> 
> **Para $\int_1^{\infty} \frac{1}{x^p} dx$**:
> - "**P**equeño **p** (p ≤ 1)**: **D**iverge"
> - "**G**rande **p** (p > 1)**: **C**onverge"
> 
> **Para $\int_0^1 \frac{1}{x^p} dx$**:
> - "**P**equeño **p** (p < 1)**: **C**onverge"
> - "**G**rande **p** (p ≥ 1)**: **D**iverge"
> 
> **Frase mnemotécnica**: "En infinito, **p** grande converge; en cero, **p** pequeño converge"

---

## 🔍 Criterios de Convergencia

### Criterio de Comparación Directa

> [!info] 📋 **Teorema de Comparación Directa**
> Sean $f(x)$ y $g(x)$ funciones tales que $0 \leq f(x) \leq g(x)$ para $x \geq a$.
> 
> **Para integrales del Tipo I**:
> - Si $\int_a^{\infty} g(x) dx$ **converge**, entonces $\int_a^{\infty} f(x) dx$ **converge**
> - Si $\int_a^{\infty} f(x) dx$ **diverge**, entonces $\int_a^{\infty} g(x) dx$ **diverge**
>

> [!example] 🧪 **Ejemplo de Comparación Directa**
> **Evaluar**: $\int_1^{\infty} \frac{1}{x^2 + 1} dx$
> 
> **Comparación**: Para $x \geq 1$, tenemos $x^2 + 1 \geq x^2$, por lo tanto:
> $$\frac{1}{x^2 + 1} \leq \frac{1}{x^2}$$
> 
> Como $\int_1^{\infty} \frac{1}{x^2} dx = 1$ (converge), entonces $\int_1^{\infty} \frac{1}{x^2 + 1} dx$ **converge**.

### Criterio de Comparación Límite

> [!info] 📋 **Teorema de Comparación Límite**
> Sean $f(x)$ y $g(x)$ funciones positivas. Si:
> $$\lim_{x \to \infty} \frac{f(x)}{g(x)} = L$$
> donde $0 < L < \infty$, entonces $\int_a^{\infty} f(x) dx$ y $\int_a^{\infty} g(x) dx$ tienen el **mismo comportamiento de convergencia**.
>

> [!example] 🧪 **Ejemplo de Comparación Límite**
> **Evaluar**: $\int_1^{\infty} \frac{2x + 1}{x^3 - x + 1} dx$
> 
> **Comparación**: Para $x$ grande, el comportamiento está dominado por los términos de mayor grado:
> $$\lim_{x \to \infty} \frac{\frac{2x + 1}{x^3 - x + 1}}{\frac{2x}{x^3}} = \lim_{x \to \infty} \frac{\frac{2x + 1}{x^3 - x + 1}}{\frac{2}{x^2}} = 1$$
> 
> Como $\int_1^{\infty} \frac{2}{x^2} dx$ converge, entonces la integral original **converge**.

---

## 🎯 Integrales Importantes y Patrones

### Integrales de Referencia Tipo I

> [!tip] 📊 **Tabla de Integrales de Referencia - Tipo I**
> 
> | Integral | Convergencia | Valor (si converge) | Condición |
> |----------|--------------|-------------------|-----------|
> | $\int_1^{\infty} \frac{1}{x^p} dx$ | $p > 1$ | $\frac{1}{p-1}$ | $p > 1$ |
> | $\int_1^{\infty} \frac{1}{x^p} dx$ | Diverge | - | $p \leq 1$ |
> | $\int_1^{\infty} \frac{1}{x(\ln x)^p} dx$ | $p > 1$ | $\frac{1}{p-1}$ | $p > 1$ |
> | $\int_1^{\infty} e^{-ax} dx$ | Converge | $\frac{1}{a}$ | $a > 0$ |
> | $\int_0^{\infty} e^{-ax^2} dx$ | Converge | $\frac{1}{2}\sqrt{\frac{\pi}{a}}$ | $a > 0$ |

### Integrales de Referencia Tipo II

> [!tip] 📊 **Tabla de Integrales de Referencia - Tipo II**
> 
> | Integral | Convergencia | Valor (si converge) | Condición |
> |----------|--------------|-------------------|-----------|
> | $\int_0^1 \frac{1}{x^p} dx$ | $p < 1$ | $\frac{1}{1-p}$ | $p < 1$ |
> | $\int_0^1 \frac{1}{x^p} dx$ | Diverge | - | $p \geq 1$ |
> | $\int_0^1 x^p dx$ | Converge | $\frac{1}{p+1}$ | $p > -1$ |
> | $\int_0^1 \frac{1}{x^p (\ln x)^q} dx$ | Complejo | - | Depende de $p$ y $q$ |

---

## 💡 Ejemplos Desarrollados

> [!example] 🎯 **Ejemplo 1: Integral Tipo I con parámetro**
> **Evaluar**: $\int_0^{\infty} xe^{-ax} dx$ donde $a > 0$
> 
> **Solución usando integración por partes**:
> Sea $u = x$, $dv = e^{-ax} dx$
> Entonces $du = dx$, $v = -\frac{1}{a}e^{-ax}$
> 
> $$\int_0^{\infty} xe^{-ax} dx = \lim_{t \to \infty} \int_0^t xe^{-ax} dx$$
> $$= \lim_{t \to \infty} \left[-\frac{x}{a}e^{-ax} + \frac{1}{a}\int e^{-ax} dx\right]_0^t$$
> $$= \lim_{t \to \infty} \left[-\frac{x}{a}e^{-ax} - \frac{1}{a^2}e^{-ax}\right]_0^t$$
> $$= \lim_{t \to \infty} \left(-\frac{t}{a}e^{-at} - \frac{1}{a^2}e^{-at} + \frac{1}{a^2}\right)$$
> 
> Como $\lim_{t \to \infty} te^{-at} = 0$ y $\lim_{t \to \infty} e^{-at} = 0$ (para $a > 0$):
> $$= 0 - 0 + \frac{1}{a^2} = \frac{1}{a^2}$$
>

> [!example] 🎯 **Ejemplo 2: Integral Tipo II**
> **Evaluar**: $\int_0^4 \frac{1}{\sqrt{4-x}} dx$
> 
> **Análisis**: Discontinuidad en $x = 4$
> 
> **Solución**:
> $$\int_0^4 \frac{1}{\sqrt{4-x}} dx = \lim_{t \to 4^-} \int_0^t (4-x)^{-1/2} dx$$
> 
> Sea $u = 4-x$, entonces $du = -dx$:
> $$= \lim_{t \to 4^-} \int_{4}^{4-t} u^{-1/2} (-du) = \lim_{t \to 4^-} \int_{4-t}^{4} u^{-1/2} du$$
> $$= \lim_{t \to 4^-} [2u^{1/2}]_{4-t}^{4}$$
> $$= \lim_{t \to 4^-} (2\sqrt{4} - 2\sqrt{4-t})$$
> $$= 4 - 0 = 4$$
>

> [!example] 🎯 **Ejemplo 3: Integral Mixta**
> **Evaluar**: $\int_0^{\infty} \frac{1}{\sqrt{x}(1+x)} dx$
> 
> **Análisis**: Discontinuidad en $x = 0$ y límite superior infinito
> 
> **Separación**: $\int_0^{\infty} \frac{1}{\sqrt{x}(1+x)} dx = \int_0^1 \frac{1}{\sqrt{x}(1+x)} dx + \int_1^{\infty} \frac{1}{\sqrt{x}(1+x)} dx$
> 
> **Evaluación de cada parte**:
> 
> **Parte 1** ($\int_0^1$): Tipo II
> Para $x$ cerca de 0: $\frac{1}{\sqrt{x}(1+x)} \sim \frac{1}{\sqrt{x}}$
> Como $\int_0^1 \frac{1}{\sqrt{x}} dx$ converge, esta parte converge.
> 
> **Parte 2** ($\int_1^{\infty}$): Tipo I
> Para $x$ grande: $\frac{1}{\sqrt{x}(1+x)} \sim \frac{1}{x^{3/2}}$
> Como $\int_1^{\infty} \frac{1}{x^{3/2}} dx$ converge (p = 3/2 > 1), esta parte converge.
> 
> **Conclusión**: Ambas partes convergen, por lo tanto la integral original converge.

---

## 🔗 Aplicaciones Prácticas

> [!note] 🌐 **Aplicaciones en Probabilidad**
> **Distribuciones de Probabilidad Continuas**:
> - **Distribución Exponencial**: $f(x) = \lambda e^{-\lambda x}$ para $x \geq 0$
>   $$\int_0^{\infty} \lambda e^{-\lambda x} dx = 1$$
> - **Distribución Normal**: $f(x) = \frac{1}{\sigma\sqrt{2\pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}$
>   $$\int_{-\infty}^{\infty} f(x) dx = 1$$
>

> [!note] 🔬 **Aplicaciones en Física**
> **Transformadas de Laplace**:
> $$\mathcal{L}\{f(t)\} = \int_0^{\infty} f(t) e^{-st} dt$$
> 
> **Energía de una partícula**:
> $$E = \int_0^{\infty} \frac{1}{2}mv^2 \rho(v) dv$$
> donde $\rho(v)$ es la distribución de velocidades.
>

> [!note] 🎵 **Aplicaciones en Análisis de Fourier**
> **Transformada de Fourier**:
> $$\hat{f}(\omega) = \int_{-\infty}^{\infty} f(t) e^{-i\omega t} dt$$
> 
> **Condición de convergencia**: $\int_{-\infty}^{\infty} \lvert f(t) \rvert dt < \infty$

---

## 🧠 Estrategias de Resolución

> [!tip] 💡 **Estrategia General**
> **Paso 1**: **Identificar** el tipo de impropiedad
> - ¿Límites infinitos? → Tipo I
> - ¿Discontinuidades? → Tipo II
> - ¿Ambos? → Mixto
> 
> **Paso 2**: **Localizar** puntos problemáticos
> - Para Tipo I: donde los límites son $\pm\infty$
> - Para Tipo II: donde $f(x) \to \pm\infty$
> 
> **Paso 3**: **Separar** si hay múltiples problemas
> - Una integral por cada punto problemático
> 
> **Paso 4**: **Formar** los límites apropiados
> - Reemplazar cada problema con una variable que tiende al valor problemático
> 
> **Paso 5**: **Evaluar** usando técnicas estándar
> - Antiderivadas, integración por partes, sustitución, etc.
> 
> **Paso 6**: **Calcular** los límites
> - Determinar si existen (convergencia) o no (divergencia)
>

> [!warning] ⚠️ **Errores Comunes y Cómo Evitarlos**
> 
> **Error 1**: No identificar todas las impropiedades
> - ✅ **Solución**: Examinar cuidadosamente tanto los límites como la función
> 
> **Error 2**: No separar correctamente las integrales mixtas
> - ✅ **Solución**: Cada punto problemático requiere su propio límite
> 
> **Error 3**: Evaluar incorrectamente los límites
> - ✅ **Solución**: Usar formas indeterminadas y regla de L'Hôpital cuando sea necesario
> 
> **Error 4**: Confundir convergencia con el valor de la integral
> - ✅ **Solución**: Recordar que convergencia significa que el límite existe y es finito
> 
> **Error 5**: No verificar las condiciones de los criterios de comparación
> - ✅ **Solución**: Asegurar que las funciones sean positivas y que la comparación sea válida

---
## 📚 Referencias

> [!quote] 📖 Notas relacionadas
> 
>
> - [[Universidad/1er Semestre/Cálculo de una Variable/Unidad 05 - Integrales/I - Fundamentos Teóricos/01 - Integral de Riemann\|01 - Integral de Riemann]] - Fundamento teórico de las integrales definidas
> - [[Universidad/1er Semestre/Cálculo de una Variable/Unidad 05 - Integrales/I - Fundamentos Teóricos/02 - Propiedades de la Integral\|02 - Propiedades de la Integral]] - Propiedades fundamentales de integración
> - [[Universidad/1er Semestre/Cálculo de una Variable/Unidad 05 - Integrales/I - Fundamentos Teóricos/04 - Teorema Fundamental del Cálculo\|04 - Teorema Fundamental del Cálculo]] - Marco teórico principal
> - [[Universidad/1er Semestre/Cálculo de una Variable/Unidad 05 - Integrales/IV - Integrales Impropias y Avanzadas/03 - Teoremas de Comparación y Desigualdades\|03 - Teoremas de Comparación y Desigualdades]] - Criterios de convergencia

---

## 🔍 Notas Recomendadas

> [!info] 📚 Para profundizar y complementar
> - [[Universidad/1er Semestre/Cálculo de una Variable/Unidad 06 – Aplicaciones de la Integral/I - Áreas/01 - Área bajo la Curva\|01 - Área bajo la Curva]] - Base conceptual de integrales definidas
> - [[Universidad/1er Semestre/Cálculo de una Variable/Unidad 05 - Integrales/III - Integrales Definidas/01 - Métodos de Integración Definida\|01 - Métodos de Integración Definida]] - Técnicas avanzadas de integración
> - [[Universidad/1er Semestre/Cálculo de una Variable/Unidad 05 - Integrales/V - Otras Técnicas/01 - Integración Numérica\|01 - Integración Numérica]] - Métodos computacionales
> - [[Universidad/1er Semestre/Cálculo de una Variable/Unidad 05 - Integrales/III - Integrales Definidas/03 - Teoremas Especiales para Integrales Definidas\|03 - Teoremas Especiales para Integrales Definidas]] - Técnicas especiales de evaluación
> - [[Universidad/1er Semestre/Cálculo de una Variable/Unidad 05 - Integrales/III - Integrales Definidas/03 - Teoremas Especiales para Integrales Definidas\|03 - Teoremas Especiales para Integrales Definidas]] - Teoremas fundamentales del cálculo

## 🏷️ Tags

#matemáticas #cálculo #integrales-impropias #convergencia #divergencia #límites #integración #análisis-matemático #universidad #probabilidad #transformadas #física-matemática #criterios-comparación #mnemotecnia #métodos-estudio