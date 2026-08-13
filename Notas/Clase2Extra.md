# de donde sale el 140mm para la formula del poder de resolucion

El número 140 que aparece en la fórmula del poder de resolución de un telescopio proviene de la física óptica, específicamente de la simplificación de la fórmula del límite de Dawes para la luz visible.
Aquí te explico detalladamente de dónde sale este valor paso a paso:
## 1. La base científica (El criterio de Rayleigh)
En física, la capacidad de un telescopio para separar dos objetos muy juntos (como estrellas binarias) está limitada por la difracción de la luz. La fórmula matemática teórica es el Criterio de Rayleigh:
$$\theta = 1.22 \times \frac{\lambda}{D}$$ 

* $\theta$: Ángulo de resolución en radianes.
* $\lambda$: Longitud de onda de la luz.
* $D$: Diámetro de la apertura del telescopio. [1, 2, 3] 

## 2. Conversión a unidades prácticas
Para que los astrónomos puedan usar la fórmula fácilmente en el mundo real, se realizan los siguientes cambios:

* Se convierte el ángulo $\theta$ de radianes a segundos de arco (arcosegundos).
* Se establece la longitud de onda ($\lambda$) en un promedio de 550 nanómetros (la luz verde-amarilla, que es donde el ojo humano es más sensible).
* Se mide la apertura ($D$) en milímetros.

Al calcular matemáticamente esa constante teórica con estos cambios, el resultado es aproximadamente 138.
## 3. El ajuste empírico (El límite de Dawes)
En el siglo XIX, el astrónomo británico W. R. Dawes realizó experimentos visuales reales con telescopios y estrellas binarias de brillo similar.
Él descubrió que el ojo humano, al observar estrellas, podía distinguir la separación un poco antes de lo que decía la teoría estricta de Rayleigh. Ajustó la fórmula basándose en sus observaciones prácticas y estableció que la constante ideal es 115.8 si el diámetro está en milímetros.
## 4. ¿Por qué se usa el 140 entonces?
El número 140 es una versión ligeramente más conservadora y realista que se utiliza hoy en día por dos razones principales:

* Calidad de la atmósfera: El límite de Dawes (116) asume condiciones atmosféricas perfectas y un espacio ideal. El valor 140 compensa las turbulencias normales del aire (el seeing atmosférico).
* Facilidad de cálculo: Para la óptica práctica y comercial, la fórmula simplificada quedó establecida como:

$$R = \frac{140}{D}$$ 
Donde $R$ es la resolución en segundos de arco y $D$ es la apertura en milímetros. Si prefieres usar pulgadas para el diámetro, la constante cambia a 5.5 ($R = 5.5 / D$).
------------------------------
Si estás calculando la resolución de un equipo específico, ¿me podrías compartir el diámetro de la apertura de tu telescopio? Con ese dato puedo ayudarte a calcular su poder de resolución exacto y explicarte qué tipo de detalles u objetos podrías llegar a ver con él.

