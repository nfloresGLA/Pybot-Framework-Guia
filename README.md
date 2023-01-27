# Guia - Pybot 2023.

### <u> ¿_Que es __Pybot___? </u>

Es un <u>framework</u> construido en __Python__ y compuesto
por multiples librerias que permiten __automatizar__
pruebas sobre diversas plataformas. <br>

Esta basado en el patron <u>__Page Object__</u>, pero con el avance
de su desarrollo se le incorporo algunas caracteristicas
de otros patrones tales como <u>__ScreenPlay y Command__</u>.

---

### <u>¿_Cuales son sus __principales__ librerias_?</u>

- __Unittest__: _Funciones_ que permiten el _armado_ del __cuerpo__
de las pruebas.

- __Pytest__: _Facilita_ la __ejecucion de las pruebas__ y la generacion de metadatos __resultantes__.

- __Request__: Ejecuta llamados a servicios API REST.

- __Allure__: Complementa el armado de pruebas con metadatos
que luego seran utilizadas para generar reportes.

- __Selenium__: Incorpora WebDrivers para la automatizacion
de Browsers (Chrome, Edge y Firebox)

- __Lackey__: Funciones para la automatizacion de inputs
al sistema. Tambien interpreta imagenes y las compara.

---

## __Requisitos previos__.

~~~ ts
> 1. Tener instalado Python
// Version de esta guia: Python 3.9.9
> 2. Tener bien configuradas las variables de entorno
// Path de Python
> 3. Tener instalado PyCharm.
// Version de esta guia: PyCharm 2022.3.1 (Community Edition)
> 4. Descargar el archivo CursoQA y agregarlo en C:\
// Nos quedaria el path de ruta: "C:\CursoQA"
~~~

---

## 1) <u> __Instalacion de Python__ </u>

### 1.1) __Descarga de Python__

<p> Pagina de descarga de
    <a 
        href="https://www.python.org/downloads/release/python-399/" 
        target="_blank">
        Python V 3.9.9
    </a>
</p>

> Ir hasta el _final de la pagina_ y buscar la seccion "_Files_".

