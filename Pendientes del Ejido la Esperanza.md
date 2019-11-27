Alejandro Ramirez Serratos,   
    correo electronico: aserratos0809@gmail.com 
    
Mario Humberto González Dimas,  
    correo electronico: mgonzalez26@ucol.mx

Juan David Hernandez Hernandez,  
    correo electronico: jhernandez14@ucol.mx
    
Campus Coquimatlán, 28400

# Pendientes-del-Ejido-la-Esperanza

Muestra los datos obtenidos de obtención de las pendientes del Ejido la Esperanza y finalmente poder mostrar una imagen de dicho Ejido.

![PalabrasdelTextoAlternativo](https://github.com/Alejandro480/Pendientes-del-Ejido-la-Esperanza/blob/master/EJIDO.png)

En la siguiente Imagen se muestra una pequeña simbologia del los rangos de elevacion con sus respectivos colores

![PalabrasdelTextoAlternativo](https://github.com/Alejandro480/Pendientes-del-Ejido-la-Esperanza/blob/master/RANGOS.png)

# Resumen

En este proyecto se prevé hacer un mapa temático del ejido la esperanza el cual contenga las características junto con las pendientes, de poder leerlo y saber que se puede sembrar en el área a estudiar.

Palabras clave: Sembrar, Cultivo, Mapa Temático, Pendiente

# Abstrac

In this project it is planned to make a thematic map of the ejido, the hope which contains the characteristics along with the slopes, of being able to read it and know that it can be sown in the area to be studied.

Keywords: Sowing, Cultivation, Thematic Map, Earrings

# Introduccion

En el proyecto se utilizará un conjunto de datos vectoriales descargados desde la página del INEGI los cuales nos permitirán crear una representación gráfica (Mapa) en ArcMap de las distintas clases de pendientes aptas para el cultivo de maíz, caña y ganadería, teniendo en cuenta que las pendientes demasiado inclinadas no son favorables debido a que existe una gran pérdida de terreno a causa de la erosión del mismo, además se aprovecha más un terreno plano o con menor pendiente.

En algunos casos la pendiente es importante para poder colocar un sistema de riego; es muy favorable tener pendientes en el terreno para que con ayuda de la gravedad el agua pueda llegar a su destino de riego.

Con la ayuda de la programación asignaremos una clasificación correspondiente a la pendiente conveniente para el cultivo y la ganadería, que automáticamente dándole la clase de pendiente asignará para qué es apta esa área.

# Desarrollo

Para desarrollar este programa se tiene que utilizar un paquete de Python que proporciona los diferentes pendientes que tiene el ejido  a estudiar con la herramienta de los sistemas de información Geográfica como lo es QGIS

1.-   Se tiene que importar e instalar la librería usada la cual es "openpyxl" ya que con ella se basara nuestro proyecto.

2.- Para poder leer el programa se tiene que tener el ejido a estudiar  como shp para que con ese formato podamos sacar las características de las pendientes.

3.- Se toman y verifican las características del terreno a estudiar para poder tener los cálculos necesarios

4.- Se imprimen los datos correspondientes para poder correr el programa.

5.-Se especifica lo que se tiene que imprimir mediante la tabla de atributos del ejido.

6.- Al poner la condición en el programa en Python se denominará dependiendo de los grados el cultivo para lo cual es buena esa área, ya sea agrícola o de agricultura.

7.- Se espera que el mapa a realizar junto con el programa señale con diferentes colores las diferentes pendientes las cuales puedan ser de buena utilidad.

# Manejo de Datos

El tipo de datos que se manejan en el programa son:

Datos geoespaciales: son requeridos para la localización de las curvas de nivel del ejido y el sistema de referenciación.

Lenguaje de programación: para lograr crear el programa y este ejecute correctamente lo que se pide.

Sistemas de Información Geográfica: los SIG importantes para el desarrollo de la localización de cada zona apta para el cultivo.

1.1. 	Sistema Operativo
El programa está diseñado para trabajar en el Sistema Operativo Windows. 

1.2. 	Equipo de prueba
El equipo en el cual fue probado el programa es una computadora portátil de la marca Hp pavilion con las siguientes características:

![PalabrasdelTextoAlternativo](https://github.com/Alejandro480/Pendientes-del-Ejido-la-Esperanza/blob/master/Especificaciones.png)

# Resultados

Lo que se logró obtener con el código fue un programa en el cual se extraen desde uns archivo xlsx los diferentes ángulos de las   pendientes  que tiene nuestro ejido para obtener las pendientes que son recomendables a este tipo de casos y que se pueda usar en  ámbito de la agricultura.

En el siguiente código se producen desde el Angulo mínimo  hasta el ángulo máximo 

![PalabrasdelTextoAlternativo](https://github.com/Alejandro480/Pendientes-del-Ejido-la-Esperanza/blob/master/Tabla.png)

Con la tabla mostrada anteriormente, generamos una grafica de pastel en la que se pudem observar las diferentes pendientes que existen en el Ejido la Esperanza

![PalabrasdelTextoAlternativo](https://github.com/Alejandro480/Pendientes-del-Ejido-la-Esperanza/blob/master/Grafica.png)

Este es el codigo que se utilizo

    import openpyxl
    
    import PIL

ELE es abreviación de Ejido La Esperanza

    doc = openpyxl.lod_workbook("ELE")

    selecciom = hoja['B2':'D5']

    for fials in seleccion:

        for columnas in filas:
    
            print (columnas.coordinate, columnas.valie)
        
        print ("---Final de Fila---")
 
Si desea ver la imagen del area de estudio indique "y"

    run = raw_input("Decea ver el Ejido de estudio y/n\n")

    from PIL import Image

Para que la imagen pudea ser mostradra debera de indicarse con el nombre de la imagen

    def show(path_name):

        image = ()
    
    image.open(path_name)=

        image.show()
    
    show()
    
# Conclusiones

González Dimas Mario Humberto:

En conclusión, puedo asumir que el cálculo de pendientes en este proyecto es importante para los ejidatarios de esa comunidad, poder conocer las condiciones aptas para el cultivo de maíz y calla es importante para la producción agrícola.

Hernández Hernández Juan David:

Por mi parte coincido con lo mencionado anteriormente el código de este programa en sí permite plasmar las pendientes del lugar, que en este caso fue el ejido la esperanza. Puede que parezca algo ilógico para las personas hablar de pendientes, pero en el mapa base creado, gráficamente el espectador puede observar claramente la pendiente correspondiente.

Ramírez Serratos Alejandro:

Al principio el proyecto y la creación del programa resultó difícil además las librerías necesarias e instalación resultaron igual.
Con las pendientes podemos ayudar y contribuir a los nuevos agricultores a elegir mejor sus áreas de cultivo. Como proyecto me parece satisfactorio porque es lo que queríamos realizar desde un principio. 

# Referencias

 https://www.inegi.org.mx/app/mapas/
 https://www.arcgis.com
 
 POSTER DE REPRESENTACION DEL PROYECTO
 
![PalabrasdelTextoAlternativo](https://github.com/Alejandro480/Pendientes-del-Ejido-la-Esperanza/blob/master/POSTER%20PENDIENTES.jpg)
