# Vídeo de presentación — paquete para Higgsfield Katana

**Pieza:** «VILLA ALBA — ÚLTIMO REFUGIO». Tráiler de unos 55 s, 16:9, 1080p, que presenta tres cosas en este orden: el recorrido 3D de la casa, la web donde se recorre y el curso de renders con IA.

**Tono:** distópico y serio, con precisión arquitectónica. El mundo de fuera es gris, polvoriento y vigilado; la casa es lo único cálido, nítido y real. El contraste entre las dos cosas es lo que da el impacto.

El guion en formato máquina, con rutas y prompts por plano, está en [`guion.json`](guion.json).

---

## 1. Cómo usarlo en Katana

Katana recrea el montaje de un **vídeo de referencia** con tus propios recursos, y se lanza desde Claude con el conector de Higgsfield.

1. **Vídeo de referencia.** Elige en *Presets de la comunidad → Style transfer* o *Personalized edits* uno con cortes rápidos, glitch, rampas de velocidad y rótulos tipográficos (estilo tráiler o anuncio tecnológico). Si no hay ninguno así, sube tú un tráiler de referencia de 30–60 s con ese ritmo.
2. **Personajes y recursos.** Sube los de la sección 4, en el orden del guion. La casa es el «personaje»: tiene que salir siempre igual.
3. **Instrucciones.** Pega el prompt maestro de la sección 2.
4. **Coste.** Antes de generar, pide el presupuesto exacto (el conector tiene una opción que calcula el coste sin lanzar nada). En la lista de presets aparecen cifras de 57 a 189 junto a «Recrear»; si son créditos, cuenta con eso por versión.
5. **Textos en pantalla.** Si Katana deforma los rótulos, genera el vídeo sin texto y añádelos después con los de la sección 5.

---

## 2. Prompt maestro (pegar en «Instrucciones»)

```
Recreate the reference edit as a dystopian architectural trailer for a real house called Villa Alba. Keep the reference's pacing, cuts, speed ramps and transitions, but replace all of its content with the uploaded assets, in the order given.

World and tone: a grey, dusty, surveilled near-future city of brutalist towers and haze; cold desaturated teal and ash tones, film grain, subtle chromatic aberration, thin scan lines, drone telemetry HUD elements (altitude, coordinates, timecode) in a thin monospace font. Against that world, the house is the only warm, sharp, perfectly lit thing: golden sunset light, white lime walls, walnut, travertine, a turquoise pool.

Rules: the house, its architecture, materials, furniture and camera paths must stay exactly as in the uploaded images and clips; never redesign, add or remove walls, windows or rooms. No people, no faces, no logos other than ZENIT, no invented text. Transitions: glitch cuts, scan-line wipes from the 3D massing view to the photoreal render, whip pans, flash frames, and short speed ramps on the drone clips. End on a clean, still, serious end card.

Structure: 1) cold open in the dystopian city, 2) reveal of Villa Alba from above, 3) drone descent and walk-through, 4) data sheet, 5) the interactive website that shows the tour, 6) the course "De plano a render" with fast before/after flashes, 7) ZENIT end card.
```

---

## 3. Guion plano a plano

| # | Tiempo | Plano | Recurso | Movimiento y transición | Texto en pantalla |
|---|---|---|---|---|---|
| 1 | 0–4 s | Señal: negro, ruido, una línea de escaneo roja cruza la pantalla | `videos/v1.mp4` muy desaturado | Entra con interferencia; corte seco | 2049. LAS CIUDADES YA NO SE DIBUJAN. |
| 2 | 4–9 s | La ciudad: torres en la bruma, polvo en el aire | `videos/v2.mp4`, `videos/v3.mp4` | Rampa de velocidad, flash blanco de 2 fotogramas | SE GENERAN. |
| 3 | 9–14 s | Revelación: la maqueta gris de Villa Alba vista desde arriba se convierte en render | `renders/maqueta/01-cenital.jpg` → `renders/final/01-cenital.webp` | Barrido de escaneo con rejilla HUD; datos de coordenadas | VILLA ALBA · 250 m² |
| 4 | 14–22 s | Descenso del dron hasta la fachada | `renders/video/t1-cenital-fachada.mp4` | HUD de telemetría (altitud que baja, rumbo); rampa lenta al llegar | ÚLTIMO REFUGIO |
| 5 | 22–30 s | Llegada a la entrada y entrada en la casa | `renders/video/t2-fachada-entrada.mp4`, `renders/video/t3-entrada-salon.mp4` | Continuo; al cruzar la puerta, golpe de luz cálida | SALÓN · 94 m² |
| 6 | 30–36 s | Estancias en ráfaga | `renders/final/06-cocina.webp`, `07-suite.webp`, `08-bano.webp`, `09-dormitorio.webp`, `10-piscina.webp` | Barridos rápidos (0,8–1,2 s por imagen), leve empuje de cámara | COCINA · SUITE · BAÑO · DORMITORIOS · PISCINA |
| 7 | 36–41 s | Ficha: vista aérea con datos que se teclean | `renders/final/11-aerea.webp` | Números que parpadean como en un terminal | 1.180.000 € · 3 DORMITORIOS · 2 BAÑOS · ENERGÍA A |
| 8 | 41–47 s | La web: el recorrido con scroll en un portátil sobre una mesa oscura | Grabación de pantalla de la web (ver 4.3) | Encuadre de producto, reflejo en la pantalla | TU PROYECTO, RECORRIDO EN LA WEB |
| 9 | 47–52 s | El curso: maqueta y render alternando muy rápido | Pares de `renders/maqueta/` y `renders/final/` | Parpadeo antes/después, 0,3 s por par | DE PLANO A RENDER · CURSO · 6 MÓDULOS |
| 10 | 52–56 s | Cierre | Fondo negro con grano | El logotipo entra con glitch y se queda quieto | ZENIT · RENDERS Y RECORRIDOS CON IA PARA ESTUDIOS |

