# [[ANÁLISIS MATEMÁTICO I]] 
---
# TEMA 6: DERIVABILIDAD I

# Derivadas
¿Qué significa?
En términos de cercanía, la derivada se encarga de relacionar los datos de entrada ($x$ cerca de $x_0$) con los datos de salida ($f(x)$ cerca de $f(x_0)$), devolviendo la “proporción”.

¿Cómo se calcula?
$$f'=\frac{\triangle f}{\triangle x}=\frac{f(x)-f(x_0)}{x-x_{0}}$$

¿Para qué sirve?

¿Cómo se usa?

Requisitos:
- Para calcular el límite $L_{f,x_{0}}$ _(llamada “recta tangente al gráfico de $f$ en $x_{0}$)_ que pasa por $(x_{0}, f(x_{0}))$ y tiene pendiente $m_{0}$ (conocida como __tasa de cambio__), la cual debemos calcular de la siguiente manera: $$m_{0}= lím~x\rightarrow x_{0} \frac{f(x)-f(x_0)}{x-x_{0}}$$
Esta cantidad puede existir (o no). Cuando existe, diremos que:
- $f$ es _“derivable”_ en $x_{0}$ y $m_{0}=f'(x_{0})$.
- la curva es _“rectificable”_ (al gráfico).
- $f(x) \approx y(x)$, con $x\approx x_0$
- $y(x)= f(x_{0})+f'(x_{0})\cdot (x-x_{0})$

==Nota:== Cuando $f'$ es derivable en $x_{0}$, la ecuación de la recta tangente (a $f$ en $x_{0}$) me permite aproximar a $f$ para $x \approx x_{0}$. $$f(x)\approx f(x_{0}+f'(x_{0})\cdot(x-x_{0}))$$

---
==Nota:== $x=x_{0}+h \rightarrow h=\triangle x$, es simplemente otra proposición notacional. $$lím ~h\rightarrow 0 ~\frac{f(x)-f(x_0)}{h}$$

---
Ejemplo: $f(x)=x²$ $$f'(x)= lím~x\rightarrow x_{0}~\frac{f(x)-f(x_0)}{x-x_{0}}$$
Remplazamos las variables:
$$f'(x)= lím~x\rightarrow x_{0}~\frac{x²-x_{0}²}{x-x_{0}}$$
Reescribimos el numerador como una diferencia de cuadrados:
$$f'(x)= lím~x\rightarrow x_{0}~\frac{(x-x_0)(x+x_0)}{x-x_{0}}$$
Simplificamos $x-x_0$:
$$f'(x)= lím~x\rightarrow x_{0}~~~(x+x_0)$$
Ya que $x\rightarrow x_{0}$, tenemos: $$f'(x)= lím~x\rightarrow x~~x+x_{0}=2x_{0}$$

---

==Tarea:== Hallar $f'(x)$ para las funciones elementales.

---
Ejemplo 1: $f(x)= |x|$.
$x_{0}=1$, $f$ es derivable en $x_{0}$ y $f'(x_{0})=1$.
$x_{0}=-1$, $f$ es derivable en $x_{0}$ y $f'(x_{0})=-1$.

Analíticamente: $$lím~ x\rightarrow 1~~\frac{f(x)-f(1)}{x-1}=lím~ x\rightarrow 1~~\frac{|x|-|1|}{x-1}=\frac{-1}{-1}=1$$
Sucede lo mismo al analizar el $lím~x\rightarrow -1$.

==Nota:== __la función módulo $|x|$ NO es derivable en $x_{0}=0$, debido a que no es rectificable, ya que los límites laterales NO coinciden__.

---

Ejemplo 2: $f(x)=³\sqrt{x}$.
[Fotos] o [Cherman]

---
## Cómo derivar fórmulas

$f(x)=x² \implies f'(x)=2x$ 
$f(x)=\sqrt{x} \implies f'(x)=\frac{1}{2\sqrt{x}}$

La derivada de una función lineal es la propia pendiente, por ejemplo $f(x)=3x-1 \implies f'(x)=3$.
Mientras que la derivada de una función constante es cero, utilizando la misma lógica.

