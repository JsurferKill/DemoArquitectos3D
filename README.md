# ZENIT — Demo de visualización arquitectónica

Prototipo de web para vender modelado, renders y recorridos a estudios de arquitectura, más un curso básico. La pieza central es **Villa Alba**, un chalet de 250 m² con piscina que se recorre con el scroll: vista cenital, fachada, entrada, cada estancia y salida, con una ficha final de precio y superficies.

## Qué hay

- `index.html` — web principal: portada con vídeo, recorrido 3D (Three.js r128) con renders de acabado y tramos en vídeo que avanzan con el scroll, servicios, proceso, preguntas y contacto.
- `curso.html` — página de venta del curso «De plano a render».
- `aviso-legal.html`, `privacidad.html` — borradores legales con huecos entre corchetes; deben revisarse antes de publicar.
- `curso/practicas/` — enunciados de las seis prácticas del curso.
- `curso/villa-alba/` — planta acotada (`planta.svg`) y cuadro de superficies.
- `renders/maqueta/` — capturas del 3D usadas como base; `renders/final/` — renders de acabado; `renders/video/` — tramos en vídeo y sus fotogramas.
- `videos/` — vídeos de portada y de la sección de trabajos.
- `SIGUIENTES-PASOS.md` — estado del proyecto y tareas pendientes.

## Verlo en local

Hace falta servirlo por HTTP (no basta con abrir el archivo):

```bash
npx serve -l 4180 .
```

y abrir `http://localhost:4180`.

Parámetros útiles en la dirección:

- `?snap` — quita la inercia del scroll, para revisar los planos uno a uno.
- `?nofx` — desactiva los efectos de imagen (oclusión ambiental, brillo, viñeta).
- `?capture` — expone `__capture(plano, ancho, alto, k)` en la consola para sacar capturas limpias del recorrido.

## Notas

- Los renders y los tramos en vídeo están generados con IA (Higgsfield) a partir de capturas del modelo 3D; la web lo indica en pantalla.
- Precios, superficies comerciales, nombre de marca y textos de servicio son de prototipo.
