# Registro y creación de aplicación en Heroku

El objetivo final que perseguimos con el proceso de pasar a producción (despliegue, _deploy_, etc) es disponer de nuestra aplicación local de Express subida a un servidor en la nube y accesible mediante una URL pública como `https://donuts-planet.herokuapp.com/`.

Heroku ofrece un servicio gratuito de alojamiento para aplicaciones basadas en NodeJS, pudiendo desplegar a sus servidores los archivos de tu servidor y obteniendo así la URL que permitirá accederlo.

🔔 Antes de comenzar __verifica que has respetado de manera exacta los nombres de los archvios al importarlos unos en otros__ ya que, por ejemplo, un modelo denominado `Whatever.model.js` puede ser importado en local como `whatever.model` pero tras el deploy fallará ya que es case-sensitive.

<hr><br>

## 1.- Elige el nombre de tu aplicación <br>

Tú elegirás qué nombre deseas para tus aplicación, aunque en adelante usaremos para esta documentación el nombre `donuts-planet` como ejemplo, lo que daría lugar a la URL `https://donuts-planet.herokuapp.com/`. 

Si tu proyecto se llama, por ejemplo, _Retaurants Locator_, sería ideal elegir un nombre como `restaurants-locator`, lo que dará lugar a la URL `https://restaurants-locator.herokuapp.com/`. 

No llames a tu aplicación `donuts-planet`. Este nombre sólo lo usaremos a efectos ejemplificativos, aparte que es tan molón que ya está cogido.

<hr><br>

## 2.- Registro <br>

Accede a [Heroku](https://www.heroku.com/) y realiza el proceso de registro con tus datos personales.

<hr><br>

## 3.- Creación de la app de Heroku <br>

Para alojar una aplicación de NodeJS es necesario antes crear y configurar la aplicación en Heroku. Para ello, selecciona **Create new app** en el menú desplegable **New** de la esquina superior derecha: <br><br>
<img width="788" alt="Captura de pantalla 2022-02-18 a las 7 52 55" src="https://user-images.githubusercontent.com/46670724/154638743-12a97ec8-f61d-4507-9f3b-b9a5da237635.png">

Indica a continuación el nombre de tu aplicación (recuerda: será tu futuro dominio) y selecciona **Create app**: <br><br>
<img width="1116" alt="Captura de pantalla 2022-02-18 a las 7 53 55" src="https://user-images.githubusercontent.com/46670724/154638928-a476f6d6-deb5-4178-918f-cacbab5e2ec7.png">

<hr><br>

## 4.- Conexión de la app de Heroku con el repositorio de Github <br>

En la pestaña **Deploy** selecciona la opción **Github: connect to Github** y haz click en el botón **Connect to Github**: <br><br>
<img width="1411" alt="Captura de pantalla 2022-02-18 a las 7 54 58" src="https://user-images.githubusercontent.com/46670724/154639055-b1d22a00-48c5-40f3-942d-746e9fb6fd36.png">

Permite que Heroku se conecte a tu Github haciendo click en **Authorize Heroku**: <br><br>
<img width="1411" alt="Captura de pantalla 2022-02-18 a las 7 55 39" src="https://user-images.githubusercontent.com/46670724/154639385-39ea1ed0-1db8-4a4a-a3f4-7696fc1ad30e.png">

Indica el nombre del repo que aloja tu proyecto y confirma la conexión haciendo click en el botón **Connect**: <br><br>
<img width="1411" alt="Captura de pantalla 2022-02-18 a las 8 00 41" src="https://user-images.githubusercontent.com/46670724/154639461-d2fb82c4-227a-440c-928e-28f08fb0dbbc.png">

Una vez conectado, selecciona **Enable automatic deploys**: <br><br>
<img width="1411" alt="Captura de pantalla 2022-02-18 a las 8 26 55" src="https://user-images.githubusercontent.com/46670724/154640035-fc791a6b-ba50-4eb5-a144-9163bc024585.png">

<hr><br>

## 5.- Agregación de variables de entorno <br>

Debido a que tu archivo `.env` no será subido, debes dar de alta manualmente cada variable de entorno a excepción de `PORT`. Para ello, accede a la pestaña **Settings** y, enla sección **Config vars** añade una por una todas las variables presentes en tu `.env`: <br><br>
<img width="1411" alt="Captura de pantalla 2022-02-18 a las 8 28 17" src="https://user-images.githubusercontent.com/46670724/154641152-0c48acd5-0e43-4f87-bf83-a17afc89e303.png">

<hr><br>

## 6.- Deploy! <br>

En la pestaña Settings, asegúrate de en la sección Buildpacks está seleccionado **NodeJS** (esto se verá como `heroku/nodejs`). De lo contrario, añádelo como Buildpack: <br><br>
<img width="1411" alt="Captura de pantalla 2022-02-18 a las 8 48 29" src="https://user-images.githubusercontent.com/46670724/154640454-fd12a0f5-d265-43a0-915c-ced1c2aaa4ba.png">

Accede de nuevo a la pestaña Deploy y selecciona, al final de la misma, el botón **Deploy branch**: <br><br>
<img width="1411" alt="Captura de pantalla 2022-02-18 a las 8 50 23" src="https://user-images.githubusercontent.com/46670724/154640650-17315830-a147-479a-a834-3b804b9e81d8.png">

Ya puedes acceder a la URL de tu proyecto. ¡Enhorabuena!


