#Busca y descarga la imagen de node 
FROM node
#Establece que el directorio de trabajo dentro del container sea /usr/app
WORKDIR /usr/app
#Copia el archivo package.json al directorio de trabajo previamente establecido
COPY ./package.json ./
#Arranca este comando para traer las denpendencias
RUN npm install
#Copia todo el contenido de esta carpeta al contenedor al directorio previamente establecido
COPY . .
#Arranca el programa con estos 3 params (Todos hacen un comando)
CMD ["npm", "run", "start"]

#Una vez se haya creado la imagen, se debe arrancar el container y habilitar el puerto.
#Es necesario tener en cuenta el puerto  del containr y el puerto por que saldra por nuestra maquina
#docker run --name express_container -t -d -p 3000:3000 express

