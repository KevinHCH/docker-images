#Se hace esta configuracion para poder desplegar una aplicacion de front 
#haciendo la build en prod usando un container de nginx

#Establece que esta sera la imagen base
FROM node as builder
WORKDIR /usr/app
COPY ./package.json ./
RUN npm install
COPY . .
#Creamos la build del proyecto para produccion
RUN npm run build

#Busca la imagen de nginx
FROM nginx
#De la otra imagen previamente creada, copia la build completa al
# dir de web de nginx para poder servirla
COPY --from=builder /usr/app/dist /usr/share/nginx/html