## Propiedades: “Álgebra de funciones derivables”
- $f$ y $g$ son derivables en $x_{0}$ entonces,
	- $f+g$ es derivable en $x_{0}$ y $(f+g)'(x_{0})=f'(x_{0})+g'(x_{0})$
	- $(constante\cdot f)$ es derivable en $x_{0}$ y $(constante\cdot f)'(x_{0})= constante\cdot f'(x_0)$
	- $f\cdot g$ es derivable en $x_{0}$ y $$(f\cdot g)'(x_0)=f'(x_{0})\cdot g(x_{0})+f(x_{0})\cdot g'(x_{0})$$
		- Esta propiedad distributiva es escalable a $n$ factores a distribuir, y se aplica de la siguiente manera: $$(f\cdot g\cdot h)'(x_{0})=f'(x_{0})\cdot g(x_{0})\cdot h(x_{0})+f(x_{0})\cdot g'(x_{0})\cdot h(x_{0})+f(x_{0})\cdot g(x_{0})\cdot h'(x_{0})$$
	- sea $g(x_{0})\neq 0 \implies \frac{f}{g}$ es derivable en $x_{0}$ y $$(\frac{f}{g})'(x_{0})=\frac{f'(x_{0})\cdot g(x_0)-f(x_{0})\cdot g'(x_0)}{(g(x_0))²}$$
	- Composición: Regla de la cadena.
	  Si $f$ es derivable en $x_{0}$ y $g$ derivable en $f(x_{0})$ entonces $g(f(x))$ es derivable en $x_{0}$, y $(g\circ f)'(x_{0})=g'(f(x))$
	- Al igual que la distributiva, la composición es escalable en factores: $$(h\circ g\circ f)'(x)=h'(g(f(x)))\cdot g'(f(x))\cdot f'(x)$$
---	
[IMPORTAR TABLA DE DERIVADAS]

---

# Aproximaciones de orden superior

Aproximación de orden “1”
$$f(x) \approx y(x)=f(x_{0})+f'(x_{0})(x_{x_{0}})$$
Ecuación de la recta tangente (al gráfico de $f$ en elpunto $(x_{0}, f(x_{0}))$) válido para $x\approx x_{0}$.

En el ejemplo: $x_{0}=0$, $f(x)=e^{x} \implies$
Cálculo auxiliar:
$f(x_{0})= e⁰=1$; $f'(x)=(e^x)'=e^x$
$f'(x_{0})=e⁰=1$

---
La ecuación para la recta tangente será $y=1+1(x-0) \longrightarrow y=1+x$.
La aproximación será: $e^{x}\approx 1+x$, cuando $x\approx 0$.
	Ejemplos:
	$e^{0.1}\approx 1+0.1=1.1$
	$e^{-0.05} \approx 0.95=1-0.05=0.95$
---

## Taylor de orden 2
Buscamos una expresión cuadrática que se aproxime para obtener los dígitos faltantes:
$$f(x_{0})+f'(x_{0})(x-x_{0})+coef(x-x_{0})²$$
Para descubrir cuánto vale el coeficiente faltante, veamos una propiedad importante de la recta tangente:
- **Propiedad:** Si $f$ es derivable en $x_{0}$, entonces la recta tangente tiene por ecuación a $y=f(x_{0})+f'(x_{0})(x-x_{0})$.
- **Además,** la función lineal tiene las siguientes características:
  1. $y(x_{0})=f(x_{0})$
  2. $y'(x_{0})=f'(x_{0})$
  - ($f$ y la aproximación $y$ coinciden en $x_{0}$ como también sus derivadas).
- **Además,** si $g(x)=a+b(x-x_{0})$ es otra función _lineal_ y $g(x_{0})=f(x_{0})$, y también $g'(x_{0})=f'(x_{0})$. Por lo que podemos afirmar que $g(x)=y(x)$.
- **Además,** si $h(x)$ es otra función (no necesariamente lineal), y $h(x_{0})=f(x_{0})$ y también $h'(x_{0})=f'(x_{0})$, entonces la recta $h$ y $f$ _comparten la recta tangente_.
  Ejemplo: 
	- $h(x)=1+sen(x) \longrightarrow h(0)=1=e⁰$.
	- $h'(x)=\cos(x) \longrightarrow h'(0)=1=e⁰$

---
Volviendo al problema de “mejorar” la precisión. Buscamos $P_{2}(x)$: $$P_{2}(x)=f(x_{0})+f'(x_{0})(x-x_{0})+coef?(x-x_{0})²$$
Tenemos que, $$P_{2}(x_{0})=f(x_{0})$$
$$P_{2}'(x)=f'(x_{0})+2*coef?(x-x_{0})$$
$$P_{2}''(x)=2*coef?$$
$$P_{2}'''(0) \equiv 0, \longrightarrow es \ el \ polinomio \ nulo$$
---
Si queremos la aproximación a orden 2:
$$P_{2}(x_{0})=f(x_{0})$$
$$P_{2}'(x_{0})=f'(x_{0}) \longrightarrow P_{2}'(x_{0})=f'(x_{0})+2*coef?*0=f'(x_{0})$$
$$P_{2}''(x_{0})=f''(x_{0}) \longrightarrow P_{2}''(x_{0})=2*coef?=f''(x_{0}) \longrightarrow coef?=\frac{f''(x_{0})}{2}$$

Finalmente, la fórmula para “la mejor aproximación de orden 2” será:
$$P_{2}(x)=f(x_{0})+f'(x_{0})(x-x_{0})+\frac{f''(x_{0})}{2!}(x-x_{0})²$$
