# [[ANÁLISIS MATEMÁTICO I]] 
---
# TEMA 4: CONTINUIDAD I, LÍMITE DE FUNCIONES  

## Límite de funciones en R

__¿Cómo se interpreta? (Gráficamente)__

[ADJUNTAR FOTO FUNCION PARTIDA DE EJEMPLO]

__¿Cuál es la aplicación?__
Nos permite detectar (cuando logremos calcular el límite utilizando solo la fórmula) tanto la _continuidad cómo también la ausencia de la misma (ya sea por un salto o por una asíntota vertical)._

__¿Cómo se calcula?__
- Gráfico: Observar cómo se comporta la continuidad de dicha función en ciertos puntos de la gráfica.
- Fórmula: Para calcular un límite la estrategia básica es remplazar los valores de x, de esta manera analizamos los valores de salida en puntos críticos de la función.

Ejemplo, veamos cómo hacerlo de las dos maneras:
$f(x)=[-2-x²,~si~x \leq{0}]$  y $f(x)=1+x, ~si~x>0$.
Analizamos el límite de $f(x)$ por izquierda ($0⁻$), para ello, vemos las condiciones de la función partida y esto nos indica que tomemos la primer fórmula.
Remplazamos, $f(x)=-2-0⁻^²\approx-2$. Con esto ya tenemos un valor de referencia para la función por izquierda.
Luego, buscamos analizar el límite de $f(x)$ por derecha ($0⁺$), ahora utilizamos la segunda fórmula y remplazamos: $f(x)=1+0⁺\approx1$.
A paritr de estos valores de referencia, podemos confirmar que la función no tiene continuidad cuando se aproxima a 0, y más específicamente podemos afirmar que hubo un salto debido a que estos valores son finitos.
![[Pasted image 20220914150826.png]]

---

### Estrategia para resolver indeterminación $\frac{0}{0}$ (Cociente de polinomios).
Se resuelve por medio de Ruffini para factorizar.
[INVESTIGAR]

Nota: Discontinuidad en el cambio.
Si existe el $límite~x\rightarrow x_0$ de $f(x)=L$, pero $x_{0} \notin Dom(f)$, diremos que en tal caso $f$ tiene una discontinuidad “evitable” en $x_0$.
¿Cómo se interpreta gráficamente?
Graficamos la hipérbola, por lo que buscamos la asíntota vertical y la asíntota horizontal y las raíces.
[ADJUNTAR FOTO GRÁFICA HIPÉRBOLA]

#### Conversión por multiplicación de conjugados
Tengamos por ejemplo el cálculo del siguiente límite 
$$lím~x\rightarrow1=\frac{4-4\sqrt{x}}{\sqrt{3+x}-2}$$
Multiplicamos por el conjugado de tanto el numerador como el denominador, $$\frac{(4-4\sqrt{x})(4+4\sqrt{x})*(\sqrt{3+x}+2)}{(4+4\sqrt{x})*(\sqrt{3+x}-2)(\sqrt{3+x}+2)}$$
Distrbuímos y nos queda $$\frac{(16-16x)(\sqrt{3+x}+2)}{(3+x-4)(4+4\sqrt{x})}$$
Factorizamos y simplificamos los términos $(x-1)$ 
$$\frac{-16(x-1)}{(x-1)}*\frac{(\sqrt{3+x}+2)}{(4+4\sqrt{x})}$$
Habiendo reconvertido la expresión nos queda que
$$\frac{4-4\sqrt{x}}{\sqrt{3+x}-2}=\frac{-16(\sqrt{3+x}+2)}{4+4\sqrt{x}}$$

---
#### Asíntota horizontal
[INVESTIGAR]

---
#### Pequeñas oscilaciones
__Para resolver indeterminaciones con funciones trigonométricas.__
Ejemplo básico de indeterminación: $$lím~x\rightarrow 0~ \frac{sen(x)}{x}=\varnothing$$
Esto se debe a que el $sen(x)\approx x$ para $x\approx 0$.

Ejemplo de práctica: $$tan(x)=\frac{sen(x)}{cos(x)}\Rightarrow \frac{x}{tan(x)}=\frac{x}{\frac{sen(x)}{cos(x)}}=\frac{x*cos(x)}{sen(x)}=\frac{cos(x)}{\frac{sen(x)}{x}}$$
De este modo hallamos la indeterminación.

Otro ejemplo de indeterminación puede ser $$lím~x\rightarrow \pi~ \frac{sen(x)}{-x+\pi}=\varnothing$$
Esto se debe a que el $sen(\pi)=0$, por lo que al aproximar $x$ a $\pi$ quedaría $\frac{0}{0}$.
$$\frac{sen(x)}{-x+\pi}=\frac{sen(x-\pi+\pi)}{-(x-\pi)}$$
[INVESTIGAR LO Q ME FALTA XD]
