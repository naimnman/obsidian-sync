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


