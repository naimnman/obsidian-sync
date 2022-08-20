# TEMA 1: CONJUNTOS
- Se definen con una letra latina mayúscula. Un conjunto está bien definido cuando es posible precisar sus elementos. 
- Ejemplos de estos pueden ser; N, Z, Q, R, C.
	- N = {0, 1, 2, 3, 4...}
	  Z = {...-3, -2, -1, 0, 1, 2, 3...}
	  A = {x: x ∈ N && x<5}

### Elementos 
- Se definen con una letra latina minúscula. Estos son los que integran  un conjunto.
  El orden de estos es irrelevante, ya que el conjunto está definido por sus elementos contenidos.

## Propiedades de los conjuntos:
- ### Inclusión: 
  Dados dos conjuntos A y B, s dice que A está incluido en B, o que A es un subconjunto de B, _si todo elemento de A pertenece a B_.
  Se escribe A ⊆ B o B ⊇ A.
	![[Pasted image 20220816085548.png]]
	- **Propiedades de la inclusión:**
	  1. Reflexiva: A ⊆ A, para todo conjunto A.
	     [HACER DIAGRAMA DE VENN]
	  2. Antisimétrica: Si A ⊆ B y B ⊆ A entonces A = B.
	     [HACER DIAGRAMA DE VENN]
	  3. Transitiva: Si A ⊆ B y B ⊆ C entonces A ⊆ C.
	     [HACER DIAGRAMA DE VENN]
	- **Plantilla de demostración de inclusión:** [INVESTIGAR]
	- __Plantilla de demostración por doble inclusión:__ 
		1. Probar que A ⊆ B.
		2. Probar que B ⊆ A.
		3. Por lo tanto, A = B.


### Conjunto de partes de un conjunto:
- Este se define como el conjunto cuyos elementos también son conjuntos.
  Dado un conjunto A, se denota el conjunto de partes de A como P(A), donde se incluyen todos los subconjuntos, incluido el vacío (no confundir con pertenencia, ya que no es general) y sí mismo.
  ![[Pasted image 20220816095958.png]] 
  Un ejemplo puede ser el conjunto de los números Reales, donde se contienen los conjuntos N, Z, Q, etc.

#### Propiedades absolutas de conjuntos definidos:
- Real + Real = Real.
- Irracional + Irracional = no absoluto.

---
## Unión de conjuntos:
- Dados dos conjuntos A y B, se llama unión de A y B, y se indica A∪B, al conjunto formado por todos los elementos que pertenecen a A o a B. En notación $$A ∪ B = {x : x ∈ A~o~ x ∈ B}.$$
- [DIAGRAMA DE VENN]

### Propiedades de la unión:
1. __Idempotente:__ _A ∪ A = A._
   Para demostrar la igualdad de los conjuntos A ∪ A y A hay que probar las dos inclusiones: (i) A ∪ A ⊆ A y (ii) A ⊆ A ∪ A. Ya vimos que (ii) es consecuencia inmediata de la definición. Probemos (i), esto es que todo elemento de A∪A es un elemento de A. Sea x ∈ A∪A. Entonces x ∈ A ó x ∈ A, luego x ∈ A. Se tiene entonces A ∪ A ⊆ A. De (i) y (ii) sigue la igualdad.
2. __Conmutativa:__ _A ∪ B = B ∪ A._
3. __Asociativa:__ _(A ∪ B) ∪ C = A ∪ (B ∪ C)._
   De forma simple, la unión del primero con el segundo, unido al tercero es igual al primero  unido a la unión del segundo y el tercero.
   [DIAGRAMA DE VENN]
---
## Intersección de conjuntos:
- Dados dos conjuntos A y B, se llama intersección de A y B, y se indica A ∩ B, al conjunto cuyos elementos son los elementos comunes a A y a B, es decir los elementos que pertenecen simultáneamente a los dos conjuntos. $$A ∩ B = {x : x ∈ A ~y~ x ∈ B}.$$
- [DIAGRAMA DE VENN]
- De la definición se desprende que A ∩ B ⊆ A _y_ A ∩ B ⊆ B, cabe recalcar que _este 'y'_ es excluyente. 
### Propiedades de la intersección:
1. __Idempotente:__ _A ∩ A = A._ 
2. __Conmutativa:__ _A ∩ B = B ∩ A._ 
3. __Asociativa:__ _(A ∩ B) ∩ C = A ∩ (B ∩ C)._

