¿Qué hice en el proceso de solución de la práctica 3?

1. Fase de Peparación:
1.1 Inicializar
>iraf
>!ds9 &

1.2 Descompresión de archivos
cl > cd Documents
cl > mkdir ejercicio/intro
cl > cd ejercicio/intro
mv ../../Downloads/fintro0001 ../../Downloads/fintro0002 .
cl > unlearn rfits
cl > rfits fintro* "" junk old+
cl > dir

1.3 diferenciación de parámetros
cl > lpar imheader
cl > imhead im010
cl > imhead im010 longheader=yes | page
cl > epar imhead # Salir con :q
Poner yes en longheader. Cuidado con cómo se ingresa este 'yes', guardar cambios y salirse de esa parte interactiva.
cl  > lpar imead # Verificar cambios

---------------
REQUISITO DE ENTREGA #1 
---(En esta parte se responde adecuadamente a las preguntas. De manera concisa)---
Para el informe final, redacte una explicación formal sustentada físicamente sobre:
1. La diferencia operativa entre parámetros obligatorios (Query) y opcionales
(Hidden) descubierta en el Paso 1.3.
2. Justifique rigurosamente el uso del formato FITS en astrofísica, comparando
su capacidad de almacenar cabeceras con metadatos de ciencia legibles
frente a formatos de imagen de consumo masivo como .JPG o .PNG (enfoque
en la pérdida de datos y bits de profundidad).
2. Fase
-----------------

2. Fase imexamine
2.1 Visualización y parpadeo
cl > display im010 1
cl > display im011 2
En el panel de control de DS9, el Match LUTs, lo hacemos con la __¿barra de color, limites de color? y el modo Blink es el modo parpadeo, que nos sirve para ver de una manera más autónoma cuál es la diferencia entre la posición de las estrellas de la primera y segunda imágen.
Después de desactivar el parpadeo:

2.2 Medición de centroides con imexamine
cl > unlearn imexamine
cl > imexamine
Ahora estamos en modo interactivo con DS9

Para el diligenciamiento de los datos en la tabla, tenemos:
Hacer la tabla en latex
289.986 83.967 289.986 85.125
281.306 189.292 281.884 191.028
331.347 134.894 332.320 136.630
Con esto, ya calculamos el $\Delta{x}= X(im011) - X(im010)$ y $\Delta{y} =  Y(im011) - Y(im010)$

2.3 Aplicar el desplazamiento (imshift)
cl > unlearn imshift
cl > imshift im011 s011 ___ ___

-----------------------------------------
REQUISITO DE ENTREGA #2
Para el informe final, los estudiantes deberán entregar:
1. La Tabla de Alineamiento Estelar de imexamine completamente diligenciada
con los centroides medidos de las 3 estrellas de referencia y los deltas
promedio finales. (Esto es la tabla de arriba)
2. El comando exacto de imshift ejecutado en el Paso 2.3. (El comando se completa con los deltas obtenidos)
3. Captura de pantalla de DS9 en el modo 'Blink' mostrando la superposición
exitosa de im010 y s011 (con sus ejes de píxeles legibles) 

(el blink es el parpadeo, para no cargar mucho el documento de latex mientras trabajo, se agregan las imágenes pero con el símbolo '\%' para que al compilar no se tenga en cuenta, luego yo le quito el símbolo para que funcione. Aquí, las imágenes se llaman 'Blink1.jpg' y 'Blink2.jpg')
-----------------------------------------

3. Análisis matemático y estadísticas comparativas
3.1 Promediar usando imsum
cl > unlearn imsum
cl > imsum im010, s011 aver1 pixt=r calct=r option=average v+
3.2 Promediar usando imarith
cl >




