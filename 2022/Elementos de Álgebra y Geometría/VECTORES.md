# [[ELEMENTOS DE ÁLGEBRA Y GEOMETRÍA]] 

---
# TEMA 10: Vectores

# 1. Coordenadas
En el plano, un punto P se puede representar mediante un par ordenado de números reales (a1, a2 ), llamados las coordenadas cartesianas de P, de la siguiente forma. Elegimos dos lı́neas perpendiculares que llamamos eje x y eje y, que se cruzan en un punto que recibe el nombre de origen. Trazamos lı́neas perpendiculares desde P a los ejes. Eligiendo unidades de medida en estos ejes, y eligiendo cuál será el sentido positivo en cada uno, producimos los números a1 y a2 “leyéndolos” sobre los ejes. El origen tendrá entonces coordenadas (0, 0). El sentido positivo se indica en el diagrama con una flecha en el eje.

![[Pasted image 20221006092802.png]]
Para el espacio tridimensional, hacemos algo parecido. Elegimos un punto que llamamos el origen, y tres lı́neas perpendiculares entre sı́ y que pasen por dicho punto, con unidades de medida y un sentido elegido como positivo. Leemos las coordenadas (a1 , a2, a3 ) como indica la figura siguiente. Es usual en los diagramas representar el eje z hacia arriba y los ejes x e y “apoyados en el suelo”.
![[Pasted image 20221006092929.png]]

# 2. Primeras operaciones algebraicas
La suma y el producto por escalares en $\mathbb{R²}$ y $\mathbb{R³}$ se definen en forma similar a lo que hicimos con matrices, es decir, componente a componente. Por ejemplo, con esas definiciones tendrı́amos:
- $(1, 3) + (−1, 7) = (0, 10)$
- $α(1 + p, q, r2 ) = (α + αp, αq, αr 2) \ si \ α ∈ \mathbb{R}$
  
Tienen las mismas propiedades que las respectivas operaciones de matrices, por ejemplo, las que nos permiten escribir (α + β)(x, y, z) = α(x, y, z) + β(x, y, z).

# 3. Vectores e interpretación geométrica de las operaciones
Vamos a dar una definición preliminar de la noción de vector. Definimos un vector como un segmento de lı́nea dirigido con punto inicial en el origen, es decir, un segmento con una dirección, sentido y magnitud (longitud) especificados, y punto inicial en el origen. Se puede representar mediante una flecha que parte del origen, como en la figura siguiente. Tipográficamente, se representa como una letra en negrita, o con una flecha arriba, o con una línea debajo o incluso sin ningún indicador especial: a, ~a, a, a. También se acostumbra usar letras cercanas a la v en el alfabeto: u, v, w. Para escritura a mano, es más cómodo escribir los vectores con flechas: ~a, ~v.

![[Pasted image 20221006094151.png]]

Esta definición funciona tanto en el plano como en el espacio. Escribiremos lo siguiente pensando que estamos trabajando en el espacio, y en el plano simplemente habrá que usar pares en vez de ternas. Usando esta definición, podemos asociar a cada vector a el punto $(a_{2} , a_{2} , a_{3})$ donde a termina (es decir, las coordenadas de la punta de la flecha). Recíprocamente, a cada punto $(a_{2} , a_{2} , a_{3})$ del espacio le hacemos corresponder el vector a que será una flecha desde el origen hasta dicho punto. Así, identificaremos a con $(a_{2} , a_{2} , a_{3})$ y escribiremos $a = (a_{1} , a_{2}, a_{3} )$.
$$\begin{equation}
a= \begin{bmatrix} 1 \\ 2  \end{bmatrix}, v=\begin{bmatrix} 0 \\ 2\end{bmatrix} 
\end{equation}$$

Sin embargo, por comodidad en la escritura seguiremos usando la notación $a = (1, 2)$, $v=(0, −1, 5)$ por ahora.

