------------------------------------------------------------------------

------------------------------------------------------------------------

# PBRs\_Erizo

Este repositorio contiene los análisis realizados para el cálculo de PBRs para las unidades de stock del Erizo.

**Descripción del contenido de la carpeta "codigos\_admb"**

El código base corresponde a un Modelo de Captura a la talla ("Modbento") creado por cristian.canales\@ifop.cl. Los códigos utilizados para este estudio corresponde a una modificación del "Modbento". Esta modificación es realizada por mariajose.zuniga\@ifop.cl y mauricio.mardones\@ifop.cl se detallará a continuación.

Contiene los códigos de ADMB principalmente MAET.tpl y MAET.dat del modelo de evaluación de stock de erizo de la zona X Norte (MAETXN) , X Sur (MAETXS) y XI (MAETXI).

Los modelos corresponden a modelos anuales (año calendario) con dinámica a la edad e información en tallas (utiliza matriz de probabilidad edad\_talla).

Los principales datos que ingresan al modelo corresponden a los desembarques, CPUE y frecuencia de tallas de la flota. Utiliza un vector de pesos medios a la talla, madurez a la talla, y parámetros de crecimiento y mortalidad natural.

## 
