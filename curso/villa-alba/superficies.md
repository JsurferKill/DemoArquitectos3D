# Villa Alba · Cuadro de superficies (planta baja)

Fuente: escena 3D de `index.html` (unidades en metros; x crece al este, z al sur). Muros de 0,20 m centrados en los ejes, por lo que la cara interior está a 0,10 m del eje. Las esquinas exteriores llevan pilares de remate de 0,20 × 0,20 m, que no alteran las superficies. Los huecos (puertas y ventanas) se consideran cerrados en el eje del muro; no se descuentan. Altura libre interior: 3,00 m (del suelo terminado, cota 0,00, a la cara inferior de la cubierta, cota 3,00).

## 1. Superficie útil (neta) por estancia

| Estancia | Extensión interior (x · z) | Fórmula | Útil (m²) |
|---|---|---|---:|
| Salón-comedor | x −7,9 … 5,0 · z −8,9 … −1,1 | 12,9 × 7,8 − 7,0 (recinto del baño 2 hasta sus caras exteriores, x −7,9 … −5,1 y z −8,9 … −6,4: 2,8 × 2,5) | 93,62 |
| Cocina | x 5,0 … 9,9 · z −8,9 … −1,1 | 4,9 × 7,8 | 38,22 |
| Recibidor | x −7,9 … −4,1 · z −0,9 … 1,9 | 3,8 × 2,8 | 10,64 |
| Suite principal | x −12,9 … −4,1 · z 2,1 … 5,9 | 8,8 × 3,8 | 33,44 |
| Baño suite | x −12,9 … −7,9 · z −0,9 … 1,9 | 5,0 × 2,8 | 14,00 |
| Dormitorio 2 | x −12,9 … −7,9 · z −8,9 … −5,1 | 5,0 × 3,8 | 19,00 |
| Dormitorio 3 | x −12,9 … −7,9 · z −4,9 … −1,1 | 5,0 × 3,8 | 19,00 |
| Baño 2 | x −7,9 … −5,3 · z −8,9 … −6,6 | 2,6 × 2,3 | 5,98 |
| **Total útil** | | | **233,90** |

Notas de criterio:

- Salón-comedor y cocina son un único espacio en el modelo (12,9 + 4,9 = 17,8 m de largo por 7,8 m; 17,8 × 7,8 − 7,0 = 131,84 m² en total, ya descontado el recinto del baño 2). Se dividen en x = 5,00 solo para rotular, con la cocina al este.
- El recibidor es una sala cerrada: su lado norte es el muro del eje z = −1 (x −8 … −4), con un paso sin hoja de 2,30 m (x −7,5 … −5,2) que lo abre al salón. Se mide hasta la cara sur de ese muro (z = −0,9) y el salón hasta su cara norte (z = −1,1); la franja de 0,20 m entre ambos es el propio muro.
- El baño 2 es un recinto de tabiques oscuros (x = −5,2 y z = −6,5) contra el muro x = −8 y el muro norte; su puerta (x −7,4 … −6,6, en el tabique z = −6,5) da al salón.
- Las bandas de suelo de roble del modelo (suite y dormitorios) no se usan como criterio; se mide siempre a caras de muro.

## 2. Superficies construidas y de parcela

La planta es una L: bloque principal x −13 … 10 · z −9 … −1 y ala oeste x −13 … −4 · z −1 … 6 (ejes).

| Concepto | Extensión | Fórmula | m² |
|---|---|---|---:|
| Construida (caras exteriores) | x −13,1 … 10,1 · z −9,1 … −0,9 y x −13,1 … −3,9 · z −0,9 … 6,1 | 23,2 × 8,2 + 9,2 × 7,0 | 254,64 |
| Construida (a ejes, referencia) | ejes de muros exteriores | 23 × 8 + 9 × 7 | 247,00 |
| Parcela | x −15 … 15 · z −12 … 12 | 30 × 24 | 720,00 |
| Piscina, lámina de agua | x 0,5 … 9,5 · z 3,0 … 7,5 | 9,0 × 4,5 | 40,50 |
| Piscina con coronación de piedra | x 0,25 … 9,75 · z 2,75 … 7,75 | 9,5 × 5,0 | 47,50 |
| Solárium (tarima), bruto | x −4 … 12,6 · z −1 … 9,6 | 16,6 × 10,6 | 175,96 |
| Solárium sin la coronación de la piscina | | 175,96 − 47,50 | 128,46 |
| Solárium a caras exteriores del edificio, sin coronación | x −3,9 … 12,6 · z −0,9 … 9,6 | 16,5 × 10,5 − 47,5 | 125,75 |
| Porche (exterior cubierto) | x −3,6 … 11,0 · z −0,9 … 1,3 | 14,6 × 2,2 | 32,12 |
| Cubierta total (con vuelos) | x −13,4 … −3,6 · z −9,4 … 6,4 y x −3,6 … 11 · z −9,4 … 1,3 | 9,8 × 15,8 + 14,6 × 10,7 | 311,06 |

Notas: el camino de acceso (x −4 … 0,2 · z −0,5 … 0,5, 4,2 m²) queda dentro del solárium y no se resta. El porche se limita por el borde de cubierta (z = 1,3; x = 11,0) y por la cara exterior del muro sur (z = −0,9); el vuelo de 0,30 m del resto del perímetro no se cuenta.

## 3. Diferencias con la web

Cifras redondeadas de la web (`index.html`, versión actual) frente a las calculadas aquí.

| Concepto | Web | Calculado | Diferencia (calc. − web) |
|---|---:|---:|---:|
| Salón-comedor | 94 | 93,6 | −0,4 |
| Cocina | 38 | 38,2 | +0,2 |
| Recibidor | 11 | 10,6 | −0,4 |
| Suite principal | 33 | 33,4 | +0,4 |
| Baño suite | 14 | 14,0 | 0 |
| Dormitorio 2 | 19 | 19,0 | 0 |
| Dormitorio 3 | 19 | 19,0 | 0 |
| Baño 2 | 6 | 6,0 | 0 |
| Habitables / útil | 234 | 233,9 | −0,1 |
| Porche | 32 | 32,1 | +0,1 |
| Solárium | 128 | 128,5 (176,0 bruto) | +0,5 (+48,0 bruto) |
| Superficie construida | 250 | 254,6 (247,0 a ejes) | +4,6 (−3,0 a ejes) |
| Piscina (lámina) | 40 | 40,5 | +0,5 |
| Piscina, dimensiones | 9 × 4,5 m | 9,0 × 4,5 m | 0 |
| Parcela | 720 | 720,0 | 0 |

Observaciones:

- Todas las cifras de estancias coinciden con la web al redondear a metros cuadrados (la suma de la web, 94 + 38 + 11 + 33 + 14 + 19 + 19 + 6 = 234, coincide con los 234 m² habitables).
- La superficie construida de la web (250 m²) queda entre los 247,0 m² a ejes y los 254,6 m² a caras exteriores; es la única cifra que depende del criterio de medición.
- El solárium de la web (128 m²) corresponde a la tarima sin la coronación de la piscina (128,5 m²), no a la tarima bruta (176,0 m²).
