# [[ELEMENTOS DE ÁLGEBRA Y GEOMETRÍA]] 
---
# TEMA 9: SISTEMAS DE EUntitledCUACIONES LINEALES, MATRICES Y DETERMINANTES.

## 10.1 MATRICES:
Una matriz $m × n$ (o de orden $m × n$) es un cuadro de números con $m$ filas (horizontales) y $n$ columnas (verticales): $$\begin{pmatrix}a_{11}& a_{12}&...&a_{1n}\\a_{21}& a_{22}&...&a_{2n}\\ \vdots & \vdots & \ddots & \vdots 
 \\a_{m1} & a_{m2} & \cdots & a_{mn}\end{pmatrix}$$
 Si $m = n$, $A$ se dice una __matriz cuadrada de orden $n$__. El número $a_{ij}$ es el elemento de la matriz que está en la _fila_ $i$ y en la _columna_ $j$.
 
 A veces usaremos la notación $A = (a_{ij})$, $1 ≤ i ≤ m$, $1 ≤ j ≤ n$, para designar una matriz de orden $m × n$.
 Si $n = 1$, la matriz tiene una sola columna y se llama matriz columna. De la misma manera, si $m = 1$, la matriz tiene una sola fila y se llama matriz fila.
- ==Síntesis==:
	- $m=n$: Matriz cuadrada.
	- $m=0 \land n=1$: Matriz columna.
	- $m=1 \land n=0$: Matriz fila.

 Dos matrices $m × n$, $A = (a_{ij})$ y $B = (b_{ij})$, son iguales si $a_{ij} = b_{ij}$ para todos los valores posibles de los subı́ndices $i$ y $j$.

__Definición 10.1:__ La suma de dos matrices $A$ y $B$ de orden $m×n$ es otra matriz $m×n$ que se obtiene sumando los elementos correspondientes de A y B. En s´ımbolos, si $A = (a_{ij})$ y $B = (b_{ij})$, entonces $A + B = (a_{ij}) + (b_ij) = (a_{ij}+ b_{ij})$.

==Requisito para el producto de matrices de distinto órden:== __La cantidad de columnas del primer factor igual a la cantidad de filas del segundo.__ Además, no es redundante recalcar que esta operación, efectivamente, tiene órden. [IMÁGEN]

__Definición 10.3:__ Sea $A$ una matriz $m × n$, y sea $B$ una matriz $n × p$. El producto de $A$ y $B$ es la matriz $A · B$ de orden $m × p$ definida por: $$A \cdot B=(c_{ij}),$$ dónde $$c_{ij}= a_{i1}b_{1j}+a_{i2}b_{2j}+···+a_{in}b_{1n}=\sum_{t=1}^{n}a_{it}b_{tj}$$

### Propiedades:
- ($M_{1}$) Asociatividad: $A\cdot (B\cdot C)= (A\cdot B)\cdot C$.
- En general, $A\cdot B \neq B\cdot A$.
- ($M_{2}$)Distribuye con respecto a la suma, respetando el orden de los factores: $$A\cdot(B+C)=A\cdot B+A\cdot C$$
  equivalentemente,$$(B+C)\cdot A= B\cdot A+C\cdot A$$
- ($M_{3}$) __Matriz de identidad de orden n:__  Esta es una matriz $n×n$ en la que $a_{ii} = 1$ para todo $i$, $1 ≤ i ≤ n$, y $a_{ij} = 0$ si $i \neq j$. Se nota I ó In. [IMAGEN]
  ![[Pasted image 20220929084507.png]]
  [INVESTIGAR MATRIZ DE IDENTIDAD]
  Para toda matriz $A$ de orden $n$, tenemos $A\cdot I_{n}=A$, y también (aunque tomando en cuenta que debe cumplir con el requisito del orden), $I_{n}\cdot A=A$.
- ($M_{4}$) $(\lambda \cdot A)\cdot B=A\cdot(\lambda \cdot B)= \lambda \cdot (A\cdot B)$. Donde _lambda_ ($\lambda$) es un _escalar_.

### Matriz traspuesta: 
Se llama __matriz traspuesta__ de la matriz $A$, y se nota $A^T$, a la matriz que _se obtiene al intercambiar las filas y las columnas de_ $A$. Es decir, si $A = (a_{ij})$, entonces $A^T = (b_{ij})$, con $b_{ij} = a_{ji}$.
- Si $A$ es $m × n$, entonces $A^T$ es $n × m$.
- Si $A = A^T$ , entonces $A$ se dice simétrica.
![[Pasted image 20220929085518.png]]
#### Propiedades:
1. $(A^T)^T=A$.
2. $(A + B)^T = A^T + B^T$.
3. $(λ · A)^T = λ · A^T$.
4. $(A · B)^T = B^T · A^T$ , si el producto $A · B$ está definido.

## 10.2 SISTEMAS DE ECUACIONES LINEALES.
Consideremos un sistema de dos ecuaciones lineales con dos inc´ognitas: $$ ax + by = e \atop cx + dy = f$$
Un par ordenado de números ($x_0$, $y_0$) se llama _solución del sistema si al reemplazar $x$ por $x_0$ e $y$ por $y_0$ se satisfacen ambas ecuaciones_. Geométricamente, esto sucede cuando el punto ($x_0$, $y_0$) es el punto de intersección de las rectas $r1$ y $r2$, de ecuación $ax + by = e$ y $cx + dy = f$, respectivamente.

