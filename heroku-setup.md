# Registro y creación de aplicación en Heroku

El objetivo final que perseguimos con el proceso de pasar a producción (despliegue, _deploy_, etc) es disponer de nuestra aplicación local de Express subida a un servidor en la nube y accesible mediante una URL pública como `https://donuts-planet.herokuapp.com/`.

Heroku ofrece un servicio gratuito de alojamiento para aplicaciones basadas en NodeJS, pudiendo desplegar a sus servidores los archivos de tu servidor y obteniendo así la URL que permitirá accederlo.

## Elige el nombre de tu aplicación

Tú elegirás qué nombre deseas para tus aplicación, aunque en adelante usaremos para esta documentación el nombre `donuts-planet` como ejemplo, lo que daría lugar a la URL `https://donuts-planet.herokuapp.com/`. 

Si tu proyecto se llama, por ejemplo, _Retaurants Locator_, sería ideal elegir un nombre como `restaurants-locator`, lo que dará lugar a la URL `https://restaurants-locator.herokuapp.com/`. 

No llames a tu aplicación `donuts-planet`. Este nombre sólo lo usaremos a efectos ejemplificativos, aparte que es tan molón que ya está cogido.

## Registro 

Accede a [Heroku](https://www.heroku.com/) y realiza el proceso de registro con tus datos personales.

## Creación de la app de Heroku

Para alojar una aplicación de NodeJS es necesario antes crear y configurar la aplicación en Heroku. Para ello, selecciona **Create new app** en el menú desplegable **New** de la esquina superior derecha:
<img width="788" alt="Captura de pantalla 2022-02-18 a las 7 52 55" src="https://user-images.githubusercontent.com/46670724/154638743-12a97ec8-f61d-4507-9f3b-b9a5da237635.png">

Indica a continuación el nombre de tu aplicación (recuerda: será tu futuro dominio) y selecciona **Create app**:
<img width="1116" alt="Captura de pantalla 2022-02-18 a las 7 53 55" src="https://user-images.githubusercontent.com/46670724/154638928-a476f6d6-deb5-4178-918f-cacbab5e2ec7.png">

## Conexión de la app de Heroku con el repositorio de Github

En la pestaña **Deploy** selecciona la opción **Github: connect to Github** y haz click en el botón **Connect to Github**:
<img width="1411" alt="Captura de pantalla 2022-02-18 a las 7 54 58" src="https://user-images.githubusercontent.com/46670724/154639055-b1d22a00-48c5-40f3-942d-746e9fb6fd36.png">

Permite que Heroku se conecte a tu Github haciendo click en **Authorize Heroku**:
<img width="1411" alt="Captura de pantalla 2022-02-18 a las 7 55 39" src="https://user-images.githubusercontent.com/46670724/154639385-39ea1ed0-1db8-4a4a-a3f4-7696fc1ad30e.png">

Indica el nombre del repo que aloja tu proyecto y confirma la conexión:
<img width="1411" alt="Captura de pantalla 2022-02-18 a las 8 00 41" src="https://user-images.githubusercontent.com/46670724/154639461-d2fb82c4-227a-440c-928e-28f08fb0dbbc.png">

