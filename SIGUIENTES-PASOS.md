# ZENIT — Siguientes implementaciones

Estado a 13 de octubre de 2026.

Archivos del proyecto:

- `index.html` — web principal con el recorrido 3D de Villa Alba.
- `curso.html` — página de venta del curso "De plano a render".
- `aviso-legal.html` y `privacidad.html` — borradores legales con huecos por rellenar.
- `curso/practicas/` — enunciados de las seis prácticas, sin nombrar programas.
- `curso/villa-alba/` — archivos de partida: `planta.svg` (planta acotada a 1:100) y `superficies.md` (cuadro de superficies medido sobre el modelo).
- `renders/maqueta/` — los 11 planos del recorrido capturados del 3D; `renders/final/` — sus renders de acabado; `renders/comparar.html` — maqueta y render lado a lado; `renders/clips.html` — fotogramas de cada tramo en vídeo; `renders/PROMPTS.md` — textos de partida.
- `videos/` — los tres vídeos.

Para verla: `npx serve -l 4180 .` desde esta carpeta y abrir `http://localhost:4180`. Añadir `?snap` quita la inercia del scroll y `?nofx` desactiva los efectos de imagen.

## Hecho (Fase 1)

- Pantalla de carga con progreso.
- Scroll con inercia y titulares animados palabra a palabra.
- Cámara continua por puertas y pasillos, sin fundidos a negro.
- Planta cenital acotada y minimapa de posición.
- Secciones "Cómo trabajamos" y preguntas frecuentes.

## Flecos de la Fase 1

- [ ] Revisar a ojo la fluidez del recorrido en escritorio ancho (sobre todo el giro al salir de la cocina).
- [ ] Reexportar los tres vídeos a 1080p o más y sustituirlos en `videos/` (ahora 720p y 480p).
- [ ] Sustituir los datos inventados: nombre ZENIT, precio de Villa Alba, "desde 1.900 €" y "149 €".
- [x] Superficies de la web corregidas con las medidas reales del modelo (salón-comedor 94 m², cocina 38 m², 234 m² habitables).
- [ ] Revisar los textos de "Cómo trabajamos" y de las preguntas frecuentes para que digan lo que se ofrece de verdad.
- [ ] Añadir casos reales y testimonios cuando haya material.

## Fase 2 — Realismo del chalet

- [ ] Decidir el camino: modelo 3D real, secuencia fotorrealista con scroll, o mezcla de ambos (recomendado).
- [ ] Modelar Villa Alba en un programa de 3D a partir de nuestra planta (no hay planos reales), con texturas y luz precalculada.
- [x] Reflejos del cielo en vidrio y agua; agua de la piscina con ondas.
- [ ] Vegetación y mobiliario de verdad en lugar de volúmenes simples.
- [x] Renders fotorrealistas de las 11 paradas (Higgsfield, Nano Banana Pro 2K, 24 créditos en total), fundidos sobre el 3D cuando la cámara se detiene.
- [ ] Repetir si se quiere más fidelidad: en la fachada y la piscina el render agranda o desplaza la lámina de agua; en la entrada, tras el vidrio de la derecha aparece un dormitorio donde debería verse el salón; el baño añade una segunda ventana.
- [x] Tramos en vídeo que avanzan con el scroll (Higgsfield, Seedance 2.0 Fast, 8 s a 720p): cenital a fachada, fachada a entrada, y entrada a salón pasando por el recibidor. Cada clip está troceado en 61 fotogramas en `renders/video/frames/`; los originales están en `renders/video/`.
- [x] Método que funcionó para la fachada a la entrada: cuatro referencias en orden (render de salida, dos renders intermedios sacados de capturas del propio recorrido 3D, render de llegada) y una descripción con tiempos («a los 0 s imagen 1, hacia los 2,5 s imagen 2…»). Las capturas intermedias se sacan con `?capture` y `__capture(plano, ancho, alto, k)`.
- [ ] Tramo piscina a vista aérea: Higgsfield lo ha rechazado dos veces por «contenido protegido», también con cuatro referencias. Los renders intermedios ya existen (`renders/final/10a-…` y `10b-…`). Probar otro modelo de vídeo o cambiar la imagen de salida.
- [ ] Comprobar en Higgsfield si las tres generaciones de vídeo rechazadas descontaron créditos (20 cada una).
- [ ] Resto de tramos (interiores): renders intermedios, proyección sobre la geometría o más clips (20 créditos por clip con este modelo; las 3 generaciones gratuitas ya están usadas).
- [ ] Indicar que las imágenes son asistidas por IA allí donde se publiquen (el recorrido ya lo rotula).
- [x] Efectos de imagen en escritorio: sombras de contacto, brillo suave, viñeta y suavizado de bordes.
- [x] Versión ligera: en móvil no se cargan los efectos, y en escritorio se desactivan solos si el equipo va lento.
- [ ] Actualizar el motor 3D a una versión actual (conviene hacerlo al incorporar el modelo real).
- [ ] Ajustar a ojo la intensidad de los efectos y el color del cielo y la bruma comparando con y sin `?nofx` (con efectos salen algo más pálidos).
- [ ] Valorar la transparencia del vidrio en la fachada; puede quedar demasiado invisible.
- [ ] Probar en un equipo lento que el paso automático a la versión sin efectos se ve bien (no se ha podido provocar).