Hay tres posibilidades para el conjunto de soluciones:
1. Puede ser vacío, es decir, _las rectas $r_{1}$ y $r_{2}$ no se cortan_. Decimos entonces que __el sistema es incompatible__.
2. Tiene exactamente un punto. Geométricamente significa que _las rectas se cortan_. Decimos que __el sistema es compatible determinado__.
3. Contiene infinitos puntos, es decir, _$r_{1}$ y $r_{2}$ son coincidentes_. En este caso decimos que __el sistema es compatible indeterminado__.
![[Pasted image 20220929093554.png]]

Para resolver un sistema de dos ecuaciones lineales con dos inc´ognitas se acostumbra usar alguno de estos tres métodos: 1. Sustitución. 2. Igualación. 3. Eliminación.

### Método de Eliminación de Gauss:
Nos proponemos indicar un método que nos permita resolver sistemas de $m$ ecuaciones lineales con $n$ incógnitas, $m$ y $n$ arbitrarios. Tal sistema puede escribirse: $(1)$
![[Pasted image 20220929093759.png]]
donde los números (reales o complejos) $a_{ij}$ , $1 ≤ j ≤ n$, $1 ≤ i ≤ m$, son los coeficientes, y los números (reales o complejos) $b1, b2, . . ., bm$ son los términos independientes.
Un sistema de $n$ números $k1, k2, . . . , kn$, es una solución del sistema de ecuaciones lineales $(1)$, si cada una de las ecuaciones del mismo se convierte en una identidad después de haber sustituido en ellas las incógnitas $x_{i}$ por los correspondientes valores $ki , i = 1, 2, . . . , n$.

[PLANTILLA DEL MÉTODO]

Si durante la aplicación del método de eliminación de Gauss alguna de las matrices intermedias tiene una fila con todos los elementos nulos excepto el último, es decir, una fila de la forma $$\begin{matrix}0 & 0 & · · · & 0 & b \end{matrix}$$con $b \neq 0$,
entonces el sistema es incompatible, ya que esa fila corresponde a una ecuación $0_{x1} + 0_{x2} + · · · + 0_{xn} = b$ que no tiene solución.

---
[CLASE FALLIDA XD]

---

## Propiedades de las Determinantes 
- $det(A\cdot B) = det(A)\cdot det(B)$
	- Siempre que $A$ y $B$ sean matrices cuadradas del mismo orden.
- $det(A\urcorner)= det(A)$
- Observación: 
	-  $det(A+B)\neq det(A)+det(B)$
	- $det(0_{nm})=0$
	- $det(I_{n})=1$

---

## Matrices inversas
Para cada elemento de la matriz, consideramos la submatriz que queda al eliminar la correspondiente fila y columna, y calculamos su determinante.
__El determinante de la submatriz se llama__ _menor complementario_ $(M_{ij})$ _del elemento_ $a_{ij}$ tomado.

Complemento algebraico o cofactor: A_ij = (-1)^i+j * M_ij
- Básicamente, dependiendo de la paridad de i+j, se cambia el signo o se mantiene.

Con los $A_{ij}$ armamos la matriz adjunta de $A$: $$\begin{equation}A=\begin{bmatrix} 1& -1& 2 \\ 0& 1& 3 \\ 1& -1& 0 \end{bmatrix}\end{equation} $$
$$\begin{equation}adjA=\begin{bmatrix} 3& 3& -1 \\ -2& -2& 0 \\ -5& -3& 1 \end{bmatrix}\end{equation} $$
La inversa de A es: $$A^{-1}=\frac{(adj(A))^T}{det A}$$
En este ejemplo, $det A = -2$, por lo que $$\begin{equation}A^{-1}=\frac{1}{-2}\begin{bmatrix} 3& -2& -5 \\ 3& -2& -3 \\ -1& 0& 1 \end{bmatrix}\end{equation}=\begin{bmatrix} -3/2& 1& 5/2 \\ -3/2& 1& 3/2 \\ 1/2& 0& -1/2 \end{bmatrix}$$
Observaciones:
- Existe $A^{-1} \iff det A \neq 0$ 
- Conviene calcular $det A$ antes de calcular la matriz adjunta
- [LA CONCHAAA]

Para verificar, alcanza con comprobar una sola de las igualdades $$A\cdot A^{-1} = I_{n} = A^{-1} \cdot A = I_{n}$$
Mejor aún, como $A^{-1} =\frac{(adj(A))^T}{det A}$, podemos comprobar si [LA CONCHAAA]

Forma matricial de un sistema de ecuaciones lineales 
[SCREENCHOT]

Definimos $$\begin{equation}A=\begin{pmatrix}a_{11}& a_{12} & \dots & a_{1n} \\ a_{21} & a_{22} & \dots & a_{2n} \\ \vdots & \vdots & \ddots &\vdots  \\ a_{m1} & a_{m2} & \dots & a_{mn} \end{pmatrix} \end{equation}$$

---
Si $A$ es cuadrada e inversible, es decir, hay tantas ecuaciones como incógnitas ($n$) y existe $A^{-1}$, entonces 
$$\begin{split} A\cdot X=B \iff \newline A^{-1} \cdot A\cdot X= A^{-1} \cdot B \iff \newline I_{n} \cdot X = A^{-1} \cdot B \iff \newline X = A^{-1} \cdot B \end{split}$$
En particular, el sistema lineal es compatible determinado

Si en un sistema lineal de $n$ ecuaciones con $n$ incógnitas la matriz de coeficientes $A$ tiene determinante no nulo, entonces el sistema es compatible determinado.