---

## 4. Recursos

Todos están en este repositorio. Si el repositorio es público, cada archivo se puede pasar también por URL: `https://raw.githubusercontent.com/JsurferKill/DemoArquitectos3D/main/` + la ruta.

### 4.1 La casa (siempre igual)
- Renders finales, 1920 px: `renders/final/01-cenital.webp` … `11-aerea.webp`.
- Renders intermedios de los tramos: `renders/final/02a-…`, `02b-…`, `10a-…`, `10b-…`.
- Maquetas del 3D, mismos encuadres: `renders/maqueta/*.jpg`.
- Tramos en vídeo, 8 s a 720p: `renders/video/t1-cenital-fachada.mp4`, `t2-fachada-entrada.mp4`, `t3-entrada-salon.mp4`.

### 4.2 El mundo distópico
- Torres y ciudad: `videos/v1.mp4` (maqueta a render), `videos/v2.mp4` (recorrido), `videos/v3.mp4` (vertical).
- Si hacen falta más planos de ciudad, prompt para generarlos aparte (imagen o vídeo):

```
Wide establishing shot of a grey brutalist megacity at dusk, endless concrete towers fading into toxic haze and dust, faint red warning lights, surveillance drones as tiny dots, cold desaturated teal and ash palette, film grain, anamorphic lens, cinematic, no people, no text.
```

### 4.3 La web (pendiente de grabar)
Graba la pantalla mientras haces scroll por el recorrido, a 1920×1080 y 30 fps:

1. Abre `http://localhost:4180` con el proyecto servido (`npx serve -l 4180 .`) o la web publicada.
2. Pulsa **Win + Alt + R** (barra de juego de Windows) para grabar la ventana del navegador.
3. Haz scroll lento desde la portada hasta la ficha: tarda unos 40 s en recorrerlo todo.
4. Repite en la página del curso, `http://localhost:4180/curso`.

Guarda las grabaciones en `presentacion/grabaciones/` y súbelas como recursos.

---

## 5. Textos en pantalla

- Tipografía: rótulos en **Inter** mayúsculas con mucho espaciado; datos y HUD en monoespaciada fina.
- Colores: blanco hueso `#f3eee5` sobre negro `#0b0a09`; acento dorado de marca `#cfa96d`; rojo de alarma solo en el plano 1.
- Textos, en orden:
  1. 2049. LAS CIUDADES YA NO SE DIBUJAN.
  2. SE GENERAN.
  3. VILLA ALBA · 250 m²
  4. ÚLTIMO REFUGIO
  5. SALÓN · 94 m²
  6. COCINA · SUITE · BAÑO · DORMITORIOS · PISCINA
  7. 1.180.000 € · 3 DORMITORIOS · 2 BAÑOS · ENERGÍA A
  8. TU PROYECTO, RECORRIDO EN LA WEB
  9. DE PLANO A RENDER · CURSO · 6 MÓDULOS
  10. ZENIT · RENDERS Y RECORRIDOS CON IA PARA ESTUDIOS

Las cifras salen de la web y son de prototipo.

---

## 6. Sonido

Katana no pone música propia más allá de la del vídeo de referencia. Si hay que añadirla después:

- Dron grave continuo y viento con polvo de fondo.
- Golpe de subgrave en cada corte de los planos 1, 2 y 3.
- Interferencia digital en los glitch.
- Al entrar en la casa (plano 5) la mezcla se abre: menos ruido, un acorde cálido.
- Silencio total un instante antes del cierre.

---

## 7. Variaciones

- **Vertical para redes (9:16):** mismos planos; usa `videos/v3.mp4` en el plano 2 y reencuadra los renders al centro.
- **Versión de 15 s:** planos 3, 4, 6 (dos estancias), 9 y 10.
- **Versión solo curso:** planos 1, 3, 9 y 10, con el texto «APRENDE A HACERLO» antes del cierre.

---

## 8. Comprobación antes de dar por buena una versión

- La casa es la misma en todos los planos: muros, ventanas, piscina y muebles en su sitio.
- No hay personas, caras ni logotipos ajenos.
- Los textos se leen y no tienen letras inventadas.
- El orden cuenta la historia: ciudad, casa, recorrido, ficha, web, curso, cierre.
- Indica que las imágenes están asistidas por IA donde se publique.