![image](https://user-images.githubusercontent.com/120741890/215074413-51b7f829-5222-4a41-ae4a-1c0bce7ed7e7.png)

### 1.2) __Instalacion del Software__

* Primera pagina

![image](https://user-images.githubusercontent.com/120741890/215204311-ca0701c3-f253-404c-8223-16c040927dff.png)

* Segunda pagina

![image](https://user-images.githubusercontent.com/120741890/215204464-cd8a9699-97b1-443f-bb05-668106baf120.png)

* Tercera pagina

> Importante: Instalarlo en __C:\Python__

![image](https://user-images.githubusercontent.com/120741890/215204676-41865bce-b6f1-4d28-83c4-9e5a90341fb3.png)

> Click en "Install" y __confirmar__ la instalacion (Aparecera un PopUp).

> Cuando termine de instalar click en "Close" y listo.

---

## 2) <u> __Variables de entorno__ </u>

###  * _Despues de instalar Python <u>correctamente_</u>.

1. Ingresar en:

![image](https://user-images.githubusercontent.com/120741890/214583124-16506e07-cb8b-42b4-b333-b9e3f63fad25.png)

2. Doble __click__ sobre "__Path__" de "Variables del sistema"

![image](https://user-images.githubusercontent.com/120741890/214583684-4445f190-54d4-4f5b-8c16-3a59bea9671f.png)

3. Verificar de tener dentro del __path__ estos valores.

* En caso de no tener alguno agregarlos.

![image](https://user-images.githubusercontent.com/120741890/214864844-c5803bd9-eaaa-45a6-ba7f-94ae2ae6c3d9.png)

---

## 3) <u> __Instalacion de PyCharm__ </u>

<p> Pagina de descarga de
    <a 
        href="https://www.jetbrains.com/pycharm/download/download-thanks.html?platform=windows&code=PCC" 
        target="_blank">
        Pycharm-community
    </a>
</p>

> Instalacion tipica, nada particular que comentar.

## 4) <u> __Carpeta CursoQA__ </u>

> Descargar la carpeta CursoQA de este repositorio.

---

## <u>Configuracion de Pybot en Pycharm</u>

## 1. Entrar en __PyCharm__
### Vista del __primer inicio__

![image](https://user-images.githubusercontent.com/120741890/214571409-7f43f438-1270-49e1-8439-2f3cbd376e9f.png)

* Click en _Open_ para elegir la carpeta del proyecto

![image](https://user-images.githubusercontent.com/120741890/214572914-7949b93c-6ebb-4d2d-9269-977268adcdef.png)

* _¡Importante_! para facilitar la agregacion del curso
agregar la carpeta de CursoQA al directorio de C: como
se muestra en pantalla.

* Seleccionar CursoQA (tiene que quedar como directory)

![image](https://user-images.githubusercontent.com/120741890/214573249-43ca0554-6411-422d-8105-9e4df4bc9e8a.png)

* Click en "Confiar en el directorio" -> __Trust Project__

* Esto nos cargara el projecto del framework
(__Puede demorar un poco__)

![image](https://user-images.githubusercontent.com/120741890/214580052-67978dbf-54b4-44b1-9c65-f802c378f577.png)

* Asegurarse que la 📁 carpeta sea CursoQA y no Functions
(Subrayado en __amarillo__)

* __Asegurarse__ que los _niveles_ sean:
- 1: __CursoQA__
- 2: __Functions__
- 3: __.idea / src__

* Los niveles corresponden al subrayado en __rojo__.

## 2. Estructura de carpetas:

![image](https://user-images.githubusercontent.com/120741890/215223636-dac81dd4-f55c-44b2-87b7-49f757755039.png)

📁 __projects__.

 ➞ Almacena todos los archivos de los proyectos.

 📁 __nombre del proyecto__. (en este caso __ejemplo__)

 ➞ Almacena todos los archivos de un proyecto. <br>
El nombre no debera tener espacios.

📁 __src__.

 ➞ Almacena todos los archivos de un proyecto.

📁 __downloads__.

 ➞ Almacena todos los archivos descargados durante la ejecucion.

📁 __files__.

 ➞ Almacena archivos varios. Puede usarse para guardar
evidencia, archivos de config o funciones.

📁 __images__.

 ➞ Almacena imagenes que pueden utilizarse para
automatizacion por imagenes con Sikuli.

📁 __outpus__.

 ➞ Almacena archivos de salida de los scripts.
Puede utilizarse para la generacion de reportes csv u otros.

📁 __resources__.

 ➞ Almacena archivos .xlsx que contienen datos de inputs
necesarios para los casos de prueba automatizados.

📁 __pages__.

 ➞ Almacena archivos .json con los elementos capturados de una aplicacion web.

📁 __tests__.

 ➞ Almacena todos los archivos Python con las pruebas
automaticas.

## 2.2. generar las variables de entorno - venv (virtual environment)
![image](https://user-images.githubusercontent.com/120741890/215224066-40b75b19-cada-4e5f-b25c-42849cde7db1.png)

* Ingresar en las configuraciones (primera opcion - arriba a la izquierda)

![image](https://user-images.githubusercontent.com/120741890/215224339-01252754-ddfd-4400-b95b-b31e2c17933b.png)

* Project: nombreCarpeta (en este caso CursoQA) > Interpreter

![image](https://user-images.githubusercontent.com/120741890/215224431-b6b73380-d6c5-4133-a507-e112d8d65fd1.png)

* Click en la solapa de Interpreters (señalado con la flecha roja) <br>
Click en Show All.

![image](https://user-images.githubusercontent.com/120741890/215224559-0434a25f-41f1-4ff1-99bc-9c11405673fd.png)

* Click en el simbolo de __+__ señalado con la flecha.

![image](https://user-images.githubusercontent.com/120741890/215224926-1b13fd3c-2a66-4221-939b-b56a7c869bb8.png)

* No hay que tocar "nada". ya deberia aparecer asi. <br>
si tenemos todo bien deberia aparecer el "Base interpreter" <br>
configurado en donde instalamos python, en caso contrario modificarlo.

![image](https://user-images.githubusercontent.com/120741890/215225015-a15b985c-1fe8-4ffe-8027-921e1c8a4bf8.png)

> Hecho esto, click en "OK" y empezara a instalar el venv.

* En la vista anterior (Python Interpreter) deberia quedar asi.


> Tienen que aparecer estas librerias y el interpreter de Python/python.exe

![image](https://user-images.githubusercontent.com/120741890/215225303-7521620c-92b0-4a1b-a82a-36150cc5150b.png)


* En caso contrario entrar de nuevo a Show All y seleccionar esa ruta. 

> Click en Existing y buscarla en la ruta de Python: 

![image](https://user-images.githubusercontent.com/120741890/215225967-731b9881-1aca-4d9c-b516-7ba390bbf524.png)


## 2.3) Otras configuraciones necesarias.

### Configuracion de carpetas.

* Dentro de Settingss ir a la opcion de abajo de la anterior <br>
Project: NombreProyecto (este caso CursoQA) > Structure

> Hay que configurar a __functions__ como __SOURCES__ y venv _excluirlo_.

![image](https://user-images.githubusercontent.com/120741890/215226149-23b1fd51-dad8-4f2b-a76f-a45695c13fc4.png)

### Configuracion de las pruebas (Testing)

* Mas abajo de la solapa > Project ir a Tools y <br>
seleccionar en el apartado "_testing_" > __Unittest__.

![image](https://user-images.githubusercontent.com/120741890/215226528-603d37c7-cc29-4675-ab62-1bc279d0a78b.png)

* Con esto el IDE (__PyCharm__) estara _listo_ para utilizar __Pybot__.

---