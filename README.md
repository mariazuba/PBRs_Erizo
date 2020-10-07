------------------------------------------------------------------------

------------------------------------------------------------------------

# PBRs\_Erizo

Este repositorio contiene los análisis realizados para el cálculo de PBRs para las unidades de stock del Erizo.

**Descripción del contenido de la carpeta "codigos\_admb"**

El código base corresponde a un Modelo de Captura a la talla ("Modbento") creado por cristian.canales\@ifop.cl. Los códigos utilizados para este estudio corresponde a una modificación del "Modbento". Esta modificación es realizada por mariajose.zuniga\@ifop.cl y se detallará a continuación.

Contiene los códigos de ADMB principalmente MAET.tpl y MAET.dat del modelo de evaluación de stock de erizo de la zona X Norte (MAETXN) , X Sur (MAETXS) y XI (MAETXI).

Los modelos corresponden a modelos anuales (año calendario) con dinámica a la edad e información en tallas (utiliza matriz de probabilidad edad\_talla).

Los principales datos que ingresan al modelo corresponden a los desembarques, CPUE y frecuencia de tallas de la flota. Utiliza un vector de pesos medios a la talla, madurez a la talla, y parámetros de crecimiento y mortalidad natural.

## **Descripción del archivo de datos y controles (.dat)**

**Datos de entrada**

**nanos** =número de años

**nedades**=número de edades a modelar

**edad\_min**=edad mínima

**ntallas**=número de clases/grupos de tallas

**Ind**=matriz de datos , desembarques, cv\_desem, CPUE, cv\_cpue, nm(tamaño de muestra)

**Tallas**=vector de tallas (clases/grupos de tallas)

**Frec\_Tallas**=matriz de frecuencia de tallas para los años de estudio

**Madurez**=vector de madurez a la talla

**Wmed**=vector de pesos medios a la talla

**Parámetros reclutamiento, períodos de desove y cpue, parámetros de crecimiento y mortalidad natural, stepness**

**sigmaR** =Coeficiente de variación de los reclutamientos

**dts**=dt desove NOVIEMBRE (Arias et al 1995 y Bay y Schmith (1981) y dt CPUE (Concentracion de la captura durante el año MES DE JULIO)

**Loo\_k\_Lo\_cv\_M**=PARAMETROS DE CRECIMIENTO Y MORTALIDAD NATURAL Loo k Lo(mm) cv(edad) M

**h**=h (pendiente de la relación S-R)

**PARAMETROS DE SELECTIVIDAD Y CAPTURABILIDAD**

**hiper\_estabilidad\_q** = coeficiente de hiper estabilidad de la CPUE (1=proporcional)

**Sel\_A50\_rango** = A50 y rango (A50= edad primera captura)

**nbloquesSel** = Número de bloques de selectividad

**ybloquesSel** = años de inicio de cada bloque de selectividad

**nbloquesq** = Número de bloques de capturabilidad

**ybloquesq** = años de inicio de cada bloque de capturabilidad

**FASES DE ESTIMACION DE PARAMETROS (valores negativos = no se estiman)**

**Fase\_q** = Estimacion del coeficiente de capturabilidad q (CPUE=q\*B\^b)

**Fase\_hiperestabilidad** = Estimacion parámetro de hiper estabilidad (b) de la CPUE

**Fase\_selectividad** = Estimacion de la selectividad

**Opt\_seldomo** = opción selectividad tipo domo

**Fase\_Lo** = Estimacion de Lo

**Fase\_cvLo** = Estimación cv(talla-edad)

**Fase\_F** = Estimación de la mortalidad por pesca

**Fase\_desvRt** = Estimacion variación anual de reclutamientos

**Fase\_No** = Estimacion condición inicial (si es \<0 esta en equilibrio)

**PROYECCION DE LA POBLACION**

**nmF =** número de multiplicadores de F

**mF** = multiplicadores de F

**nproy** = número de años a proyectar

**opt\_FRMS** = opción para utilizar Frms estimado por fuera (\>0 activado, \<0 desactivado)

**FRMS** = Frms estimado por fuera del modelo admb
