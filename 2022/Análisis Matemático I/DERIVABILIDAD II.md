# [[ANÁLISIS MATEMÁTICO I]] 
---

# TEMA 7: DERIVABILIDAD II

# Otras aplicaciones
“Estudio”
Hacer tabla de valores: Muy costoso.
Preferimos: Buscar “puntos notables”,
- $C⁰(f)=\text{ceros de f}$
- Vértices.
- Descanso. 
- Máx.
- Mín.
- Bordes del dominio/cambio de fórmula.

Ya tenemos
1. Dominio (provisional).
2. Continuidad (agrandar el dominio si es posible).
3. $C⁰(f) \longrightarrow C⁺(f), C⁻(f)$.
4. "Monotonía" $\longrightarrow$ Extremos locales (máx y mín).
   La monotonía (creciente o decreciente) está guardado en el signo de $f'$. El esquema de trabajo será:
   - Analizar la existencia de $f'$ (derivabilidad de $Dom(f')$).
   - Hallar la fórmula derivando (por tabla).
   - “Puntos críticos”:
      - Singulares (dónde no hay derivada): no existe $f'$.
      - Regulares (los ceros de la derivada): $[x\in Dom(f'): f'(x)=0]$
      - Intervalos de crecimiento y decrecimiento.
---
## Resultados teóricos útiles:
**Teorema:** $f:[a,b] \longrightarrow \mathbb{R}$ tal que $f$ es derivable en el intervalo $J$ y $f'(x)>0$, **entonces $f$ es estrictamente creciente en $J$** (es decir, $x_{1}<x_{2}$ en $J \implies f(x_{1})<f(x_{2})$.
Asimismo, sea $f$ derivable en $J$ pero $f'(x)<0$, **entonces $f$ es estrictamente decreciente en $J$**.

---
==Nota:== _Si $f$ es estrictamente creciente o decreciente, entonces $f$ es **inyectiva**._
==Nota:== $f(x)= \frac{1}{x} \implies f’(x)=-\frac{1}{x²}<0 \implies$ $f$ es decreciente en los intervalos $(0, \infty)$ y $(-\infty, 0)$.
==Nota:== $f: J \rightarrow \mathbb{R}$, _entonces $f$ es contínua e inyectiva_ $\implies f$ **es estríctamente monótona**.

---
**Teorema:** $f: [a, b] \rightarrow  \mathbb{R}$, y es contínua y estrictamente creciente, entonces la $Img(f)=[f(a), f(b)]$.
- $x=a$, mínimo absoluto.
- $x=b$, máximo absoluto.
- $f(a)$ es el valor mínimo.
- $f(b)$ es el valor máximo.
Si en vez de ser estictamente creciente es estrictamente decreciente, entonces los valores se invierten, $Img(f)=[f(b), f(a)]$.

---
Tenemos acceeso a la imagen de cada intervalo de monotonía, pero, si $J$ no tiene algún borde?
Ejemplo: $f(x)= \frac{1}{x}$, $(0, \infty)$

**Teorema:** $J=(a, b]$, $f: J \rightarrow \mathbb{R}$, y es estrictamente monótona y contínua, entonces existen los límites;
- $lím\ x \rightarrow a⁺ \ f(x)= -\infty \lor +\infty=f(a^+)$
- $lím\ x \rightarrow b⁻ \ f(x)=f(b)=f(b⁻)$

**Teorema:** Si $f$ es derivable en $(a,b)$ y $f'(x) \neq 0$ en $(a,b)$, entonces el signo de la derivada es constante.
- Elijo $x_{0} \in (a,b)$;
	- $f'(x_{0})>0 \longrightarrow f$ es creciente en $(a,b)$
	- $f'(x_{0})<0 \longrightarrow f$ es decreciente en $(a,b)$.
Y en cada intervalo la imagen se calculará haciendo 
- $(f(a⁺), f(b⁻))$ creciente.
- $(f(b⁻), f(a⁺))$ decreciente.