## Suma de vectores
Definimos la suma de vectores (pensados como flechas) con la llamada regla del paralelogramo, como sigue. Para sumar los vectores $a = (a_{1} , a_{2}, a_{3} )$ y $b = (b_{1} , b_{2} , b_{3})$ consideramos el paralelogramo que tiene $a$ y $b$ como lados adyacentes (ver figura 1). La suma $a + b$ se define como el vector que va a lo largo de la diagonal.
![[Pasted image 20221006095448.png]]
Muy importante: afortunadamente, las componentes de este vector $a + b$ resultan ser $(a_{1}  + b_{1}, a_{2} + b_{2}, a_{3} + b_{3} )$, que es precisamente el resultado de sumar las ternas correspondientes a los vectores a y b. No es difícil de probar pero no lo demostraremos aquí.
Resumiendo, tenemos dos tipos de objetos: unos algebraicos (ternas de números) y otros geométricos (vectores como flechas). Definimos cómo sumar los objetos algebraicos (componente a componente) y cómo sumar los geométricos (regla del paralelogramo). También dimos una forma de “traducir” un vector a una terna y viceversa. Lo que nos dice la observación de recién es que es lo mismo sumar los vectores y luego traducir el resultado a una terna, que traducir primero a ternas y después sumar.

## Producto de un escalar por un vector
El producto de un escalar por un vector también tiene una descripción geométrica. Si $λ$ (lambda) es un escalar (es decir, un número real) y a es un vector, se define $λa$ como sigue:
- Si $λ > 0$, entonces λa tiene la misma dirección y sentido que a, pero su longitud se multiplica por λ.
- Si $λ < 0$, entonces λa tiene sentido opuesto al de a, y su longitud se multiplica por |λ| (por ejemplo, −2a medirá el doble que a).
- Si $λ = 0$, entonces $λa = 0$.
A decir verdad, si $a = 0$ la descripción anterior no se puede aplicar literalmente (porque no se le asigna dirección ni sentido), pero simplemente es $λ \ne 0$ para todo $λ ∈ \mathbb{R}$.
![[Pasted image 20221006095916.png]]
Del lado algebraico, como ternas, será simplemente $λa = (λa_{1}, λa_{2}, λa_{3})$, es decir, esta multiplicación de un escalar por un vector se corresponde con la multiplicación de un escalar por una terna.

## Diferencia de vectores
La diferencia de vectores se calcula ası́: $a − b = a + (−1)b$. Es decir, invertimos el sentido de $b$ y se lo sumamos a $a$. **Algebraicamente es restar componente a componente.**

---
*Comentario. Una aclaración sobre los términos “dirección” y “sentido”. Imaginemos un plano de una ciudad perfectamente cuadriculada donde hay calles verticales (Norte-Sur) y calles horizontales (Este-Oeste). Decimos que las calles N-S tienen todas la misma dirección, y lo mismo con las E-O. Si tenemos dos autos yendo por dos calles N-S, uno hacia el N y el otro hacia el S, decimos que van en la misma dirección pero en sentido opuesto. Si hay un tercer auto que va por una calle E-O, decimos que va en una dirección diferente a los otros. No podemos comparar el sentido del tercer auto con el de los anteriores; para hablar de mismo sentido o sentido opuesto, es un prerrequisito tener la misma dirección.*

---
# 4. Vectores libres
Definimos a los vectores, también llamados vectores libres, como segmentos dirigidos en el plano o en el espacio (a diferencia de antes, no pedimos que partan del origen). Aquellos segmentos que se pueden obtener uno de otro mediante traslaciones paralelas (sin rotaciones) se consideran como el mismo vector.
![[Pasted image 20221011081412.png]]

