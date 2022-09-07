# [[ANÁLISIS MATEMÁTICO I]]
---

# TEMA 3: Sucesiones numéricas
- Una sucesión numérica es un conjunto ordenado de números. Cada uno de ellos es denominado término (también elemento o miembro) de la sucesión y al número de elementos ordenados (posiblemente infinitos) se le denomina la longitud de la sucesión. $$f:N➙R$$
- __Aspectos a conocer de las suceciones:__
	- _Monotonía:_
		- Creciente.
		- Decreciente.


---
## Sucesiones Recursivas:
Son procesos con retroalimentación. En este caso se dispone de una fórmula que indica cómo hallar un término a partir de los anteriores.
$$a_{n+1}=a_0+r*a_n$$
Este ejemplo recibe el nombre de __sucesión aritmética.__
- Una sucesión aritmética es _creciente_ cuando la razón $r$ por la que está acompañada está sumando a la función recursiva. $r>0$
- En cambio, la sucesión aritmética es _decreciente_ cuando dicha razón $r$ está restando a la función. $r<0$

__Sucesiones Geométricas:__ Una sucesión geométrica es aquella en la que cada término $a_n$ se obtiene multiplicando al término anterior $a_{n-1}$ por un número $r$ llamado _razón_. Cabe aclarar que la _razón_ de una sucesión geométrica debe ser constante en toda la sucesión.

---
## Expresiones asintóticas (cálculo de límite)
$$a_n=\frac{2n²+3n-1}{3n³+6n-2}$$
- Localizar los __términos dominantes__, siendo estos los términos con _mayor exponente_.
- Sacar factor común con los __términos dominantes__. 
  Numerador: $$2n²+3n-1=2n²(\frac{2n²}{2n²}+\frac{3n}{2n²}-\frac{1}{2n²})$$
  Denominador: $$3n³+6n-2=3n³(\frac{3n³}{3n³}+\frac{6n}{3n³}-\frac{2}{3n³})$$
- Esto es $$\frac{2n²(1+\frac{3}{2n}-\frac{1}{2n²})}{3n³(1+\frac{2}{n^2}-\frac{2}{3n³})}$$
- Simplificar $$\frac{2(1+\frac{3}{2n}-\frac{1}{2n²})}{3n(1+\frac{2}{n^2}-\frac{2}{3n³})}$$
- Los términos dentro del paréntesis son aproximadamente iguales a 1. $$\frac{(1+\frac{3}{2n}-\frac{1}{2n²})}{(1+\frac{2}{n^2}-\frac{2}{3n³})}≈1$$
- Mientras que de los factorizados podemos llegar a que $$a_n≈\frac{2}{3n}$$