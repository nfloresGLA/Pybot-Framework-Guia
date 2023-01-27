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

## 2) <u> __Variables de entorno__ </u>