Las componentes de un vector se obtienen de cualquiera de las siguientes formas.
- **Geométricamente:** trasladándolo de forma tal de que parta del origen y tomando las coordenadas del extremo final.
- **Algebraicamente:** Si el vector va del punto $P$ al punto $Q$, las componentes se calculan como las coordenadas de $Q$ menos las de $P$.
Por ejemplo, el vector que va de $P (5, 5)$ a $Q(7, 8)$ es $(2, 3)$. Se lo denota $\overrightarrow{PQ}$. Si denotamos al punto en el origen $(0, 0)$ con la letra $O$ y consideramos al punto $R(2, 3)$, resulta que $\overrightarrow{OR} = (2, 3) = \overrightarrow{PQ}$. Es decir, los extremos de las dos flechas son distintos, pero representan al mismo vector.

**La suma de vectores libres** se puede calcular como antes, es decir, trasladamos ambos vectores para que partan del origen, _consideramos el paralelogramo que forman y tomamos la diagonal del mismo_. Pero hay otra forma equivalente de ver una suma $a + b$. Trasladamos $b$ de forma que parta desde el extremo final de $a$, quedando ası́ uno a continuación del otro. **La suma aparecerá como el vector que va del extremo inicial de a al extremo final de b** (figura 2). Si invertimos los roles, colocando a a continuación de $b$, el vector que resultará será el mismo.
![[Pasted image 20221011082254.png]]

# 5. Módulo
**El módulo de un vector $a$ es su longitud**. Se denota $\|a\|$, y es un número real no negativo, aunque puede dar $0$, pero sólo en el caso de que a sea el vector nulo.
En el plano, si $a=(a_{1}, a_{2})$, usando el teorema de Pitágoras se tienen $\|a\| = \sqrt{a^2_{1}+a²_{2}}$.  En el espacio, si $a = (a_{1} , a_{2}, a_{3} )$ entonces $\|a\| = \sqrt{a^2_{1}+a²_{2}+a²_{3} }$. En realidad estas fórmulas son válidas si elegimos ejes que sean perpendiculares entre sı́ y con la misma unidad de medida, quedando el módulo expresado en esa misma unidad de medida. Existen situaciones donde esto no es ası́.
Observemos, de la definición de producto por un escalar, que $\|\lambda a\| = |\lambda| \|a\|$. Es decir, los escalares “salen” del módulo, pero en valor absoluto.
Un vector de módulo 1 recibe el nombre de vector unitario. Notemos que **podemos “transformar” cualquier vector no nulo en uno unitario dividiéndolo por su módulo**. Esto es, si $a \neq 0$, entonces $a/\|a\|$ tiene la misma dirección y sentido que $a$, y módulo $1$. Este proceso se llama normalizar el vector $a$.

# 6. Base estandar de vectores
Una vez elegido un sistema de coordenadas, es conveniente definir tres vectores particulares a lo largo de los ejes x, y, z:
$$i=(1,0,0); j=(0,1,0); k=(0,0,1)$$
Estos forman la llamada base standard de vectores (figura 3). También se los denota a veces $e_{1}, e_{2}, e_{3}$. En el plano, tendremos una componente menos y un vector menos: $i = (1, 0)$, $j = (0, 1)$.
![[Pasted image 20221011083933.png]]
Sea $a=(a_{1}, a_{2}, a_{3})$ cualquier vector. Entonces $a = a_{1}i + a_{2}j + a_{3}k$, ya que desarrolando se obtiene $$a_{1}i + a2 j + a3 k = a1 (1, 0, 0) + a2 (0, 1, 0) + a3 (0, 0, 1) = (a1 , a2, a3 )$$

---
# 8.

---
# 9.

---
# 10. Producto mixto o producto triple

Hay una operación entre tres vectores que combina un producto escalar con un producto vectorial. Por su importancia, recibe una denominación propia, que es la de producto mixto o triple. 
El producto mixto de tres vectores en el espacio a, b y c (en ese orden) es (a × b) · c. Una forma fácil de hacer esta operación, sin necesidad de hacer las dos operaciones en forma sucesiva, es poner a, b y c como filas en un determinante de 3 × 3: 
$$(a\times b)\cdot c \begin{bmatrix}
a_{1} & a_{2} & a_{3} \\ 
b_{1} & b_{2} & b_{3} \\ 
c_{1} & c_{2} & c_{3}
\end{bmatrix}$$

