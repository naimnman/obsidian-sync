# [[ANÁLISIS MATEMÁTICO I]]
---
# TEMA 1: LOS NÚMEROS __Monotonía__ 
		- _Creciente:_ una función es creciente cuando conserva desigualdades. 
		  Cuando $a>1$, $a^x$ y $log_{a}~x$ __son crecientes__
		  Ejemplo: $-1<2$ = $(-1)²<2²$ = $1<4$.
		- _Decreciente:_ una función es decreciente cuando invierte las desigualdades. 
		  Cuando $0<a<1$, $a^x$ y $log_{a}~x$ __son decrecientes.__ 
		  Ejemplo: $-2<1$ → $(-2)²>1²$ → $4>1$..

## Conjuntos numéricos:
- __Naturales:__ 
	- Ordinales: Aquellos que siven para ordenar; _1°, 2°, 3°, 4°..._
	- Cardinales: Aquellos que sirven para contar; _0, 1, 2, 3, 4..._
- __Enteros:__ a partir de la expansión de los naturales, se agrega la noción de opuestos.
	-  _...-3, -2, -1, 0, 1, 2, 3..._
- __Racionales:__ a partir de la expansión de los números enteros, se crea este conjunto de manera que es posible expresar valores numéricos como el cociente de dos números, _p_ y _q_.
	- Notación fraccional: _½, ⅝, ⅛, etc._
	- Notación decimal: _0.2, 1.16, etc._
	- $$Q := {[\dfrac{p}{q}: p ∈ Z ~y~ q ∈ N ]}$$
	- __Ordenamiento de fracciones:__  Al igualar los denominadores de dos fracciones, se vuelve trivial comparar su tamaño ya que solo debemos comparar el numerador.
- __Reales:__ ALL OF THEM (almost).$$R=[0]∪[S*a_0·a_1·a_2·a_3...*10^{m∈Z}]$$
![[conjuntosNumericos.png]]
### Pertenencia e inclusión:
La inclusión, denotada por ⊆, se da entre conjuntos, mientras que la pertenenia, denotada por el símbolo ∈, se da entre un elemento y un conjunto (y en ese orden).
#### Densidad en los números racionales:
- Esta propiedad característica del conjunto racional nos asegura que entre dos números racionales R1 y R2, es posible encontrar otro número de la misma especie. Una forma sencilla de encontrarlo es mediante el promedio de R1 y R2. 
#### Arquimedianidad:
- Esta propiedad nos dice que con una regla arbitrariamente pequeña, y con mucha pa-
ciencia, podemos medir longitudes arbitrariamente grandes. Simbólicamente, esta propiedad se expresa:
Sean 0 < a, M ∈ R dos números reales positivos cualesquiera. Entonces existe k ∈ N tal que M < k · a.
Aquí, a es la regla, M es el objeto a medir y k ∈ N es la cantidad de veces que hay que poner la regla a continuación de sí misma para superar el valor de M (es decir, el tamaño de la paciencia).
De manera informal, se puede expresar como la propiedad de no tener elementos infinitamente grandes ni infinitamente pequeños. A partir de esto, podemos llegar a que no hay número real más grande que cualquier número natural.

---

## Notación científica:
- __Dígitos significativos:__ Son aquellas cifras las cuales son distintas de cero, aunque también los ceros entre dos significativos también lo son y, pofloat double long double visual ranger último, los ceros al final de la parte decimal.
- __Órden de magnitud:__ Indica la magnitud (tamaño tangible) del número a representar, se ve reflejado directamente en el exponente.
- __Mantisa:__ La mantisa de un número decimal sería la parte fraccionaria, prescindiendo de su parte entera. Ex: Dado el número 12.31415, la mantisa sería 0,31415.

---
# Potenciación
## Propiedades:
- __Producto de potencias de igual base:__ En un producto este estilo, se suman los exponentes y se mantiene la base.
- __Potencia de una potencia:__ Al encontrarse con una potencia elevada a otra potencia, se mantiene la base  y se multiplican los exponentes.

---
# Logaritmo: 
- _"La división repetida es el logaritmo"_
- __Definición:__ Un logaritmo expresa potenciación, o sea, indica el exponente por el cual se debe elevar la base para obtener la potencia indicada. De esta forma podemos hacer la correlación entre un logaritmo y la potenciación siendo los siguientes términos equivalentes: Exponente = logaritmo. Potencia = número. $$2^x=5 ~;~ x=log_2~5$$
- __Identidad fundamental:__
  Dado un $x>0$ y un $r>0$ y $r≠1$, podemos escribirlo de la siguiente manera: $$x=r^{log_r~128}$$
-  __Cambio de base:__ $${log_r~x = \dfrac{log~x}{log~r}}$$

---
## Propiedades de los Reales:
### Completitud:
Llamada axioma de completitud, esta garantiza una correspondencia biunívoca (uno a uno) entre el conjunto de los números reales y el conjunto de puntos en la recta o eje.
Daremos las dos versiones una con ínfimo y la otra con supremo estableciendo que son equivalentes:
- Todo conjunto no vacío y acotado inferiormente tiene ínfimo.
- Todo conjunto no vacío y acotado superiormente tiene supremo.
---

[TODO LO Q ME FALTA XD]
---

# Funciones Trascendientes

## Funciones exponenciales:
- __Básicas:__ $f(x)=a^x$. Para que esto se cumpla, $a > 0$ y $a ≠ 1$ con $a$ pertenenciente a los números reales.
	- Dominio = R.
	- Imagen: (0;+∞). Esto quiere decir $a^x=b>0$.
	- La función tiene su inversa: $log_{a}~x: (0, ∞)$ 
	- La distribución del logaritmo en un producto: $$log_{a}~(u*v)=log_{a}~u+log_{a}~v$$ Con $u>0$ y $v>0$.
	- El logaritmo de un número exponencial: $$log_{a}~(u^r)=r*log_{a}~u$$
	- __Es inyectiva:__ $a^x=a^z$ => $x=z$.
	- __Es sobreyectiva:__ $a^x: R$ => Codominio: (0, ∞).
		- Debido a que es _inyectiva_ y _sobreyectiva_, podemos decir que es __biyectiva__.
	-  __Monotonía__ 
		- _Creciente:_ una función es creciente cuando conserva desigualdades. 
		  Cuando $a>1$, $a^x$ y $log_{a}~x$ __son crecientes__
		  Ejemplo: $-1<2$ = $(-1)²<2²$ = $1<4$.
		- _Decreciente:_ una función es decreciente cuando invierte las desigualdades. 
		  Cuando $0<a<1$, $a^x$ y $log_{a}~x$ __son decrecientes.__ 
		  Ejemplo: $-2<1$ → $(-2)²>1²$ → $4>1$.
## Funciones Trigonométricas:
- Semejanza: Implica proporcionalidad, si los lados son iguales, los ángulos también lo serán.

- Índice de periodicidad: A partir de $
- Relación de $t_1$ y $t_2$: [FOTO]
	- $t_{1}+t_{2}=$


---
#GLOSARIO 
- Biyectiva: <iframe src="https://es.wikipedia.org/wiki/Biyectiva" allow="fullscreen" allowfullscreen="" style="height:100%;width:100%; aspect-ratio: 16 / 9; "></iframe> 
- 