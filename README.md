# Estimador Ingresos Bogota
Herramienta analítica para estimación de ingresos en hogares en la ciudad de Bogota

## Preparación de la herramienta

### Requisitos
Python 3.8 o superior.
Anaconda.

### Librerías necesarias
- [x] folium
- [x] warnings
- [x] pandas
- [x] geopandas
- [x] zipfile
- [x] shutil
- [x] numpy
- [x] datetime
- [x] os
- [x] shapely.geometry
- [x] re

## Uso de la herramienta

### Primera vez.

Luego de instalado el python y las librerias que se listaron anteriormente se debe descomprimir el archivo [Estimador_Ingresos.rar](https://github.com/lilianahernandezroa/EstimadorIngresosBogota/blob/main/Estimador_Ingresos.rar), la carpeta debe verse así:

![Carpeta herramienta](https://github.com/lilianahernandezroa/EstimadorIngresosBogota/blob/main/1_Preparacion.jpg)

### 1. Listado de direcciones.

En el archivo [DireccionesClientes.csv](https://github.com/lilianahernandezroa/EstimadorIngresosBogota/blob/main/Estimador_Ingresos.rar) se encuentran los campos Cliente_ID y DIRECCION, en el archivo de ejemplo se incluye un listado con 1027 direcciones de colegios de la ciudad de Bogotá:

![Direcciones](https://github.com/lilianahernandezroa/EstimadorIngresosBogota/blob/main/1_Insumo.jpg)

#### NOTA. Este archivo es un csv separado por punto y coma, debe mantenerse esa estructura, además, dentro de las direcciones no debe estar ese carácter para evitar corrimientos y errores con la geolocalización.

### 2. Ejecución.
Dentro de la misma carpeta, se encuentra el cuaderno de jupyter [Ingresos_Clientes.ipynb](https://github.com/lilianahernandezroa/EstimadorIngresosBogota/blob/main/Estimador_Ingresos.rar), para su ejecución es necesario ejecutar Anaconda ingresando las siguientes instrucciones:

```bat
cd "ruta ejecutable"
jupyter notebook
```

![Anaconda](https://github.com/lilianahernandezroa/EstimadorIngresosBogota/blob/main/2_Ejecucion_Anaconda.jpg)

Seguido a esto se debe abrir en un navegador la siguiente ventana, por favor abrir el archivo resaltado en amarillo:
![Estimador](https://github.com/lilianahernandezroa/EstimadorIngresosBogota/blob/main/2_Ejecucion_Estimador.jpg)

Para ejecutar la herramienta se hace click en la opción que se resalta en amarillo:
![Jupyter](https://github.com/lilianahernandezroa/EstimadorIngresosBogota/blob/main/2_Ejecucion_jupyter.jpg)

### 3. Resultados.

Luego de finalizada la ejecución, en la carpeta Entregable, encontrara una carpeta con la fecha y hora de ejecución, dentro está un archivo CSV con todas las direcciones que fueron ingresadas junto con el mapa como se muestra a continuación:

![Entregable](https://github.com/lilianahernandezroa/EstimadorIngresosBogota/blob/main/3_Entregables.jpg)

#### Datos clientes
En el archivo DatosClientes.csv se encuentra cada una de las direcciones ingresadas con el resultado de la geolocalización y una observación para las direcciones que no pudieron ser georeferenciadas en Bogotá:

![Datos clientes](https://github.com/lilianahernandezroa/EstimadorIngresosBogota/blob/main/3_DatosClientes.jpg)

#### Mapa con la geolocalización

![Mapa](https://github.com/lilianahernandezroa/EstimadorIngresosBogota/blob/main/3_mapa.jpg)



> Elaborado por Liliana Hernandez Roa y Oscar Pachon Triana, Junio 2023