[1] [https://www.tarmacview.com](https://www.tarmacview.com/es/glossary/angular-resolution/)
[2] [https://chineselens.com](https://chineselens.com/es/understanding-numerical-aperture/)
[3] [https://es.wikipedia.org](https://es.wikipedia.org/wiki/Resoluci%C3%B3n_%C3%B3ptica)


# 44' Júpiter tamaño angular, tengo f = 1000, cómo se sabe que el tamaño lineal es s=0.21

Para calcular el tamaño lineal ($s$) de la imagen de Júpiter que se forma en el plano focal de tu telescopio, se utiliza la fórmula del tamaño de la imagen para ángulos pequeños.
Aquí te muestro el paso a paso matemático de cómo se llega a esos 0.21 mm:
## 1. La Fórmula Fundamental
Cuando un objeto astronómico tiene un tamaño angular $\theta$, el tamaño de su imagen en el plano focal depende directamente de la distancia focal ($f$) del telescopio:
$$s = f \cdot \tan(\theta)$$ 
Como el ángulo de Júpiter es extremadamente pequeño (medido en segundos de arco), podemos usar la aproximación de ángulo pequeño, donde $\tan(\theta) \approx \theta$ (siempre que $\theta$ esté expresado en radianes):
$$s = f \cdot \theta_{\text{radianes}}$$ 
------------------------------
## 2. Convertir el ángulo a Radianes
Tu dato es $\theta = 44''$ (segundos de arco). Para pasarlo a radianes, debemos recordar que:

* $1^{\circ} = 3600''$ (segundos de arco).
* $1 \text{ radián} \approx 206,265''$. [1] 

Hacemos la conversión:
$$\theta_{\text{radianes}} = \frac{44''}{206,265} \approx 0.0002133 \text{ radianes}$$ 
------------------------------
## 3. Calcular el Tamaño Lineal ($s$)
Ahora multiplicamos este ángulo en radianes por la distancia focal de tu telescopio ($f = 1000 \text{ mm}$):
$$s = 1000 \text{ mm} \cdot 0.0002133 \text{ rad}$$ 
$$s \approx 0.2133 \text{ mm}$$ 
Redondeando a dos decimales, obtienes exactamente 0.21 mm.
------------------------------
## En resumen
Ese 0.21 mm es el tamaño real (físico) que medirá el disco de Júpiter si colocaras una regla o un sensor de cámara digital directamente en el foco de tu telescopio de 1000 mm de focal.
Si te interesa la astrofotografía, ¿quieres saber cuántos píxeles ocuparía Júpiter en el sensor de tu cámara actual con esa distancia focal?

[1] [https://www.astronomia.edu.uy](http://www.astronomia.edu.uy/CTE2/campoprofundo.pdf)

# Calcular F0V_{70mm}, sabiendo que FoV=AFoV/m y AFoV=50deg

El campo visual real para un ocular de 70 mm es de $3.5^{\circ}$ (grados).
Para llegar a este resultado utilizando la relación con tu telescopio anterior de distancia focal ($f = 1000 \text{ mm}$), realizamos los siguientes pasos:
## 1. Calcular la Magnificación ($m$)
La magnificación o aumento del telescopio se obtiene dividiendo la distancia focal del telescopio entre la distancia focal del ocular ($70 \text{ mm}$):
$$m = \frac{f_{\text{telescopio}}}{f_{\text{ocular}}} = \frac{1000 \text{ mm}}{70 \text{ mm}} \approx \mathbf{14.29 \times}$$ 
## 2. Calcular el Campo Visual Real ($FoV$)
Aplicamos la fórmula que proporcionaste usando el Campo Visual Aparente ($AFoV = 50^{\circ}$):
$$FoV = \frac{AFoV}{m} = \frac{50^{\circ}}{14.2857} = \mathbf{3.5^{\circ}}$$ 
------------------------------
## ¿Qué significa este resultado?
Un campo visual de $3.5^{\circ}$ es sumamente amplio en astronomía. Como referencia, la Luna llena mide aproximadamente $0.5^{\circ}$ de diámetro, lo que significa que podrías alinear unas 7 Lunas llenas una al lado de la otra dentro de lo que ves por este ocular. [1] 
¿Te gustaría calcular cuántos minutos de arco representa este campo o verificar si un ocular de 70 mm causaría problemas de pupila de salida con tu telescopio?

f_telescope = 1000f_eyepiece = 70AFoV = 50
m = f_telescope / f_eyepieceFoV = AFoV / m
print(f"m = {m}")
print(f"FoV = {FoV}")


[1] [https://www.saracco.com](https://www.saracco.com/2012/11/20/telescopios-2/)


# CCD= [4,80\times3,6]mm, Cuanto es FoV_x

El campo visual horizontal ($FoV_x$) para tu sensor CCD de $4.80 \text{ mm}$ en un telescopio de $f = 1000 \text{ mm}$ es de $16.5$ minutos de arco (aproximadamente $0.275^{\circ}$).
Para calcular el campo visual de un sensor de cámara (en astrofotografía de foco primario), se utiliza la trigonometría básica. Aquí tienes el paso a paso:
## 1. La Fórmula del FoV para Sensores
El campo visual de un sensor se calcula de forma independiente para su eje X (horizontal) y su eje Y (vertical) usando la dimensión del chip y la distancia focal ($f$):
$$FoV_x = 2 \cdot \arctan\left(\frac{\text{Ancho del sensor}}{2 \cdot f}\right)$$ 
------------------------------
## 2. Cálculo en Grados
Sustituimos el ancho del sensor ($4.80 \text{ mm}$) y la focal ($1000 \text{ mm}$):
$$FoV_x = 2 \cdot \arctan\left(\frac{4.80}{2000}\right)$$ 
$$FoV_x = 2 \cdot \arctan(0.0024)$$ 
Utilizando la aproximación para ángulos pequeños (donde $\arctan(x) \approx x$ en radianes):
$$FoV_x \approx 2 \cdot 0.0024 = 0.0048 \text{ radianes}$$ 
Convertimos los radianes a grados multiplicando por $\frac{180}{\pi}$ (o por $57.2958$):
$$FoV_x = 0.0048 \cdot 57.2958 \approx \mathbf{0.275^{\circ}}$$ 
------------------------------
## 3. Conversión a Minutos de Arco ($'$)
Como el valor en grados es menor a 1, en astronomía es mucho más práctico expresarlo en minutos de arco (sabiendo que $1^{\circ} = 60'$):
$$FoV_x = 0.275^{\circ} \cdot 60 \approx \mathbf{16.5'}$$ 
------------------------------
## En perspectiva (Comparación con Júpiter)
En tus preguntas anteriores vimos que Júpiter mide $44''$ ($0.73'$) de tamaño angular. Como tu sensor cubre $16.5'$ de cielo horizontalmente, Júpiter cabrá perfectamente en la foto y ocupará aproximadamente el 4.4% del ancho total de la imagen.
¿Te gustaría calcular también el $FoV_y$ (vertical) para tener el encuadre completo, o conocer la escala de placa en arcosegundos por píxel si me das la resolución de tu cámara?

