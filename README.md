# El Origen - Productos Naturales

## Stack
El proyecto está armado con NodeJS por lo cuál corre en un entorno de NGINX.

Se compone por:

 - Armado web en servidor (SSR)
 - REST API

**Keywords**: NodeJS, EJS, API, MongoDB, Heroku

## Levantar el proyecto
Para levantar el proyecto local:

 1. Descarga del repo
 2. Instalar módulos en el **/website** y en la  **/api**

    *npm i* 

Para que funcione el sitio es necesario primero levantar el servicio en **/api**.

#### Levantar API

 1. Levantar una instancia local de MongoDB que exponga el puerto 27017. 
 2. Crear una base llamada **origen** en MongoDB
 3. Levantar el servicio con el comando `node index.js` dentro de **api/src**. Opcionalmente se puede usar `nodemon index.js` si se va a trabajar sobre la API

#### Levantar Website

Una vez corriendo el servicio, levantar el proyecto **website** con los comandos `node app.js` o `nodemon app.js` en la carpeta **/website**


## Consignas del trabajo

El proyecto cuenta de dos partes:
   

#### Cliente
El origen es una empresa en desarrollo que vende alimentos naturales.

  

#### Pedido

Como cliente está interesado en armar una web en donde muestre sus productos para generar identidad de marca. Además nos comenta que tiene perspectivas de crecimiento y quiere armar, a largo plazo, una aplicación y un blog en donde muestre cómo hacer las recetas de los productos que vende.

  

## Aspectos Técnicos

El departamento de diseño relevó lo que quiere el cliente y armó un diseño de la web a realizar.  

### Bootstrap

Como este cliente es un potencial cliente a largo plazo, desde el departamento técnico nos piden que utilicemos Bootstrap para el desarrollo, dada que esta tecnología es conocida por muchos/as desarrolladores/as y nos permite realizar cambios de manera simple.

  
### Web - App - Blog

Entendiendo que el cliente hoy quiere una web, pero es posible que mañana quiera una App y un Blog. El equipo técnico pide que armemos una REST API. Hoy solamente quiere un endpoint de productos en donde se listen los productos.

 

### Base de Datos

Si bien el cliente aún no tiene una base de datos, sí tiene una lista de los productos que vende.

  

## Equipos

  

### Equipo FrontEnd

Encargado de desarrollar la página en Bootstrap. La página deberá ser 100% estática para luego pasarla al equipo de BackEnd.

  

### Equipo BackEnd:

Encargado de tomar la producción que armó el equipo FrontEnd y dinamizar la página. Deberán armar la página con SSR, utilizando un motor de témplales EJS. La página debe contar con los partials necesarios para que la misma pueda crecer en el tiempo.

  

### Equipo API:

Encargado de armar el servicio que traiga productos. Esta API servirá tanto para la web, como para la app y el blog.