# Práctica 3 — El salón al atardecer

Módulo 3, Materiales e iluminación. Tiempo estimado: entre 3 y 5 horas. Necesitas: el modelo de Villa Alba de la práctica 2, con capas ordenadas.

## Objetivo

Al terminar sabrás asignar una paleta corta de materiales, colocar el sol según una orientación y una hora, añadir luz artificial cálida y generar una vista interior con la atmósfera de un atardecer. Aprenderás a juzgar la imagen por criterios concretos y no solo por si te gusta.

## Punto de partida

El modelo de la práctica 2 y los archivos de partida de Villa Alba (carpeta `curso/villa-alba/`), en especial `planta.svg`, como referencia de estancias y orientación: el norte está hacia arriba y el salón-comedor tiene su cristalera hacia el sur, sobre el porche. Si no modelaste mobiliario, añade al menos unos volúmenes simples en el salón.

## Pasos

1. Elige una paleta de entre cuatro y seis materiales: suelo interior, muros, carpintería, deck de madera, agua de la piscina y cubierta. Anótala en una lista con el color base de cada uno.
2. Crea cada material con su color, su rugosidad y su reflejo, y asígnalo por capas. Comprueba con una vista de prueba que ningún elemento queda con el material por defecto.
3. Aplica texturas a la madera y al suelo y ajusta su escala. Comprueba que una tabla de deck mide algo realista, entre 10 y 20 cm de ancho, y que la dirección de la veta es coherente.
4. Orienta el modelo con el norte correcto, de modo que la fachada principal mire al sur. Comprueba que el sol del mediodía queda hacia ese lado.
5. Coloca un sol bajo desde el suroeste, con una altura de unos 10 a 20 grados sobre el horizonte, y un cielo de atardecer. Comprueba que las sombras largas caen hacia el noreste y atraviesan el salón por los ventanales.
6. Añade luces interiores cálidas: unas pocas luminarias en el salón-comedor y la cocina. Comprueba que su color es cálido y que no compiten con el sol hasta quemar la imagen.
7. Elige la cámara del salón: altura de ojos de 1,20 a 1,60 m, horizontal y con las verticales rectas. Comprueba que se ve parte del ventanal y de la piscina.
8. Haz una prueba rápida de baja resolución y corrige exposición, color de las luces y materiales sobreexpuestos.
9. Genera la imagen final con el motor de render a la mayor calidad que tu equipo permita y guárdala.

## Entregable

Una vista interior con materiales y luz resueltos. Lo entregas como una imagen del salón al atardecer en horizontal, de 1920 px de ancho como mínimo, acompañada de la lista de materiales que has usado.

## Lista de comprobación

- [ ] Hay entre cuatro y seis materiales y ninguno conserva el aspecto por defecto.
- [ ] La escala de las texturas es realista (tablas de 10 a 20 cm de ancho).
- [ ] La luz principal es un sol bajo del suroeste y las sombras caen hacia el noreste.
- [ ] Las luces interiores son cálidas y visibles sin quemar la imagen.
- [ ] El horizonte está nivelado y las verticales son rectas.
- [ ] La imagen tiene al menos 1920 px de ancho y no muestra ruido de grano visible.
- [ ] No hay zonas totalmente negras ni totalmente blancas con detalle perdido.

## Errores frecuentes

- Colores saturados sin rugosidad, que dan un aspecto de plástico. Lo notas porque todo brilla igual.
- Texturas a escala incorrecta, como tablas enormes o minúsculas. Lo notas al comparar con una persona o un objeto conocido.
- Luces artificiales demasiado fuertes que anulan el atardecer. Lo notas porque ya no se ven las sombras del sol.
- Orientar mal el norte, de forma que el sol baja por donde no toca. Lo notas porque el salón no recibe luz desde los ventanales.
- Cámara demasiado alta o inclinada. Lo notas porque las paredes convergen.

## Para ir más allá

- Renderiza el mismo salón al mediodía y compara cómo cambia el ambiente.
- Prueba una segunda temperatura de luz interior y elige la que mejor funcione con el cielo.
