# Three.js – Shaders, Partículas y Post‑Procesado

Este repositorio contiene una colección de ejemplos prácticos desarrollados con [Three.js](https://threejs.org/) que exploran tres áreas fundamentales de la gráfica 3D en tiempo real: **shaders personalizados (vertex/fragment)**, **sistemas de partículas** y **efectos de post‑procesado**. El proyecto está estructurado en tres módulos independientes, cada uno con sus propias demostraciones.

## Módulo 1 Vertex y fragment
Este módulo contiene tres ejercicios que demuestran el uso de shaders GLSL para manipular geometría y aplicar iluminación no estándar.

### Slime sinusoidal
Un objeto con forma de slime (geometría esférica deformada) cuyo tamaño y forma oscilan siguiendo una función sinusoidal. El vértice se desplaza a lo largo de la normal dependiendo del tiempo, creando un efecto orgánico.

<img width="480" height="270" alt="Image" src="https://github.com/user-attachments/assets/a752e686-317d-47a9-ae79-3bee5395f112" />

### Esfera con iluminación Blinn‑Phong
Implementación del modelo de iluminación Blinn‑Phong c. La esfera reacciona a una fuente de luz direccional, mostrando reflejos especulares y difusos calculados manualmente en el fragment shader.

<img width="480" height="270" alt="Image" src="https://github.com/user-attachments/assets/bf95ea29-8265-4120-acb4-a7ea15f054a2" />

### Toon shading sobre una superficie
Aplicación de sombreado tipo “cel shading” sobre una superficie. Los colores se cuantifican en bandas discretas para lograr el efecto cartoon, y se añaden bordes de silueta mediante el uso de normales.

<img width="480" height="270" alt="Image" src="https://github.com/user-attachments/assets/32fe5bb7-912a-4ac3-9966-0161a650995d" />

## Sistemas de partículas
Dos ejemplos que explotan THREE.Points y THREE.BufferGeometry para simular comportamientos dinámicos con miles de partículas.

### Humo
Simulación de una columna de humo que se eleva y se dispersa. Cada partícula tiene posición, velocidad, tamaño y opacidad variables, generando un efecto realista.

<img width="480" height="270" alt="Image" src="https://github.com/user-attachments/assets/345be6e4-f562-43d4-afcb-bf1abef648dc" />

### Rasengan (1 millón de partículas)
Representación del famoso jutsu del anime Naruto. Un billón (1 000 000) de partículas giratorias que forman una esfera compacta con un núcleo brillante. El alto rendimiento se logra mediante el uso de BufferAttribute y actualizaciones en el bucle de animación con operaciones eficientes.

<img width="480" height="270" alt="Image" src="https://github.com/user-attachments/assets/3900ff8b-991b-4850-9bfe-7f0e047df64c" />

## Post‑procesado
Un único ejemplo que muestra cómo aplicar efectos de post‑procesado a la escena completa utilizando el EffectComposer de Three.js.

Se aplica un filtro que incluye Desenfoque (blur)

<img width="480" height="270" alt="Image" src="https://github.com/user-attachments/assets/6bb2def3-2797-4e05-8980-ff7c57b957ef" />
