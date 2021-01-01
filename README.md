# Salida a producción de un modelo 
 
En este repo solo se hará la arquitectura del código, para así publicarlo a través de una API para que esté disponible desde la web. 
 
Para este ejemplo específico solo se realizará la publicación para un servidor local, pero lo de menos es mandarlo a un servidor de azure o en cualquier otro servicio en la nube, para que pueda ser visto por los demás usuarios.  
 
Ahora, veamos la estructura de las carpetas: 
 
![24](https://user-images.githubusercontent.com/63415652/103446057-e3e53780-4c40-11eb-9cba-282a8d5a5aa2.PNG)
 
 
Como podemos ver, el código se compone de varios archivos y varias carpetas, que son: 
 
* ArchitectVEnv: Es nuestro entorno virtual, el cual contiene todas las dependencias necesarias para que funcione el código. 
 
* in: Aquí estarán los archivos de entrada, en este proyecto será el dataset de la felicidad. 
 
* models: Aquí se guardará el mejor modelo encontrado a través de la validación cruzada. 
 
* out: Aquí saldrán los archivos CSV o de excel, pero en este caso no lo estamos usando. 
 
Ahora quedan 4 archivos más, que son: 
 
* main: Este es el archivo principal de ejecución. 
 
* models: Donde estarán nuestros modelos. 
 
* Server: Este con podrá permitir la configuración de nuestro servidor. 
 
* utils: Aquí estarán funciones como la carga y la explotación de los archivos. 
 
Ahora que ya tenemos nuestra arquitectura y el código listo, vamos a correr el servidor y nos vamos a ir a la ruta de predict: 
 
![25](https://user-images.githubusercontent.com/63415652/103446183-628ea480-4c42-11eb-98e8-f14345e3265d.PNG)
 
Y listo, tenemos un json que tiene una llave que se llama producción y el valor de la predicción que nos genero el modelo según los datos que le pasamos a nuestra predicción. 
 
Y ya así con el json que nos devolvió, podemos tratarlo en una web, una app móvil, desde js, android, etc. sin importar la naturaleza de lo que estemos haciendo ya tenemos las predicciones y tenemos un sistema que se conecta a nuestro modelo, de una manera extensible modular, fácil de utilizar que podemos convertir en la solución que estamos buscando.
