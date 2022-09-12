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

## Límite (sucesiones)

Formalizar la idea de “comportamiento terminal”
[GRÁFICO FUNCIÓN DECRECIENTE CON LÍMITE EN 5]
Asumiendo que el gráfico es “decreciente”, ¿qué podemos decir de $a_{184}$? Recordar que $a_n=a(n)$
$$a_{184}\approx{5}$$
_Resumiendo, el escenario es “para valores grandes de n” vale $a_{n}\approx{L}$ (por ahora $L\in{R}$), es decir, límites ==finitos==._

==Nota: los números Naturales==
_Solo pueden crecer._ Entonces, “valores grandes de n” será interpretado como “estár cerca de infinito” 
[RECTA NUMÉRICA]

Cuando $a_{n}\approx{L}$, “$n\rightarrow\infty$”, ocurre que:
[FOTO CElU]
Dónde $\epsilon$ denota la “precisión”, que decrece a medida que $n$ se hace más grande. $L+\epsilon$ y $L-\epsilon$

Existe un término $n_0$ a partir del cual los términos siguientes aproximan a $L$ con esa precisión.

Simbólicamente, $a_n$ “está en la región” para $n\geq{n_0}$ quiere decir $L-\epsilon<a_n<L+\epsilon$, usando notación de entornos: $$|a_n-L|<\epsilon$$
En definitiva, $lím~a_n=L\in{R}$, si y sólo si $\forall\epsilon>0$ exíste $n_0:|a_n-L|<\epsilon$ para $n\geq{n_0}$.

## Límite infinito
[FOTO LÍMITE INFINITO]
“Estar cerca de $\infty$” $\iff$ “estar lejos de $0$”.
$lím~a_n=+\infty$   
__Si y sólo si $\forall{M}>0$ existe $n_0:M<a_n$, para $n\geq{n_0}$
$a_{n}< -M$, reordenando $M< |a_{n}|$.__

### Arquimedianidad
Si $a>0$ cualquiera (muy pequeño) y $b>0$ cualquiera (muy grande), existe $k\in{N}:a*k\leq{B}\leq{a*(k+1)}$
por lo que la parte entera $k$ es igual a $\lfloor \frac{b}{a} \rfloor$

Tomando $a_{k}=k$ podemos demostrar que $\lceil M \rceil$, $\forall{M}>0$ $\exists{k}: M<k=a_{k}$.

Análogamente, $lím~n² = +\infty$.
Demostración: Tomar $M>0$, $M<n²$, aplicando raíz cuadrada $\sqrt{M}< |n|$.

### Algunos límites conocidos
- $lím~n^r=+\infty$, con $r>0$.
- $lím~\frac{1}{n^r}=lím~n^{-r}=0$
- $lím~q^n$ es igual a:
	- $0$, si $|q|<1$
	- $+\infty$, si $|q|>1$
	- [PREGUNTAR]
	- [PREGUNTAR]

==NOTA:== 
Demostrar $(\frac{13}{7})^{n} \rightarrow +\infty$,
$m < (\frac{13}{7})^{n}$
[PREGUNTAR]

### Álgebra de límites 
- Supongamos $a_{n} \rightarrow L\in{R}$ y $b_{n} \rightarrow T\in{R}$, entonces
	- $lím~a_{n}+b_{n}=L+T$
	- $lím~a_{n}-b_{n}=L-T$
	- $lím~a_{n}*b_{n}=L*T$
	- $lím~\frac{a_{n}}{b_{n}}$ es igual a:
		- $\frac{L}{T}$, cuando $T\neq{0}$.
		- $\infty$, cuando $L\neq 0 \land T=0$.
		- $?$, cuando $L=0 \land T=0$.
- Luego, $a_{n}\rightarrow L$ y $b_{n} \rightarrow \infty$
	- 
	- $lím~\frac{a_{n}}{b_{n}}=0$
	- $lím~\frac{b_n}{a_n}=Sg(L)$


### Indeterminaciones
Casos NO contemplados en álgebra de límites:
- $\frac{a_n}{b_n}$, dónde $a_{n}\rightarrow 0$ y $b_{n}\rightarrow 0$, por lo que tenemos $\frac{0}{0}$.
- $a_{n}*b_{n}$, dónde $a_{n}\rightarrow 0$ y $b_{n}\rightarrow \infty$, por lo que tenemos $0*\infty$
- $a_{n}-b_{n}$, dónde $a_{n}\rightarrow \infty$ y $b_{n}\rightarrow -\infty$, por lo que tenemos $\infty - \infty$.
- [INVESTIGAR INDETERMINACIONES DE ÁLGEBRA DE LÍMTIES]

### Criterio del cociente (útil para sucesiones)
De términos grandes por lo menos, geométricas.
[INVESTIGAR Y ADJUNTAR PLANTILLA DE RESOLUCIÓN]

### Multiplicación por conjugado
[INVESTIGAR Y ADJUNTAR PLANTILLA DE RESOLUCIÓN]
[<iframe src="https://www.matematicatuya.com/limite/S2a.html" allow="fullscreen" allowfullscreen="" style="height:100%;width:100%; aspect-ratio: 16 / 9; "></iframe>](https://www.matematicatuya.com/limite/S2a.html)