## Interpretación geométrica
El resultado del producto triple es un número real. Su valor absoluto es el volumen del paralelepı́pedo con aristas a, b y c, pensados con origen común: 
![[Pasted image 20221013081756.png]]
Además, su signo proporciona la siguiente información, ilustrada en la figura 7.
- Si (a × b) · c > 0, significa que si aplicamos la regla de la mano derecha a los vectores a y b, el vector c queda del mismo lado que el pulgar. No necesariamente son paralelos, sino que lo que estamos diciendo es que el vector c y el pulgar quedan del mismo lado del plano que contiene a a y b. Decimos que la terna de vectores a, b y c, en ese orden, tiene orientación positiva.
- Si (a × b) · c < 0, significa que si aplicamos la regla de la mano derecha a los vectores a y b, el vector c queda del lado contrario al pulgar. Decimos que la terna de vectores a, b y c tiene orientación negativa.
- Si (a × b) · c = 0, significa que el paralelepı́pedo tiene volumen 0, es decir, que los tres vectores están contenidos en un mismo plano si los pensamos con origen común. Decimos que a, b y c son coplanares.
![[Pasted image 20221013081911.png]]
Figura 7: Conservamos a y b fijos, y variamos c. Se indica qué ocurre con el producto mixto (a × b) · c.

Observación para el plano: En el plano también hay una noción de orientación positiva y negativa. Supongamos que los ejes x e y están ubicados en la forma usual, es decir, de forma tal que para llevar el semieje x positivo al semieje y positivo hay que girar en sentido antihorario (contrario al movimiento de las agujas del reloj). Si a = (a1 , a2 ), b = (b1 , b2 ) entonces podemos calcular el siguiente determinante:
$$d=\begin{bmatrix}
a_{1} & a_{2} \\ b_{1} & b_{2}
\end{bmatrix}$$
Su valor absoluto es el área del paralelogramo con lados a y b, pensados con origen común.
Además, su signo proporciona la siguiente información, ilustrada en la figura 8.
![[Pasted image 20221013082122.png]]
_Figura 8: Orientaciones y el valor de $d$._
- Si d > 0, significa que para llevar a sobre b hay que girar en sentido antihorario. Decimos que el par de vectores a, b, en ese orden, tiene orientación positiva.
- Si d < 0, significa que para llevar a sobre b hay que girar en sentido horario. Decimos que el par de vectores a, b, tiene orientación negativa.
- Si d = 0, significa que el paralelogramo tiene área 0, es decir, que los dos vectores están contenidos en una misma recta si los pensamos con origen común. Decimos que a y b son colineales.

# 11. Bases
En el plano, una base ordenada (o simplemente base) está formada por dos vectores no nulos y no paralelos, dados en un orden concreto. La escribimos con notación de conjuntos, por ejemplo, $$B =\{ (1,2), (0,1) \}$$
pero entendiendo que interesa el orden en que están dados: hay un primer y un segundo vector.

En la figura 8, los vectores a y b forman una base en los casos que corresponden a d > 0 y d < 0.
En el espacio, una base ordenada estará formada por tres vectores no nulos y no coplanares.
En la figura 7, los vectores a, b y c forman una base en el primer y tercer caso, pero no en el segundo.

