# Historial de Prompts – Parcial Desarrollo Web

Archivo de promps a chatgpt para recrear la imagen

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

hubo un problema con chat y continue en gemini estos son promps de gemini, también lo que hizo chat estaba mal y corrido.

### Prompt 1: Estructura Semántica

Genera la estructura HTML para un componente de interfaz. Necesito un contenedor principal (clase canvas) de 400x300px. Dentro, debe haber cuatro sub-contenedores (clase group) distribuidos en las esquinas. Cada grupo contendrá dos elementos div: uno para un cuadrado y otro para un círculo. Asegúrate de usar nombres de clases descriptivos para facilitar la especificidad en el CSS posterior.

### Prompt 2: Estilos Base y Modelo de Caja

Aplica estilos CSS a la estructura anterior. El canvas debe tener un fondo azul oscuro (#1919a6). Define el tamaño de los cuadrados y círculos usando unidades rem para que sean escalables. Los cuadrados son de color cian (#70d5e5) y los círculos rosa (#d4569e). Usa border-radius: 50% para transformar los div en círculos. Asegúrate de que el contenedor principal esté centrado en el viewport usando un layout de box-model estándar (margin auto).

### Prompt 3: Layout y Refinamiento (Flexbox)

Ahora, organiza el layout. El contenedor canvas debe usar display: flex con flex-wrap: wrap y justify-content: space-between para enviar los grupos a las esquinas. Para los grupos internos, usa display: flex y align-items: center.

Nota que en la imagen, el orden del círculo y el cuadrado cambia según la posición. Utiliza la pseudo-clase :nth-child o aplica una clase inversa para ambiar el flex-direction: row-reverse en los grupos de la derecha y los de abajo, logrando esa simetría visual exacta. El contenedor de 400x300px debe estar centrado verticalmente en la pantalla.

:)

