#Ahora se va a crear una imagen usando la base de Alpine, alpine son distros ligeras super basicas
#orientadas a la seguridad y al minimalismo de linux, por tener, no tiene ni bash


FROM alpine
#Lanza desde la consola apk (Repos de alpine) y agrega el modulo bash
RUN apk add --update bash

#Se define que por defecto abra la consola y la deje en bash lista para poder usar comandos de bash
#Ejemplo: docker run --name custom_bash bash_image -c ls
#-c ls: Es un comando terminal de linux que permite listar los directorios, de esta manera se podrían
#ejecutar distintos comandos pasados por parámetros
ENTRYPOINT ["bash"]
