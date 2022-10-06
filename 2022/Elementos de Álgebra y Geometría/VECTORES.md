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
Vamos a dar una definición preliminar de la noción de vector. Definimos un vector como un segmento de lı́nea dirigido con punto inicial en el origen, es decir, un segmento con una dirección, sentido y magnitud (longitud) especificados, y punto inicial en el origen. Se puede representar mediante una flecha que parte del origen, como en la figura siguiente. Tipográficamente, se representa como una letra en negrita, o con una flecha arriba, o con una lı́nea debajo o incluso sin ningún indicador especial: a, ~a, a, a. También se acostumbra usar letras cercanas a la v en el alfabeto: u, v, w. Para escritura a mano, es más cómodo escribir los vectores con flechas: ~a, ~v.

![[Pasted image 20221006094151.png]]

Esta definición funciona tanto en el plano como en el espacio. Escribiremos lo siguiente pensando que estamos trabajando en el espacio, y en el plano simplemente habrá que usar pares en vez de ternas. Usando esta definición, podemos asociar a cada vector a el punto $(a_{2} , a_{2} , a_{3})$ donde a termina (es decir, las coordenadas de la punta de la flecha). Recı́procamente, a cada punto $(a_{2} , a_{2} , a_{3})$ del espacio le hacemos corresponder el vector a que será una flecha desde el origen hasta dicho punto. Ası́, identificaremos a con $(a_{2} , a_{2} , a_{3})$ y escribiremos $a = (a_{1} , a_{2}, a_{3} )$.
$$\begin{equation} a= \begin{dmatrix} 1 \\ 2 \end{dmatrix} \end{equation}$$
$$\begin{equation} v= \begin{dmatrix} 0 \\ -1 \\ 5\end{dmatrix} \end{equation}$$
Sin embargo, por comodidad en la escritura seguiremos usando la notación $a = (1, 2)$, $v=(0, −1, 5)$ por ahora.

## Suma de vectores
Definimos la suma de vectores (pensados como flechas) con la llamada regla del paralelogramo, como sigue. Para sumar los vectores a = (a1 , a2, a3 ) y b = (b1 , b2 , b3) consideramos el paralelogramo que tiene a y b como lados adyacentes (ver figura 1). La suma a + b se define como el vector que va a lo largo de la diagonal.
![[Pasted image 20221006095448.png]]
Muy importante: afortunadamente, las componentes de este vector a + b resultan ser (a1 + b1, a2 + b2, a3 + b3 ), que es precisamente el resultado de sumar las ternas correspondientes a los vectores a y b. No es difı́cil de probar pero no lo demostraremos aquı́.
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
