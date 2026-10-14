# Práctica 5 — Un recorrido horizontal y su versión vertical

Módulo 5, Animación y vídeo. Tiempo estimado: entre 3 y 5 horas. Necesitas: el modelo de la práctica 3 y las tres imágenes finales de la práctica 4.

## Objetivo

Al terminar sabrás planificar y animar un recorrido de cámara por el modelo, exportarlo como vídeo horizontal y preparar a partir de él una versión vertical. Aprenderás a controlar la velocidad, la duración y los encuadres para que el resultado se vea fluido.

## Punto de partida

El modelo de la práctica 3, las imágenes de la práctica 4 y la planta de los archivos de partida de Villa Alba (`curso/villa-alba/planta.svg`) para consultar las estancias que quieres recorrer.

## Pasos

1. Dibuja el recorrido sobre el plano en una hoja o en tu programa: de la entrada al salón y, por la cristalera, hacia el deck y la piscina. Comprueba que la trayectoria pasa por huecos reales y nunca por muros. La cristalera tiene vidrio: oculta o abre la hoja de vidrio en ese tramo para que la cámara no la atraviese.
2. Decide la duración, entre 10 y 20 segundos, y cuántos planos o tramos habrá. Escribe el guion en una lista corta con tiempo y encuadre de cada tramo, y apóyate en los encuadres de las tres imágenes de la práctica 4 para elegir qué quieres mostrar.
3. Crea la ruta de cámara en tu programa con pocos puntos de control y una altura de ojos constante, entre 1,50 y 1,60 m. Comprueba la trayectoria en la vista en planta.
4. Define el objetivo de la cámara para que mire hacia delante con giros suaves. Reproduce el recorrido en pantalla y comprueba que no hay sacudidas ni cambios bruscos de dirección.
5. Ajusta la velocidad para que sea constante, sin acelerar ni frenar bruscamente, salvo en el inicio y el final. Comprueba con un cronómetro que la duración total está dentro del rango.
6. Revisa el recorrido fotograma a fotograma en los pasos de puerta y esquinas. Comprueba que la cámara no atraviesa ningún muro ni ve el exterior del modelo por dentro.
7. Exporta el vídeo horizontal en formato 16:9, al menos 1920 × 1080 y a 24 o 30 imágenes por segundo. Si vas a recortar de él la versión vertical, exporta a 3840 × 2160: de un vídeo de 1920 × 1080 solo se aprovechan 608 px de ancho en 9:16 y habría que ampliarlo casi el doble. Comprueba que el vídeo se reproduce completo.
8. En el editor de vídeo, crea una versión vertical 9:16 de al menos 1080 × 1920 reencuadrando el contenido (a partir de 3840 × 2160 el recorte mide 1215 × 2160 px y no pierde nitidez). Si hace falta, desplaza el encuadre durante el recorrido para que el punto de interés quede centrado.
9. Exporta ambos vídeos y revísalos en una pantalla pequeña.

## Entregable

Dos vídeos exportados, uno en 16:9 y otro en 9:16. Cada uno dura entre 10 y 20 segundos.

## Lista de comprobación

- [ ] El vídeo horizontal es 16:9 y mide al menos 1920 × 1080.
- [ ] El vídeo vertical es 9:16 y mide al menos 1080 × 1920.
- [ ] La duración de cada vídeo está entre 10 y 20 segundos.
- [ ] La velocidad de cámara es constante, sin tirones.
- [ ] En ningún fotograma la cámara atraviesa un muro, una cubierta ni el suelo.
- [ ] El horizonte se mantiene nivelado a lo largo de todo el recorrido.
- [ ] En la versión vertical, el elemento principal no queda cortado en ningún momento.

## Errores frecuentes

- Demasiados puntos de control, que producen un movimiento nervioso. Lo notas al ver la trayectoria con curvas innecesarias.
- Recorridos demasiado rápidos o con cambios de ritmo. Lo notas al ver el vídeo en pantalla pequeña y no entender dónde estás.
- Atravesar muros en esquinas y puertas. Lo notas al revisar fotograma a fotograma esos puntos.
- Recortar el centro del vídeo horizontal para la versión vertical, de modo que el punto de interés queda fuera. Lo notas al ver el vídeo vertical completo.
- Exportar con una proporción distinta de la prevista. Lo notas en las propiedades del archivo.

## Para ir más allá

- Añade un fundido de entrada y salida y una pista sonora sencilla.
- Prepara una versión de unos 6 segundos, en bucle, para usar como fondo en la web.
