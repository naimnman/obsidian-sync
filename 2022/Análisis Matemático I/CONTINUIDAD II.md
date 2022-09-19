# [[ANÁLISIS MATEMÁTICO I]] 
---
# TEMA 5: CONTINUIDAD II, FUNCIONES CONTÍNUAS.

$f$ es contínua en $x_0$ cuando ocurre:
- existe $lím~x\rightarrow x_{0}⁺$ $f(x)=L_{1} \in R$
- existe $lím~x\rightarrow x_{0}⁻$ $f(x)=L_{2} \in R$
- existe $f(x_0)$
- _son todos iguales_.

__Nomenclatura__
- Cuando $L_1=L_2$, diremos que $f$ tiene una discontinuidad evitable en $x_0$ _(el gráfico tiene un hueco)._

Esto puede ocurrir por dos razones distintas;
- $x_{0} \notin Dom(f)$, por ejemplo, $f(x)= \frac{x²-3x+2}{x²-1}$, en $x_0=1$.
	- ¿Cómo evitar la discontinuidad? _”Llenar el hueco:”_
		- agregar $x_0$.
- $x_{0} \in Dom(f)$, pero $f(x_{0}) \neq L_1=L_2$.
	- ¿Cómo evitar la discontinuidad? _“Llenar el hueco:”
		- corregir $f(x_0)$.
	- Por ejemplo, $f(x)= \frac{x²-1}{\sqrt{x-1}}$, $g(x)=\sqrt{x-1}$
	  Planteo: $x-1>0\rightarrow x>1$, implica $Dom (f): (1, +\infty)$.
		- __¿Dónde puede fallar la continuidad?__
		- __¿Dónde hay que mirar con cuidado la continuidad? (Álgebra de funciones contínuas)__
			- _2 casos:_
				- “Falla la fórmula”.
				- Borde del dominio (no implica que el borde sea parte del dominio).
		- $$lím~x\rightarrow 1⁺ ~ \frac{x²-1}{\sqrt{x-1}} $$
			- Dónde el númerador tiende a 0 y el denominador también.
		- __C.A:__ $$\frac{x²-1}{\sqrt{x-1}} = \frac{(x²-1)\sqrt{x-1} }{(\sqrt{x-1})(\sqrt{x-1})}=$$$$\frac{(x-1)(x+1)\sqrt{x-1} }{(x-1)} = (x+1)\sqrt{x-1}$$Por lo que, al buscar el límite con la fórmula reescrita tenemos que $$lím~x\rightarrow 1⁺ ~ f(x)=(x+1)\sqrt{x-1}=0$$
		  Y llegamos a que $f$ tiene una discontinuidad evitable en $x_0=1$.
		  En otras palabras, para “evitar”, debemos “cambiar” la función: $f(x)=(x+1)\sqrt{x-1}$ y $f(1)=0$.
	- __Nomenclatura:__
		- $L_{1}\neq L_{2}$, significa que $f$ tiene discontinuidad de tipo salto (finito).
			- Si $L_{1}$ o $L_2$, o ambos es infinito, entonces la recta $x=x_{0}$ es una asíntota vertical (derecha, izquierda, ambos) de $f$.
- __Álgebra de funciones continuas:__
	- Sean $f$, $g$ y $h$ funciones continuas: $f$ y $g$ son continuas e $J$, entonces $g(x) \neq 0$ en $J$ y $h$ es contínua en el intervalo $I$.
	- La función $f+g$ es contínua en $J$.
	- La función $f*g$ es contínua en $J$.
	- La función $\frac{f}{g}$ es contínua en $J$.
	- Si $f(x) \in I$ para $x \in J$, entonces $h(f(x))$, osea $h\circ f$, es contínua en $J$.
---
__Proposición:__ ==Teorema de Bolzano.==
- $f$ es contínua en $[a,b]$ y $f(a)*f(b)<0$, entonces, existe $c \in (a,b): f(c)=0$. 
  __Coloquialmente,__ _la función tiene al menos una raíz en el intervalo $(a,b)$ ó, la ecuación tiene al menos una solución en $(a,b)$._
- Por ejemplo, $f(x)=x-cos(x)$, y consideramos la ecuación $f(x)=0$.
	- ¿Tiene solución? ¿Cuántas? ¿Dónde están?
	- $f$ es resta de funciones contínuas en $R$, entonces $f$ es contínua en $R$.
	- En general, la dificultad está en hallar intervalo donde $f$ cambie de signo, $f(0)=0-cos(0)=-1$, y $f(1)=1-cos(1)=0,45...$, por lo que entre este intervalo debe existir al menos un cambio de signo.
	  [GEOGEBRA F(X)]
	- Para buscar dicha raíz, remplazamos utilizando una busqueda binaria, hasta allar el cambio de signo
	  ![[Pasted image 20220919153749.png]]
---
- Variantes: 
	- Método de punto fijo.
	  $x-cos(x)=0$ $\rightarrow ~ x=cos(x)$ $\rightarrow x=f(x)$, debemos remplazar por una sucesión definida:
	  $x_{n+1}=cos(x_n)$, en la calculadora sería $ANS=cos(ANS)$, sucesivamente.
	  
  1) Para el mismo problema, $f$ es contínua en $(a,b)$ y existen $lím~x\rightarrow a⁺$ $f(x)=f(a⁺)$ y $lím~x\rightarrow b⁻$ $f(x)=f(b⁻)$.
		- Consecuencia: todo polinomio de grado impar tiene (al menos) una raíz real.
  2) Para resolver la ecuación $f$ contínua en $(a,b)$ y $f(x)\neq 0$ en $(a,b)$, entonces el signo de $f$ es constante en $(a,b)$. Para saber el signo, alcanza con elegir $x_0(a,b)$ y buscar el signo $(f(x_0))$.
     - Ejemplo: Sea $f(x)=\frac{x+1}{x²-4}$, hallar $C⁰$, $C⁺$ y $C⁻$. $$C⁰(f)=[x:f(x)=0]$$ $$C⁺=[x:f(x)>0]$$ $$C⁻=[x:f(x)<0]$$
     