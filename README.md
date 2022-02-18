# Deploy a Heroku

## Objeto del documento

Describir el proceso para deplegar a producción en [Heroku](https://www.heroku.com/) + [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) una aplicación de [ExpressJS](https://expressjs.com/).

## Fases de paso a producción

El paso a producción o _deploy_ supone subir tu aplicación (tanto la BBDD de MongoDB como la aplicación de Express) a un servidor real que pueda ser accedido desde cualquier navegador. Esto, en esencia, supondrá que los datos y funcionalidades desde los que ahora accedes a través de `http://localhost:5005` serán servidos desde un dominio real como podría ser `http://www.donuts-planet.herokuapp.com`.

Para pasar a producción nuestra aplicación debemos _deployar_ los dos bloques que la componen:

### **1.- Aplicación de base de datos (MongoDB)**
Hacer el paso a producción de la base de datos (MongoDB) desde el entorno local a una base de datos remota alojada en MongoDB Atlas ([link](https://github.com/german-alvarez-dev/express-deploy-docs/blob/main/database-deploy.md)).
  
### **2.- Aplicación de servidor (ExpressJS)**
Hacer el paso a producción de la aplicación (ExpressJS) desde tu servidor local a una aplicación remota alojada en Heroku ([link](https://github.com/german-alvarez-dev/express-deploy-docs/blob/main/application-deploy.md))