#### Leyes de absorción: 
1. __A ∪ (A ∩ B) = A.__ Como A ∩ B ⊆ A, entonces por el teorema 1 resulta A ∪ (A ∩ B) = A. 
2. __A ∩ (A ∪ B) = A.__ Como A ⊆ A ∪ B, entonces por el teorema 2 resulta A ∩ (A ∪ B) = A.

#### Leyes distributivas: 
1. __A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C).__ 
2. __A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C).__
[DEMOSTRACIÓN]

---
## Complemento:
- Dados dos conjuntos A y B, tales que A ⊆ B, se llama complemento de A relativo a B, y lo notamos CBA, _al conjunto formado por todos los elementos de B que no pertenecen a A._ $$CBA = {x : x ∈ B ~y~ x ∉ A}.$$
- [DIAGRAMA DE VENN]

---

## Diferencia:
- Dados dos conjuntos A y B, se llama diferencia entre A y B, en ese orden, al conjunto formado por los elementos que pertenecen a A y no pertenecen a B. Se nota A − B. $$A − B = {x : x ∈ A ~y~ x ∉ B}.$$
- [DIAGRAMA DE VENN]

### Propiedad de diferencia:
- __A − B = A ∩ B'.__

### Leyes de De Morgan. 
1. __(A ∩ B)' = A' ∪ B'.__ 
2. __(A ∪ B)' = A' ∩ B'.__
---

## Producto cartesiano:
- Dados dos conjuntos A y B, y objetos cualesquiera a ∈ A y b ∈ B, _consideraremos __pares ordenados__ de primera coordenada a y segunda coordenada b_, que notaremos _(a, b)_. Dos pares ordenados (a, b) y (a', b') son iguales si y sólo si a=a' y b=b'.
- __Definición:__ Dados dos conjuntos A y B, llamamos producto cartesiano de A y B, y lo notamos A × B, al conjunto formado por todos los pares ordenados (a, b), con a ∈ A y b ∈ B. Es decir, $$A × B = {(a, b) : a ∈ A ~y~ b ∈ B}.$$
- El producto cartesiano de A por B se suele representar en el plano considerando dos rectas perpendiculares. Los elementos de A se representan por puntos sobre la recta horizontal, y los elementos de B se representan por puntos sobre la recta vertical. Cada elemento (a, b) de A × B se representa por el punto del plano que se obtiene como intersección de rectas perpendiculares a los ejes por los puntos que corresponden a a y a b.
- [REPRESENTACIÓN DE PLANO CARTESIANO]
- Al producto cartesiano A × A se lo nota A^2. Si A ≠ B, entonces A × B ≠ B × A.

---
#GLOSARIO 
- **Elemento genérico:** algún elemento perteneciente al conjunto el cual no es determinado, normalmente representado por una letra minúscula.
- **Conjunto Vacío (∅):** Este conjunto no tiene ningún elemento, _por lo que está contenido en en cuaqluier conjunto_. Este se define por cualquier propiedad que no sea verificada por ningún objeto.
- __Contenido:__ Un objeto está contenido dentro de otro conjunto cuando cada uno de sus elementos pertenece a dicho conjunto.
- __Perteneciente:__ Un objeto pertenece a un conjunto cuando forma parte de los elementos del mismo.
- __Contraejemplo:__ un caso excepcional (o no) que implica que cierta afirmación no se cumple. Un único contraejemplo ya es suficiente para probar falsa respectiva afirmación.
- __Si y solo si:__ Entre dos afirmaciones, el conector si y solo si se utiliza cuando la primera afirmación implica una segunda afirmación, esto asumiendo que la primera es verdadera. Luego, a partir de la segunda afirmación, y asumiendo que es verdadera, se llega a la primera afirmación por implicación. Esta implicación inversa se denomina _recíproca_.