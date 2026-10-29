# Ciclo de vida de contenedores docker, Dockerfile y docker hub

## Actividad 1.1: explorar una imagen

1. Busca la imagen de Apache con docker search httpd. ¿Que resultado corresponde a la imagen
oficial y como lo has identificado?
2. Descarga las etiquetas httpd:2.4 y httpd:2.4-alpine y compara su tamaño con docker image ls.
¿A qué se debe la diferencia?
3. Con docker image inspect httpd:2.4-alpine, localiza la arquitectura, el puerto que declara
(ExposedPorts), el proceso principal (Cmd), la carpeta de trabajo (WorkingDir) y la señal de parada
(StopSignal). Para obtener un dato concreto puedes usar --format, por ejemplo docker image
inspect --format '{{.Config.Cmd}}' httpd:2.4-alpine.