Tanto en el plano como en el espacio, se puede saber si ciertos vectores dados forman una base si:
1. La cantidad de vectores es correcta (2 en el plano, 3 en el espacio)
2. El determinante formado poniendo los vectores como filas de una matriz (de 2 × 2 o 3 × 3 respectivamente) es distinto de 0.
Además, así como decíamos que el par o la terna de vectores tenía orientación negativa o
positiva según el signo del determinante, también diremos que la base tiene orientación positiva o negativa.
Una base proporciona un sistema de coordenadas donde los ejes no son necesariamente perpendiculares entre sí. En muchos contextos, es útil tener los ejes adaptados a las características del problema estudiado, en vez de que sean perpendiculares. 
# 11.1 Combinaciones lineales
Una característica fundamental de las bases es que todo vector se puede escribir como combinación lineal de los vectores de una base, y además en forma única. Es decir, si $B = {b_{1} , b_{2} , b_{3}}$, entonces todo vector v del espacio puede escribirse como $$v= \lambda_{1} b_{1} + \lambda_{2} b_{2} + \lambda_{3} b_{3}$$
y además los números reales $λ_{1} , λ_{2}, λ_{3}$ se pueden elegir de una única forma para ese v. Estos números se llaman las componentes de v en la base B. Comparar con lo que ocurría con la base standard de vectores vista antes. (Para el plano es lo mismo con un término menos).
Más adelante veremos fórmulas que permiten cambiar de base puntos y vectores, es decir, calcular las coordenadas o componentes en una base sabiendo las mismas en otra base. Esto permite “traducir” información que esté expresada en un sistema de coordenadas a otro. En la figura 9 se eligió una base B del plano, y se indican las componentes de los vectores en la base B (en otra base, serán otras componentes). ![[Pasted image 20221013084012.png]]
_Figura 9: Una base del plano y componentes de dos vectores en dicha base._

# Ecuación paramétrica de la recta
En el espacio, sea $P_{0}$ un punto y $d_{L}$ (o $\overrightarrow{d_{L}}$) un vector no nulo (en breve veremos por qué lo designamos así). Consideremos la recta que pasa por $P_{0}$y tiene la misma dirección que $d_{L}$ (figura 10).
Llamemos L a dicha recta1 (observemos que L es un conjunto de puntos). Llamemos (x0 , y0 , z0) a las coordenadas de P0 y (u 1 , u2, u3) a las componentes de dL. Entonces la recta L tiene la siguiente ecuación:
![[Pasted image 20221013085638.png]]
---
![[Pasted image 20221013085814.png]]
Esto significa: dar valores reales al parámetro λ; para cada uno de estos λ se genera un punto cuyas coordenadas (x, y, z) son las indicadas por estas tres fórmulas; haciendo que λ recorra todos los valores reales, obtenemos un conjunto de puntos que llamamos L. Observemos que es “L :” y no “L =”. Esto es porque estamos diciendo “el conjunto L está descripto por estas ecuaciones”. No es correcto decir que el conjunto L sea igual a las ecuaciones, ya que se trata de objetos de distinto tipo.
En el plano se puede hacer la misma construcción sólo que todo tendrá una componente o coordenada menos, y no habrá una ecuación con z. El vector dL se llama vector director de la recta L, ya que es el que le da su dirección. Observemos que cualquier múltiplo (no nulo) de dL también servirı́a como vector director de la misma recta. Asimismo, el punto P0 puede ser cualquier punto de la recta. Una misma recta tendrá ası́ muchas posibles ecuaciones paramétricas alternativas. Si conocemos dos puntos P y Q distintos en una recta, podemos construir una ecuación −→ paramétrica para dicha recta tomando por ejemplo P0 = P y dL = P 

Ejemplo 1. Escribamos la ecuación paramétrica de la recta que pasa por los puntos P (1, 4) y −→ Q(0, 5). Tomemos dL = P Q = (0 − 1, 5 − 4) = (−1, 1). Entonces
![[Pasted image 20221013090208.png]]
Observemos que para $λ = 0$ se obtiene el punto $(1, 4)$, y para $λ = 1$ el $(0, 5)$. Supongamos que queremos saber si la recta pasa o no por el punto $(3, 2)$. Lo que hacemos es buscar el valor de $λ$, si es que existe alguno, tal que las coordenadas $(x, y)$ producidas por estas fórmulas son $(3, 2)$. Planteamos entonces el sistema de ecuaciones
![[Pasted image 20221013090247.png]]
que tiene dos ecuaciones y una incógnita. En este caso el sistema es compatible determinado y la solución es $λ = −2$. Si fuera incompatible, significaría que la recta no pasa por el punto dado.

