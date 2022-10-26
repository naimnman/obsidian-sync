# [[ANÁLISIS MATEMÁTICO I]]
---
# TEMA 8: PRIMITIVAS

## Problema de optimización

### Esquema "general"
- **Datos**
	- _Dominio = "Dominio del problema"_ (No necesariamente el dominio de la fórmula).
	- _Función objetivo = Fórmula._

**Pregunta (problem):** Hallar el valor máximo o mínimo, dependiendo del problema.

**"Con $10$ metros de cable, ¿puedo encerrar $8m²$? ¿Qué tipo de figura es la óptima?".**

La función objetivo será $A(x)=x(5-x)$, para un rectángulo.
Donde $x$ representa la longitud del lado, por lo que $x\geq_{0} \implies (5-x)\geq_{0} \iff x \leq 5$.
Esto nos indica que el **dominio del problema** será el siguiente: $[0,5]$.

---
### Problema de optimización de una lata.

Tenemos que hallar la fórmula de costo total para la manufacturación de una lata.

$$CT=C_{1} +C_{2} +C_{lata}$$
$$=2CT+C_{lata}=2*2Superficie_{tapa}+Superficie_{lata}$$
$$=4\cdot \frac{\pi D²}{4}+Perimetro*L$$
**y llegamos a la función objetivo:**
$$CT_{D}=\pi D²+\frac{4V}{D}$$

Luego, a partir de la función objetivo, planteamos el problema de optimización. En este caso, buscamos minimizar el costo total por medio del diámetro.

Nuestro dominio del problema será: $D>0$, $(0, \infty)$.

Luego, nos preguntamos si existe la solución.
**Teorema:** $f$ contenida en $[a,b]$ entonces $f$ alcanza su máximo y su mínimo absolutos.

Buscamos su derivada primera: $$CT'=$$
```ad-note
[Completar con filminas]
```

---

# Primitivas

