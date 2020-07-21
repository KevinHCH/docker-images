# Los Dockerfiles son archivos de que permiten establecer gran parte de la configuración de nuestra
# imagen de docker, es decir, permiten crear nuestras propias imagenes personalizadas

#Busca la imagen de ubuntu, si no establece la version, coge la ultima
FROM ubuntu 

#Dentro del container ejecuta estos comandos
RUN apt-get update
RUN apt-get install nodejs -y

#Cuando termine el proceso previo ejecuta este comando dentro del container
CMD ["node"]

#La diferencia entre RUN y CMD es que el CMD se usa como comandos o parámetros que introduce
#el usuario para arrancar un script o una aplicacion


#Para "compilar" la imagen previamente creada usamos la instruccion:
#docker build -t <nombre_imagen> . 
#Se usa punto para indicar que busque el archivo Dockerfile, sólo deberia haber un archivo Dockerfile
# por carpeta o proyecto