# 13. Ecuación del plano en el espacio
En el espacio, podemos describir un plano (es usual llamarlo π por ejemplo) a partir de un punto del mismo (es decir, de $P_{0} ∈ π$) y un vector no nulo nπ (o $\overrightarrow{n_{\pi}}$) , que llamamos vector normal a $\pi$.
Este vector será perpendicular al plano $π$. En este contexto, la palabra “normal” significa “perpendicular”. Si $nπ = (a, b, c)$ entonces la ecuación del plano (también llamada ecuación implícita del plano) es $$\pi: ax+by+cz+d=0,$$
donde $d$ es un número que se puede calcular sabiendo que las coordenadas de $P_{0}$ satisfacen la ecuación del plano.
![[Pasted image 20221013092856.png]]

**Observaciones:**
- Como antes, es “$π :$”, y no “$π =$”. 
- La ecuación significa: $π$ es el conjunto de todos los puntos del espacio cuyas coordenadas $(x, y, z)$ verifican la igualdad $ax + by + cz + d = 0$. 
- No probaremos que efectivamente una ecuación de este tipo representa a un plano, pero notemos que por ejemplo haciendo $a = 0, b = 0, c = 1, d = 0$, obtenemos la ecuación $z = 0$, que es el plano $xy$. 
- Es una ecuación lineal con tres incógnitas $x, y, z$. Notemos que $a, b y c$ no pueden ser simultáneamente $0$, ya que habíamos dicho que $n_{}π \neq 0$. Entonces siempre habrá una incógnita que se podrı́a despejar en términos de las dos restantes. Quedan ası́ dos variables independientes, que se corresponden con los dos “grados de libertad” en que uno puede moverse en un plano. 
- Es una ecuación lineal con tres incógnitas $x, y, z$. Notemos que $a, b y c$ no pueden ser simultáneamente $0$, ya que habíamos dicho que $n_{\pi} \neq 0$. Entonces siempre habrá una incógnita que se podría despejar en términos de las dos restantes. Quedan así dos variables independientes, que se corresponden con los dos “grados de libertad” en que uno puede moverse en un plano. 
- Se puede multiplicar $nπ$ por cualquier escalar no nulo y seguirá sirviendo como vector normal al plano. También, el punto $P_{0}$ puede ser cualquier punto del plano. Un mismo plano tendrá muchas posibles ecuaciones, todas equivalentes.

**Ejemplo 2.** Escribamos la ecuación del plano $π$ que pasa por el punto $(−1, 3, 2)$ y tiene vector normal $nπ = (1, 0, −1)$. La ecuación (preliminar) será $\pi: 1x+0y-1z+d=0,$ es decir, $\pi: x-z+d=0$.
con $d$ a determinar sabiendo que $(−1, 3, 2)$ satisface la ecuación. En la ecuación, reemplazamos $(x, y, z)$ por las coordenadas de ese punto, y queda $−1 − 2 + d = 0$, de donde $d = 3$. Finalmente la ecuación queda $π : x − z + 3 = 0$.

**Comentario.** Una ecuación como 2x − y = 3 describe una recta si estamos trabajando en el plano pero es la ecuación de un plano si estamos trabajando en el espacio. El contexto de la ecuación es relevante para poder decir qué representa. Habitualmente no escribimos con todo este detalle, pero lo que estamos queriendo decir al escribir “2x − y = 3” es lo siguiente:
- **En el plano:** “Consideremos todos los puntos del plano cuyas coordenadas (x, y) en el sistema de coordenadas elegido verifican que 2x − y = 3.” 
- **En el espacio:** “Consideremos todos los puntos del espacio cuyas coordenadas (x, y, z) en el sistema de coordenadas elegido verifican que 2x − y = 3.” En esta ecuación en particular, la coordenada z no juega ningún papel. Esto no quiere decir que z sea 0, sino algo totalmente opuesto: z es libre de tomar todos los valores reales.

