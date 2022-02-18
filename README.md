# Deploy a Heroku

## Objeto del documento

Describir el proceso para deplegar a producción en [Heroku](https://www.heroku.com/) + [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) una aplicación de [ExpressJS](https://expressjs.com/).

## Fases de paso a producción

El paso a producción o _deploy_ supone subir tu aplicación (tanto la BBDD de MongoDB como la aplicación de Express) a un servidor real que pueda ser accedido desde cualquier navegador. Esto, en esencia, supondrá que los datos y funcionalidades desde los que ahora accedes a través de `http://localhost:5005` serán servidos desde un dominio real como podría ser `http://www.donuts-planet.herokuapp.com`.

**Base de datos**: hacer el paso a producción de la base de datos local a una base de datos remota en MongoDB Atlas:
  1. Realizar el registro en MongoDB Atlas para crear y conectar la base de datos remota 
  
**Servidor**: hacer el paso a producción de la aplicación de servidor local a una aplicación remota en Heroku:
  1. Realizar el registro en Heroku para crear y configurar la aplicación remota 
  2. Transferir los archivos de la aplicación local a la aplicaciónn remota 
