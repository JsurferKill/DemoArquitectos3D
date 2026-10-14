# Villa Alba — de la maqueta al render

Cada imagen de `maqueta/` es un plano exacto del recorrido de la web (1920 × 1080). Se sube como imagen de referencia y se pide un render fotorrealista que respete la geometría. El resultado se guarda en `final/` con el mismo nombre.

Ajustes usados: Nano Banana Pro, 16:9, 2K (2 créditos por imagen). En la tanda final el estilo se reforzó hacia «ultra-luxury modern minimalist» (travertino, microcemento, nogal a libro abierto, latón cepillado) y, en la entrada, hubo que describir el encuadre explícitamente («eye-level view… NOT an aerial view») porque el primer intento devolvió una vista aérea.

## Texto común (va al principio de todos los prompts)

```
Turn this 3D massing view into a photorealistic architectural photograph. Keep the exact same camera, perspective, composition and geometry: every wall, opening, window mullion, roof edge, piece of furniture and the pool must stay in the same position, size and proportion. Do not add, remove or move any architectural element. Replace the flat colours with real materials and natural light. Warm golden-hour sunset light from the south-west, soft long shadows, clear sky with a warm horizon. Contemporary Mediterranean villa: smooth white lime render walls, slim black aluminium frames, large clear glass panes with subtle reflections, polished light microcement floors, oak and dark walnut joinery, natural linen and bouclé upholstery. High-end architectural photography, 24 mm tilt-shift lens, straight verticals, realistic global illumination, fine material detail, no people, no text, no watermark.
```

## Texto específico de cada plano (se añade a continuación)

| Archivo | Añadir |
|---|---|
| `01-cenital.jpg` | Aerial top-down drone photograph. L-shaped single-storey house with a flat roof covered in light gravel and a row of dark solar panels, turquoise swimming pool with a stone coping, ipe wood deck, green lawn, mature palm trees, low white perimeter wall, dry Mediterranean landscape around the plot. |
| `02-fachada.jpg` | Exterior view from the garden. Fully glazed south façade under a deep cantilevered flat roof, interior softly lit with warm light, still pool water reflecting the house and the sunset sky, ipe wood deck, white sun loungers, real palm trees with detailed fronds, trimmed hedge. |
| `03-entrada.jpg` | Entrance porch. Full-height pivot door in natural oak standing open, dark walnut cladding around it, wood deck underfoot, glazed walls on both sides with gentle reflections, warm light coming from the hall. |
| `04-recibidor.jpg` | Entrance hall looking through a wide opening into the living room. Dark walnut panelled volume on the left, white walls, microcement floor with a soft sheen, large abstract terracotta painting on the far wall, linen sofa, warm evening light. |
| `05-salon.jpg` | Open-plan living room. Large low linen sofa with terracotta cushions, dark walnut coffee table, wool rug, floor lamp, open kitchen with a stone-topped island in the background, floor-to-ceiling sliding glass doors opening onto the wood deck and the pool, sunset light pouring in and casting long shadows on the floor. |
| `06-cocina.jpg` | Open kitchen. Full-height dark walnut cabinet wall with an integrated black oven, long island with a honed natural stone worktop, three brass and leather bar stools, three small pendant lights glowing warm, long horizontal window with a view of the garden at sunset, a small potted plant on the counter. |
| `07-suite.jpg` | Master bedroom. Low bed with white linen bedding and a grey wool throw, walnut slatted headboard wall, bedside tables with small warm lamps, two pendant lights, oak plank floor, wool rug, floor-to-ceiling glazing looking onto the pool and palm trees at sunset. |
| `08-bano.jpg` | Master bathroom. Freestanding white stone bathtub under a window with sunset light, floating oak vanity with a pale stone top and two basins, large mirror with a soft light strip above, frameless glass shower screen, microcement floor and walls, folded linen towels. |
| `09-dormitorio.jpg` | Secondary bedroom. Bed with white and grey linen, small walnut desk with a chair, framed print on the wall, oak plank floor, wool rug, window with warm evening light and a long shadow across the wall. |
| `10-piscina.jpg` | View across the swimming pool towards the house at dusk. Calm turquoise water with gentle ripples reflecting the lit interior, pale stone coping, ipe wood deck, white sun loungers, outdoor sofa under the porch, glazed façade glowing with warm interior light, palm tree behind the roof. |
| `11-aerea.jpg` | Aerial three-quarter drone photograph of the whole property at sunset. L-shaped flat-roofed white house with solar panels, pool and wood deck in the inner corner, lawn, palm trees with long shadows, low white perimeter wall, dry Mediterranean terrain beyond. |

## Comprobación de cada resultado

- La cámara y la geometría coinciden con la maqueta: mismos muros, huecos, carpinterías y muebles.
- No hay elementos inventados (puertas, ventanas, plantas enteras, personas, rótulos).
- La luz viene del suroeste y es de atardecer en todas, para que la serie sea coherente.
- Las imágenes están asistidas por IA: indicarlo donde se publiquen.
