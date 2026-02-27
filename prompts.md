Prompt 1 
Genera SOLO el HTML para un componente UI. Requisitos:
- Usa etiquetas semánticas (main/section/div) y evita <br>.
- El componente principal debe ser un contenedor de 400x300 (lo estilizaré luego).
- Dentro, crea dos filas (superior e inferior) y en cada fila dos grupos (izquierda y derecha).
- Cada grupo contiene 2 elementos decorativos (figuras) representados con <span>.
- Agrega atributos accesibles: aria-label en el contenedor y aria-hidden en los spans decorativos.
No incluyas CSS todavía.
Prompt 2
Ahora genera style.css con estilos base:
- Aplica un reset mínimo (* { box-sizing: border-box } y body margin: 0).
- Define el contenedor principal con width: 400px; height: 300px; y un background azul similar a la referencia.
- Crea clases .shape, .shape--square, .shape--circle.
- Usa unidades en px para igualar el mockup, pero usa rem en padding general del viewport.
- Asegura que los círculos sean perfectos con border-radius: 50%.
Nota de especificidad: usa selectores de clase simples, evita IDs.
Prompt 3
Refina el layout para que coincida con la imagen:
- Centra el contenedor (400x300) vertical y horizontalmente en el viewport usando Grid (place-items: center) o Flex.
- Dentro del contenedor, usa Flexbox con flex-direction: column para tener fila superior e inferior separadas con justify-content: space-between.
- Cada fila debe usar display:flex y justify-content: space-between para separar el grupo izquierdo y derecho.
- Cada grupo debe usar display:flex y gap para separar las 2 figuras.
- La fila superior debe alinear al inicio (align-items: flex-start) y la inferior al final (align-items: flex-end).
Incluye comentarios breves en el CSS explicando flex-direction y justify-content.