A diferencia de antes, donde teníamos los datos ($f(x)=x³+3x+1$) y buscábamos el resultado ($f'(x)$), ahora requisamos a partir de un resultado ($f'(x)$) llegar a los distintos datos originales ($f(x)$'s).

```ad-info
Notas: 
1. **La primitiva no es única**, puede pasar $g_{1} \neq g_{2}$ y $g'_{1} = g'_{2}$
2. **Teorema:** $f: [a,b] \rightarrow \mathbb{R} continua \implies$ existe primitiva $F: [a,b] \rightarrow \mathbb{R}$. 
3. Aunque no hay unicidad, sí ocurre:
   - Si $F$ y $G$ son primitivas de $g$ ($F'\equiv G' \equiv g$) en $[a,b] \implies$ existe $c \in \mathbb{R}$ (**depende del intervalo**) tal que $F(x)-G(x)=c$. 
```

## Notación
Si $F$ es una primitiva de $f$ (osea $F'=f$), notaremos $\int f(x) dx = F(x)+c$ a la familia de primitivas.

### ¿Cómo se obtiene $F$?

_Difícil en general (si buscamos la "fórmula" sin la "viborita")._

Si aceptamos expresiones con $\int$ es inmediato!

Veremos:
- Proposiciones
- Métodos:
	- Sustituciones,
	- Partes,
	- Fracciones simples.
- ¿Para qué sirve? (par)
- ¿Cómo se usa?

```ad-tip
**NOTA:** COMPROBAR DERIVANDO LUEGO DE OBTENER LA PRIMITIVA. 
```

---

## Propiedad (linealidad)

1. $\int (f(x)`g(x)) \, dx = \int f(x) \, dx+\int g(x) \, dx$
   - Ejemplo: $\int (e^x+x²) \, dx=\int e^x \, dx+\int x² \, dx=e^x+\frac{x³}{3}+c$
2. $k \in \mathbb{R}$, $\int kf(x) \, dx=k\int f(x) \, dx$ 
   - Ejemplo: $\int 6\cos x \, dx=6\int \cos x \, dx=6sen x+c$
---

[Notas]

---
## Fracciones Simples:
Ejemplo: $\int \frac{lineal}{cuadrática\rightarrow (\triangle <0)}$ 
$$\frac{2-3t}{t²+t+2}$$
1. $\triangle = b²-4ac=1-8<0$
2. Completar cuadrados (escribir en forma canónica $\rightarrow \ z²+1$):
   $$t²+t+2=a(t-t_{v})²+y_{v}$$
	Vértice: $-\frac{b}{2a}=-\frac{1}{2}=t_{v}$
	$y_{v}=\left( -\frac{1}{2} \right)²-\frac{1}{2}+2=\frac{7}{4}$
	$a=1$
	$$t²+t+2=\left( t+\frac{1}{2} \right)²+\frac{7}{4}$$
3. Derivar denominador:
   $2t+1=2\left( t+\frac{1}{2} \right)$
4. Numerador | Denominador'
5. Escribimos $$\frac{-3t+2}{\left( t+\frac{1}{2} \right)²+\frac{7}{4}}=\left( \frac{(\frac{3}{2})(2t+1)}{\left( t+\frac{1}{2} \right)²+\frac{7}{4}} \right)\dots$$
etc.

---

## Fracciones simples
- Raíces múltiples.
- Raíces no reales.
  
### Caso raíces no reales:$\frac{3t+1}{(t-4)(t²+1)}$
#### Método:
1. Grado del denominador = $3$.
   Grado del numerador = $1<3?$ Sí.
2. #$coef= grado(Den)=3$
3. $$\frac{3t+1}{(t-4)(t²+1)}=\frac{A}{t-4}+\frac{B+Ct}{t²+1}$$
   $t=4 \rightarrow A$, $t={?} \rightarrow B$, $t={?} \rightarrow C$.
	Sumar, igualar numerador, "despear".

$3t+1=A(t²+1)+(t-4)(B+C \cdot t)=At²+A+tB+Ct²-4B-4Ct$
Para obtener cada coeficiente hacemos "como antes" (?) (para los coeficientes que tienen asociada una raíz).

$A \rightarrow t=4$, $3 \cdot 4+1=A(4²+1) \rightarrow \frac{13}{17}=A$

Los restantes? A mano pa.
- Estrategia 1: "igualar coeficientes"
	- $t² \rightarrow 0=A+C \rightarrow C=-A=-\frac{13}{17}$
	- $t\rightarrow 3=B-4C\rightarrow B=3+4C=3-4 \cdot\frac{13}{17}$
	- $t⁰ \rightarrow 1=A-4B$

### Caso raíces múltiples.
Ejemplo: $$\frac{2x²+5}{(x-1)²(x+2)}=\frac{A}{x+2}+\frac{B}{(x-1)²}+\frac{C}{(x-1)}$$
$grado(denominador)= 3 \rightarrow A,B,C$
$x=2 \rightarrow A$, $x=1 \rightarrow B,C$ (doble). Siendo $B$ el coeficiente de la potencia mayor. 

**Suma:**
$2x²+5=A(x-1)²+B(x+2)+C(x+2)(x-1)$
**A:** reemplazo $x=-2$, $$2(-2)²+5=A(-2-1)² \rightarrow \frac{13}{9}=A$$
**B:** reemplazo $x=1$, $$2 \cdot 1²+5=B(1+2) \rightarrow \frac{7}{3}=B$$
**Sugerencia: Para obtener los siguientes coeficientes a la raíz múltiple podemos; primero derivar y luego reemplazar en la raíz múltiple.**
$(2x²+5)'=$
$4x=2A(x-1)+B+C(x-1)+C(x+2),$ reemplazo $x=1$
$4=B+C(1+2)$

---

## Aplicaciones
- Cálculo de áreas/volúmenes.
	- "Integral definida": $$Área(a,b)=lím~(ancho)\rightarrow_{0} ~ \sum \foralláreas$$
	  $$\int^{b}_{a} f(x) \, dx $$
	  1. Si $f(x)>0$ en $[a,b] \implies \int^{b}_{a} f(x) \, dx=A$
	  2. Si $f(x)<0$ en $[a,b] \implies \int^{b}_{a} f(x) \, dx=-A$
	  3. Si $f(x)$ cambia de signo $\implies \int^{b}_{a} f(x) \, dx=A-A$
	     
¿Cómo se calcula el área?
$$A(R)= \int^{b}_{a}|f(x)-g(x)|\, dx$$
Si aparte calculamos $C⁺$ y $C⁻$, podemos confirmar en qué intervalos cuál de las funciones es mayor. $$A(R)=\int^{c}_{a}(g(x)-f(x)), dx+\int^{b}_{c}(f(x)-g(x)), dx$$

---
Ejemplo: Hallar el área encerrada por los gráficos de $\sqrt{x}$ y $x²$.
**Nota:** *¿Faltan los bordes lateral? No, estos serán los puntos de corte.*
$$f(x)=g(x) \rightarrow (\sqrt{ x })²=x⁴ \rightarrow x(x³-1)=0$$
Por lo que los bordes laterales serán $a=0$ y $b=1$. Tenemos que el intervalo de integración es $[0,1]$.
**Cálculo auxiliar:**
$h=\sqrt{ x }-x²$
[Foto]

---
### Regla de Barrow
$$\int^{b}_{a} h(t)\, dt=H(t) |^b_{a}:=H(b)-H(a)$$
donde $H$ es una primitiva de $h$ en $[a,b]$.

**Método:** 2 pasos!
1. Hallar la primitiva.
2. Hallar la variación.
   - $H(b)$
   - $H(a)$
   - Luego restar.
     
En el ejemplo $\int^{1}_{0}(\sqrt{ x }-x²)$