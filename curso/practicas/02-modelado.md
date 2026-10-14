# Práctica 2 — Levantar el volumen del chalet

Módulo 2, Modelado. Tiempo estimado: entre 4 y 6 horas. Necesitas: el juego de planos limpio y a escala de la práctica 1.

## Objetivo

Al terminar sabrás construir en tu programa de modelado un volumen completo a partir de un plano: muros con huecos, forjado, cubierta plana con vuelo, piscina y deck. También sabrás comprobar el modelo con cifras (superficie construida y altura libre) en lugar de fiarte solo del aspecto.

## Punto de partida

El juego de planos de la práctica 1 y los archivos de partida de Villa Alba (carpeta `curso/villa-alba/`), en especial el cuadro de superficies (`superficies.md`) y la planta (`planta.svg`). La vivienda es un chalet en L de una planta: el bloque principal, al norte, contiene el salón-comedor con la cocina abierta, los dormitorios 2 y 3 y el baño 2; el ala oeste, al sur de él, contiene el recibidor (cerrado, con un paso ancho sin hoja hacia el salón), la suite y su baño. Los muros miden 0,20 m de espesor.

## Pasos

1. Abre el archivo de planos e inserta o enlaza el plano en el origen. Comprueba que las coordenadas de la esquina de la parcela coinciden con las de la práctica 1.
2. Levanta los muros siguiendo el plano, con espesor real y altura libre de 3,00 m. Mide un muro de cada ala y comprueba que el espesor y la altura son los esperados.
3. Crea el forjado de suelo y apoya los muros sobre él. Comprueba en una vista lateral que no hay huecos ni solapes entre muro y forjado.
4. Abre los huecos de puertas y ventanas con las medidas del plano. Comprueba que la puerta de entrada y los ventanales del salón dan al lugar correcto y que ningún hueco atraviesa una esquina.
5. Añade la cubierta plana, con un vuelo de 0,30 m en el perímetro y una prolongación al sur que cubre el porche (hasta unos 2,2 m más allá de la fachada sur, apoyada en dos pilares). Comprueba en alzado que es horizontal y que el vuelo se ve en la fachada sur.
6. Modela la piscina de 9 × 4,5 m como un vaso hundido y el deck de madera a su alrededor, con el porche. Comprueba que la lámina de agua queda por debajo del nivel del deck.
7. Organiza el modelo por capas o grupos: muros, forjado, cubierta, huecos, piscina, deck, parcela. Comprueba que puedes ocultar la cubierta y ver el interior.
8. Calcula la superficie construida a partir del modelo y compárala con el cuadro de superficies: 254,6 m² medidos a caras exteriores y 247,0 m² a ejes de muros (la web anuncia 250 m²). Comprueba que tu cifra queda a menos del 5 % de 250 m².
9. Da una vuelta alrededor del modelo con la vista libre y revisa que no hay caras sueltas, huecos sin cerrar ni elementos flotando.

## Entregable

El modelo de Villa Alba con la piscina y su entorno inmediato. Lo entregas como el archivo del modelo con capas ordenadas, acompañado de tres capturas de la vista general (a 1920 px de ancho como mínimo) desde el sur, el oeste y una vista aérea.

## Lista de comprobación

- [ ] La altura libre interior es de 3,00 m en todas las estancias.
- [ ] La superficie construida está entre 238 y 262 m².
- [ ] Todas las puertas y ventanas están abiertas en el muro, no dibujadas encima.
- [ ] La cubierta es plana y tiene vuelo visible en la fachada sur.
- [ ] La piscina mide 9 × 4,5 m y el deck la rodea.
- [ ] El modelo está en el origen de la práctica 1 y la orientación sur es correcta.
- [ ] Cada elemento está en su capa y puedes ocultarlos por separado.

## Errores frecuentes

- Modelar sobre un plano desplazado, de modo que el modelo queda lejos del origen. Lo notas al comparar coordenadas con la práctica 1.
- Dibujar los huecos como un dibujo pegado al muro. Lo notas al mirar desde el interior: no hay luz entre el hueco y el muro.
- Muros que no llegan al forjado o lo atraviesan. Lo notas con una vista lateral y un corte.
- Fiarte de la vista y no medir. Lo notas cuando la superficie calculada se aleja del cuadro de superficies.

## Para ir más allá

- Modela un mobiliario básico en el salón (sofá, mesa, cocina) como volúmenes simples, para que el interior no esté vacío en la práctica 3.
- Añade el cerramiento de la parcela y un volumen simple de vegetación.
