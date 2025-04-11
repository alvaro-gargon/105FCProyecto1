# Fundamentos de contenerización


## Actividad 1. Servidor Web Simple con Nginx.


### Paso 1: Construcción de la imagen
```
sudo docker build -t 105fcproyecto1:1.0 .
```
 
### Paso 2. Ejecutar el contenedor en el puerto 80, 100fcproyecto1 
```
sudo docker run -d -p 80:80 --name 105fcproyecto1 105fcproyecto1:1.0
```
 
### Paso 3. Comprobación: http://localhost 

 
### Paso 4. Se pide modificar el fichero index.html desde el contenedor. 
```
sudo nano index.html

```
comprobacion
```
docker exec -it 105fcproyecto1 cat /usr/share/nginx/html/index.html

```