## Fase 3 — El curso "De plano a render"

Seis módulos, cada uno con vídeos explicativos y una práctica de proyecto.

- [ ] Confirmar las herramientas que se enseñan (modelado, render, IA, vídeo).
- [ ] Módulo 1 — Del plano al 3D. Práctica: preparar los planos de Villa Alba.
- [ ] Módulo 2 — Modelado. Práctica: levantar el chalet.
- [ ] Módulo 3 — Materiales e iluminación. Práctica: el salón.
- [ ] Módulo 4 — Render con IA. Práctica: de maqueta a tres renders.
- [ ] Módulo 5 — Animación y vídeo. Práctica: recorrido horizontal y versión vertical.
- [ ] Módulo 6 — Web con scroll y publicación. Práctica final: proyecto propio publicado.
- [x] Enunciado de la práctica de cada módulo (`curso/practicas/`), con pasos, entregable y lista de comprobación.
- [x] Archivos de partida del módulo 1: planta acotada y cuadro de superficies de Villa Alba.
- [ ] Guion de los vídeos de cada módulo (depende de las herramientas elegidas).
- [ ] Añadir a los enunciados las indicaciones propias de cada programa cuando se elijan.
- [ ] Resto de archivos de partida: alzados y secciones, modelo base, vistas de maqueta para la práctica 4.
- [ ] Grabar los vídeos explicativos.
- [x] Página de venta del curso (`curso.html`), con temario, prácticas, preguntas y lista de espera sin pago.
- [ ] Revisar el temario de `curso.html`: los títulos de las lecciones son una propuesta sin nombrar programas.

## Fase 4 — Alojar y vender

- [ ] Elegir dónde vive el curso: plataforma hecha (recomendado para empezar) o zona privada a medida.
- [ ] Dar de alta la cuenta de cobro y los datos fiscales.
- [ ] Subir módulos, prácticas y vídeos; probar el alta de un alumno de principio a fin.
- [ ] Conectar los botones "Apuntarme" y "Pedir presupuesto" con el pago y el formulario.

## Para publicar la web

- [ ] Dominio y alojamiento.
- [ ] Formulario de contacto que envíe de verdad.
- [x] Borradores de aviso legal y de privacidad y cookies, enlazados desde el pie.
- [ ] Rellenar los huecos entre corchetes de las páginas legales (titular, NIF, domicilio, email, dominio, alojamiento, plazos de conservación) y que las revise un profesional.
- [ ] Decidir con ese profesional: bases legales de cada formulario, casilla de consentimiento en la lista de espera y si se alojan en local las tipografías y librerías.
- [x] Título, descripción e icono de la pestaña.
- [ ] Imagen para compartir en redes.
- [ ] Analítica de visitas.

## Modelo de Villa Alba

Corregido en el modelo 3D, y reflejado en la planta y el cuadro de superficies del curso:

- [x] Recibidor cerrado hacia el salón, con un paso de 2,30 m.
- [x] Baño 2 ampliado a 6 m².
- [x] Esquinas exteriores rematadas.
- [x] Muros de cierre dentro de la parcela de 30 × 24 m.

Pendiente (al no haber planos reales, se decide sobre nuestro propio diseño):

- [ ] Los dormitorios 2 y 3 y el baño 2 abren directamente al salón; falta un pasillo o distribuidor. Supone redistribuir la planta y rehacer el recorrido.

## Decisiones abiertas

1. ¿Con qué herramientas se hacen hoy el modelo y los renders?
2. Resuelto: no hay planos reales del chalet. Villa Alba es un diseño propio y su planta de referencia es `curso/villa-alba/planta.svg`.
3. ¿Plataforma hecha o curso alojado en la propia web?
4. ¿Nombre y marca definitivos?
