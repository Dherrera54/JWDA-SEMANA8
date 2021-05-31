# JWDA-SEMANA8

Repositorio del grupo conformado por: Angelica Rodriguez, Jorge Barrera, Wilson Gonzalez y Dario Herrera

Ghost 3.42.5

## Estrategia de pruebas

De acuerdo con lo requerido, hemos preparado la estrategia de pruebas para la herramienta GHOST v3.42.5, considerando un periodo de 8 semanas para las pruebas, y 4 ingenieros con una carga de 8 horas semanales cada uno. En el siguiente enlace se puede acceder a la estrategia de pruebas de nuestro equipo: [Estrategia de pruebas](https://drive.google.com/file/d/14q8HxiaViYn40oREXcW4lmNxdKC6othO/view?usp=sharing)

A continuación detallaremos la distribución de actividades a realizar en las 8 semanas de trabajo.

## Semana 1

En la semana 1, además del diseño de la estrategia de pruebas, hemos considerado la reunión con el Gerente de Proyecto así como la organización y estructuración del repositorio que usaremos en el transcurso del proyecto.

De igual manera como parte de las actividade de la primera semana, hemos iniciado con las pruebas exploratorias manuales, así como pruebas de reconocimiento aleatorias con Smart-Monkey.

Los resultados de las pruebas exploratorias manuales los hemos documentado en el inventario que se encuentra en el siguiente enlance: [Inventario de pruebas exploratorias](https://uniandes-my.sharepoint.com/:x:/g/personal/d_herrerag_uniandes_edu_co/EchmpZbGTXdOkKtGqViiDvgBieczDyZ6d1mnLPSZLi9Nuw?e=l489rD)

El resultado de las pruebas de reconocimiento con Smart-Monkey se encuentra documentado en el siguiente video:

[!image](https://user-images.githubusercontent.com/78655008/120123322-c8d90e00-c173-11eb-97d1-bacc6a07632f.mp4)

### [Pruebas E2E Kraken](https://github.com/Dherrera54/JWDA-Semana8/tree/E2E_Kraken_Ghost3.42.5)

# Pruebas visuales VRT
En la estrategia visuales par VRT se crea con Resemble, aca contiene el link de la rama que se creo para la ejecucion **https://github.com/Alejito29/JWDA-Kraken-Semana5/tree/Resemble/Semana6/resemble**

Una breve explicacion para la ejecucion de **Resemble.JS**, el detalle se encuentra en el link indicado en la descripcion.

# Ejecutando VRT con Resemble.js ⚙️

Para ejecutar debe  hacer lo siguiente:

1. **Para ejecutar VRT en Resemble.js** debe ejecutar el comando **git checkout Resemble/Semana6**
2. Luego de moverse a la rama Resemble/Semana6 debe ir a la carpeta **resemble** ejecutando el siguiente comando **cd resemble**
3. Allí deberá ejecutar el comando **npm install**
4. En el archivo **index.js** que se encuentra dentro de la carpeta **resemble** deberá modificar el path que contiene a la carpeta **resemble**, como se indica en la siguiente imagen:

![image](https://user-images.githubusercontent.com/78829003/118384661-7f15f280-b5cd-11eb-8467-f3b1a93bc2b5.png)
5. Para ejecutar el vrt para cada uno de los escenarios deberá modificar la variable **scenario** y la variable **steps**, teniendo en cuenta lo siguiente:

![image](https://user-images.githubusercontent.com/78829003/118384817-d6689280-b5ce-11eb-90d3-2f21376cf51e.png)

|Scenario|Steps|
|--------|-----|
|Login_invalid_user_invalid_pass|6|
|Login_invalid_user_valid_pass|6|
|Manage_settings_change_timezone|10|
|Manage_settings_make_private|9|
|Pages_filter_by_item_1st|11|
|Pages_filter_by_item_1st_to_4th|17|
|Post_creation_new_post_button|13|
|Post_creation_scheduled|19|
|Tag_manage_add_metadata|16|
|Tag_manage_delete_tag|13|


6. Luego de modificar las variables anteriores, deberá ejecutar el comando **node index.js** lo cual le creará una carpeta dentro de la carpeta **results** con el nombre del escenario ejecutado. Dentro de esta carpeta encontrará las imágenes del resultado de las comparaciones realizadas paso a paso y el reporte de cada una de estas comparaciones, igualmente por cada paso.

![image](https://user-images.githubusercontent.com/78829003/118384703-ecc21e80-b5cd-11eb-8b9c-41c7bc78ceef.png)



# Pruebas con datos aleatorio- pseudo aleatorio y aleatorio
La estrategia para esas pruebas se puede ejecutar del  siguiente link **https://github.com/Alejito29/JWDA-Kraken-Semana5/tree/feature/ag_kraken_data**, en el cual se crea un programa que permite crear diferentes archivos en base al escenario escogido. 

Una breve explicacion para la ejecucion de **Pruebas con datos aleatorio- pseudo aleatorio y aleatorio**, el detalle se encuentra en el link indicado en la descripcion del readme


## Pasos para ejecutar el Generador.jar para las pruebas E2E sobre Ghost 3.42.5: Este tiene cubrimientos para generar  los diferentes tipos de datos **Prioriatio, Complemento del pseudo y aleatorio**

* Clonar el repositorio **https://github.com/Alejito29/JWDA-Kraken-Semana5**

* Ubicarse en la rama **feature/ag_kraken_data**

* Abrir el ejecutable **Generador.jar** que se encuentra en la raiz del proyecto, en caso de ser sistema operativo linux debe ejecutarlo con la terminal, si es mac o windows unicamente debe darle doble click, como requisito es necesario que tenga instalado JAVA  1.7.

![Evidenica jar2](https://user-images.githubusercontent.com/78820446/119274217-70829900-bbd4-11eb-989e-1825cb0150da.png)


* Por ultimo debe escoger el nombre del test, cuantas veces se va repetir la creacion y que tipo de dato desea. Con el jar podra crear diferentes tipos de datos, en este caso usted define cuanto dataset desea generar, aunque si genera el maximo cubriria los casos solicitados solo que se demoraria la ejecucion.

 ![Evidenica jar](https://user-images.githubusercontent.com/78820446/119274137-1bdf1e00-bbd4-11eb-9f1e-ab7cb971bb13.png)

Observacion en la wiki se encuentra el detalle tecnico como ejecutar cada prueba con los diferentes tipos de datos 

* https://github.com/Alejito29/JWDA-Kraken-Semana5/wiki/Pool-de-datos-Apriori
* https://github.com/Alejito29/JWDA-Kraken-Semana5/wiki/Pool-de-datos-pseudo-aleatorio-din%C3%A1mico
* https://github.com/Alejito29/JWDA-Kraken-Semana5/wiki/Aleatorio

Adicional en caso que desen tener acceso al fuente del codigo java lo encontraran aca **https://github.com/Alejito29/JWDA-Java-Semana7**

