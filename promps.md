# Historial de Prompts – Parcial Desarrollo Web

Archivo de promps a chatgptpara recrear la imagen

A partir de una imagen de referencia, genera la estructura HTML semántica
para un componente de interfaz puramente visual (sin interacción ni lógica).
El diseño representa un panel rectangular con figuras geométricas repetidas
(cuadrados y círculos) distribuidas en sus extremos, siguiendo un patrón
simétrico horizontal y vertical.
Crea un contenedor principal que luego será centrado en el viewport.
Dentro de él, define una estructura clara que permita ubicar **pares de elementos**
en las esquinas del contenedor, **priorizando la reutilización de nodos y clases**.
Utiliza clases reutilizables y nombres descriptivos.
No incluyas estilos CSS ni posicionamiento, solo HTML bien estructurado
y correctamente anidado.

### Prompt 2 – Estilos base y normalización visual

Crea el código de una hoja de estilos CSS que defina la apariencia base del componente.
Configura el contenedor principal con dimensiones fijas (400px por 300px)
y un color de fondo azul oscuro.
Define estilos comunes para las figuras geométricas, asegurando consistencia
en tamaños y proporciones.
Los cuadrados deben ser color celeste y los círculos rosados, utilizando
border-radius: 50% para estos últimos.
Aplica el box model de forma explícita y mantén baja la especificidad
de los selectores.
No resuelvas aún la distribución espacial final.

### Prompt 3 – Layout y refinamiento con Flexbox

Implementa el layout final utilizando Flexbox.
Centra el contenedor principal tanto vertical como horizontalmente
dentro del viewport.
Distribuye las figuras geométricas de forma simétrica en las cuatro esquinas
del contenedor, respetando el patrón visual observado en la imagen.
Utiliza flexbox anidado si es necesario y propiedades como
justify-content, align-items y gap.
Evita completamente el uso de position absolute o floats.
Prioriza un layout claro, legible y fácil de mantener.

:)

