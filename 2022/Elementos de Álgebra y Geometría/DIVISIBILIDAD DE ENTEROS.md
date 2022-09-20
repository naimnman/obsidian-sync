# [[ELEMENTOS DE ÁLGEBRA Y GEOMETRÍA]]
---
# TEMA: DIVISIBILIDAD DE ENTEROS
_Definición 6.1:_ Sean $a, b ∈ Z$. Se dice que $a$ divide a $b$, y escribimos $a | b$, si existe $k ∈ Z$ tal que $b = a · k$.
En este caso diremos también que $a$ es un factor de $b$, que $b$ es divisible por $a$ ó que $b$ es múltiplo de $a$. Si $a$ no divide $a|b$ escribimos $a|b$.

## Propiedades:
1. $a|a$. Reflexividad: cada número entero es divisibile por sí mismo, siendo $k=1$.
2. Si $a|b$ y $b|c$, entonces $a|c$. Transitividad:
   $b=a*k$ y $c=b*k'$, remplazando $c=a*k*k'=a*k''$, donde $k''=k*k'$ 
3. $a|0$. Donde explícitamente $k=0$. 
4. Si $c|a$ y $c|b$, entonces $c|ax+by$, con $x,y\in{Z}$. 
   _Si un número divide a otros dos, entonces divide a cualquier combinación lineal de esos dos._
5. Si $a|b$, entonces $a|-b$, $-a|b$ y $-a|-b$. [Self-explanatory]
6. Si $a|b$, entonces $ac|bc$. Es posible mantener la igualdad debido a que la divisibilidad de enteros es una relación binaria.
7. Si $a|b$ y $b\neq{0}$, entonces $|a|\leq{|b|}$. Esto debido a que por condición $a<b$ para que $b$ pueda ser escrito como $b=a*k$.
8. $a|b$ y $b|a$ <=> $|a|=|b|$.
	- __Demostración:__
	   Supongamos que $a|b$ y $b|a$,
	   $b=a*k$, para cierto $k\in{Z}$
	   $a=b*k'$, para cierto $k’\in{Z}$
	   Remplazando $a=a*k*k'$
	   Si fuera $a=0$, de $b=a*k$ resulta $b=0$, en ese caso; $|a|=|b|$.
	   En cambio, si $a\neq{0}$, $a=a*k*k'$ implica $k*k'=1$ por simplificación.
	   Entonces como $k*k'\in{Z}$, resulta que el valor de $k=\pm{1}$.

### Observaciones:
1.  $c|a+b$ no implica que $c | a$ ó $c | b$. Por ejemplo, $6 | 4 + 8$, pero $6 \nmid 4$ y $6 \nmid 8$.
2. Sin embargo, si $c | a + b$ y se sabe que $c | a$ entonces $c | b$ (pues $c | (a + b) − a$).
3. Si $c | a$, entonces $c | k · a$ para todo $a ∈ Z$.
4. Si $c | a$, entonces $c | a²$  y $c | a^n$ para todo $n ∈ N$.

---

## Máximo Común Divisor
Sea $a ∈ Z$ y sea $D(a) = [c ∈ Z : c | a]$. Es claro que $D(a) = D(−a)$, para todo $a ∈ Z$ y si $a \neq 0$ , $D(a)$ es un conjunto finito.

### Algoritmo de Euclides (existencia del máx. común div.)
Sean $a$ y $b$ dos enteros no simultáneamente nulos. Como $(a, b) = (a, −b)$, podemos suponer sin pérdida de generalidad que $b > 0$. 
Sea $r_1$ el resto de dividir $a$ por $b$ . Si $r_1 = 0$ entonces $b | a$ y entonces $(a, b) = |b| = b$. Si $r_1 \neq 0$ por divisiones sucesivas obtenemos:
![[Pasted image 20220920082047.png]]
donde, como $b > r1 > r2 > · · · ≥ 0$, al cabo de un número finito de divisiones se obtiene un resto nulo, es decir, $$r_{n-1}=r_{n} \cdot q_{n+1}$$
(de lo contrario habría infinitos enteros positivos menores que $b$). Veamos que $r_n = (a, b)$. En efecto, como $r_n | r_{n-1}$ , aplicando el corolario anterior reiteradamente obtenemos: $$r_n = (r_{n−1}, r_n) = (r_{n−2}, r_{n-1}) = · · · = (r_2, r_3) = (r_1, r_2) = (b, r_1) = (a, b)$$
Este algoritmo se puede esquematizar mediante la siguiente tabla: 
![[Pasted image 20220920082639.png | #small]]
El último resto no nulo es el máximo común divisor. Si el resto es cero en la primera división, es decir, si $a$ es un múltiplo de $b$, entonces $(a, b) = b$ (estamos suponiendo que $b > 0$). En este caso convenimos en que el último resto no nulo es $b$.

---
- [Proposición 6.6]
	- [Demostración]
- [Definición 6.7]
- [Proposición 6.8 (Euclides)]
- [Proposición 6.9]
	- [Demostración ]
---

## Mínimo Común Múltiplo (M.C.M)
Dado un número entero $a$, sea $M(a)$ el conjunto de todos los múltiplos no negativos de $a$. Así por ejemplo, $M(3) = [0, 3, 6, 9, . . .]$, $M(0) = [0]$, $M(1) = N ∪ [0]$. Es claro que $M(a) \neq ∅$.
Sean $a$ y $b$ dos enteros y notemos $M(a, b)$ el conjunto de todos los múltiplos no negativos comunes de $a$ y $b$. Es claro que $M(a, b) = M(a) ∩ M(b)$. Vamos a probar el siguiente teorema
- __Teorema 6.12:__ Si $a$ y $b$ son dos enteros, entonces existe $m ∈ M(a, b)$ tal que si $c ∈ M(a, b)$, entonces $m | c$.
El número $m$ del teorema se llama el mínimo común múltiplo de los enteros $a$ y $b$, y se nota [a, b].

Observemos que de la demostración del teorema anterior resulta un procedimiento para calcular el mínimo común múltiplo de $a$ y $b$ no simultáneamente nulos, a saber, $$[a,b]= \frac{|a \cdot b|}{(a,b)}$$

## Números Primos
Si $a ∈ Z$, $a$ es divisible por $a, −a, 1, −1$, que se denominan los _divisores triviales de a_ . Si a posee otro divisor, éste se llama un _divisor propio_.

- __Definición 6.13:__ Un entero $a \neq 0, 1, −1$ se dice primo si sus únicos divisores son los triviales.

- __Teorema 6.14:__ Todo número entero $a \neq  0, 1, −1$ admite por lo menos un divisor primo positivo.
	- __Demostración:__ Sea $m \in Z$,  _el menor entero mayor que 1 que divide a $a$_. Veamos que $m$ es primo. Si $m$ no fuera primo existiría $k ∈ Z$ tal que $1 < k < m$ y $k | m$. Como $m | a$, resulta $k | a$, lo que contradice la definición de $m$.