# PBRs\_Erizo

Este repositorio contiene los análisis realizados para el cálculo de PBRs para las unidades de stock del Erizo. \#	MODELO	DE	CAPTURA	A	LA	TALLA	(MODBENTO)	IFOP	cristian.canales\@ifop.cl																																							 El modelo utilizado corresponde a Modbento modificado por mariajose.zuniga\@ifop.cl

**Descripción del contenido**

1.  codigos\_admb: contiene los códigos de ADMB principalmente MAET.tpl y MAET.dat del modelo de evaluación de stock de erizo de la zona X Norte (MAETXN) , X Sur (MAETXS) y XI (MAETXI). Los modelos corresponden a modelos anuales (año calendario) con dinámica a la edad e información en tallas (utiliza matriz de probabilidad edad\_talla). Los principales datos que ingresan al modelo corresponden a los desembarques, CPUE y frecuencia de tallas de la flota. Utiliza un vector de pesos medios a la talla, madurez a la talla, y parámetros de crecimiento y mortalidad natural.

## **Descripción del .dat**

### **Datos de entrada**

-    "nanos" = número de años

-   "nedades" = número de edades a modelar

-    "edad\_min" = edad mínima

-   "ntallas" = número de clases/grupos de tallas

-    "Ind" = matriz de datos , desembarques, cv\_desem, CPUE, cv\_cpue, nm(tamaño de muestra)

-   "Tallas" = vector de tallas (clases/grupos de tallas)

-    "Frec\_Tallas" = matriz de frecuencia de tallas para los años de estudio

-    "Madurez" = vector de madurez a la talla

-    
 "Wmed" = vector de pesos medios a la talla

### Controles

-    "sigmaR" = Coeficiente de variación de los reclutamientos

-    "dts" = dt desove NOVIEMBRE (Arias et al 1995 y Bay y Schmith (1981) y dt CPUE (Concentracion de la captura durante el año MES DE JULIO)

-    "Loo\_k\_Lo\_cv\_M" = PARAMETROS	DE	CRECIMIENTO	Y	MORTALIDAD	NATURAL Loo	k	Lo(mm)	cv(edad)	M	

-    
 "h" = h (pendiente de la relación S-R)

-    "hiper\_estabilidad\_q" = coeficiente de hiper estabilidad de la CPUE (1=proporcional)

    **PARAMETROS DE SELECTIVIDAD**

-   "Sel\_A50\_rango" = A50 , rango (A50= edad primera captura)

-    "nbloquesSel" = Número de bloques de selectividad

-    
"ybloquesSel" = años de inicio de los bloques de selectividad

-    "nbloquesq" = Número de bloques de capturabilidad

-    "ybloquesq" = años de inicio

    ### Fases de estimación

-    "Fase\_q"

-   "Fase\_hiperestabilidad"

-   "Fase\_selectividad"

-   "Opt\_seldomo"

-    "Fase\_Lo"

-    
"Fase\_cvLo"

-    "Fase\_F"

-    "Fase\_desvRt"

-    "Fase\_No"

    #### Proyección      

-    
"nmf" = número de multiplicadores de F

-    "mF" = multiplicadores de F

-   "nproy" = número de años a proyectar

-   "opt\_FMRS" = opción para utilizar Frms estimado por fuera (\>0 activado, \<0 desactivado)

-    
"FMRS" = Frms estimado por fuera del modelo admb
