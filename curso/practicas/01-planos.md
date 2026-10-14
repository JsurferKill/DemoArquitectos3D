# Práctica 1 — Preparar los planos de Villa Alba

Módulo 1, Del plano al 3D. Tiempo estimado: entre 2 y 3 horas. Necesitas: solo los archivos de partida de Villa Alba.

## Objetivo

Al terminar sabrás dejar un plano listo para modelar: sin ruido, a escala real, con unidades coherentes, un origen de referencia fijo y cada tipo de elemento en su propia capa. Es la base de todo lo que viene después; un error de escala aquí se arrastra hasta la web final.

## Punto de partida

Los archivos de partida de Villa Alba (carpeta `curso/villa-alba/`): el plano acotado de la planta (`planta.svg`, a escala 1:100, con el norte hacia arriba) y el cuadro de superficies (`superficies.md`), que también indica la altura libre de 3,00 m. La parcela mide 30 × 24 m (720 m²), la fachada principal mira al sur y la vivienda es un chalet en L de una planta y unos 250 m². El plano llama solárium a la tarima de madera que rodea la piscina; en estas prácticas se le llama también deck.

## Pasos

1. Crea la estructura de carpetas del curso (partida, modelo, imágenes, vídeo, web) y copia dentro los archivos de partida. Comprueba que puedes abrirlos desde la nueva ubicación.
2. Abre el plano en tu programa de modelado o de dibujo y fija las unidades en metros (o milímetros, pero decide una y no la cambies). Comprueba que una cota conocida, por ejemplo el lado de 30 m de la parcela, se lee como 30 m.
3. Limpia el plano: elimina el cajetín, la leyenda, las notas, los rótulos de estancia, los rayados, el mobiliario y todo lo que no sea geometría de obra o cota. Comprueba que solo quedan muros, huecos, cubierta, piscina, deck, porche, límites de parcela y cotas.
4. Escala el plano si hace falta. Mide dos distancias en direcciones distintas, una horizontal y otra vertical, y compáralas con las cotas impresas. Comprueba que la diferencia es inferior a 1 cm.
5. Elige un punto de referencia, por ejemplo la esquina suroeste de la parcela, y colócalo en el origen (0, 0). Comprueba que todo el plano queda en coordenadas positivas y que el sur apunta hacia abajo en la vista en planta.
6. Crea capas por elemento: muros, huecos, forjado, cubierta, piscina, deck y porche, parcela, cotas. Pasa cada línea a su capa. Comprueba que al apagar una capa desaparece solo ese elemento.
7. Los archivos de partida solo incluyen la planta. Anota en el propio archivo la altura libre de 3,00 m, que usarás en la práctica 2; si además tienes alzados o secciones propios, colócalos junto a la planta, a la misma escala y alineados con ella. Comprueba que la altura libre que figura en ellos es 3,00 m.
8. Mide en el plano la superficie útil de cada estancia, a caras interiores de los muros, y compárala con la columna "Útil" del cuadro de superficies. Anota las diferencias.
9. Guarda el archivo con un nombre claro y con versión (por ejemplo, planos_villa-alba_v1) y haz una copia de seguridad.

## Entregable

Un juego de planos limpio, a escala y listo para modelar. Lo entregas como el archivo de planos con unidades definidas, origen fijo y capas por elemento, acompañado de una imagen de la planta en horizontal, de al menos 1920 px de ancho, que muestre las capas visibles.

## Lista de comprobación

- [ ] Las unidades están definidas y son las mismas en todo el archivo.
- [ ] La parcela mide 30 × 24 m con una tolerancia de 1 cm.
- [ ] La piscina mide 9 × 4,5 m.
- [ ] El origen (0, 0) está en el punto de referencia elegido y el sur queda hacia abajo.
- [ ] Hay una capa por tipo de elemento y ninguna línea queda en la capa por defecto.
- [ ] No quedan rótulos, notas, rayados ni mobiliario; el único texto son las cotas, en su capa.
- [ ] La suma de superficies útiles medidas se acerca al total del cuadro de superficies (233,90 m²), con una diferencia inferior al 3 %.

## Errores frecuentes

- Escalar con una sola medida: el plano parece correcto en un eje y falla en el otro. Compruébalo midiendo en dos direcciones.
- Mezclar unidades, como un plano en centímetros dentro de un archivo en metros. Lo notas porque la parcela sale cien veces más grande o más pequeña.
- Dejar el plano lejos del origen. Más adelante la cámara y las vistas se comportan de forma extraña; lo notas si las coordenadas tienen muchas cifras.
- Meter todo en una sola capa, lo que obliga a seleccionar a mano al modelar. Lo notas al apagar una capa y ver que no cambia nada.

## Para ir más allá

- Añade una capa de acotaciones propias (ejes y cotas totales) para comprobar el modelo del módulo 2.
- Prepara un segundo archivo con el plano simplificado solo con contornos, útil como base ligera.
