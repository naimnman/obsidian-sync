# [[ELEMENTOS DE ÁLGEBRA Y GEOMETRÍA]]
---

# TEMA 2: RELACIONES BINARIAS
- En Matemática la noción de relación es de mucha importancia. Definir una relación R es fijar una ley que permita decir para cada par de objetos a y b, cuándo a está en la relación R con b. Por ejemplo, si R es la relación ≤ entre números naturales, entonces 4R6, o escrito de otra forma, (4, 6) ∈ R.
- __Definición:__ Dados dos conjuntos A y B, una relación binaria R entre los elementos de A y los elementos de B (o en A × B), es un subconjunto (R) del producto cartesiano A × B: $$R ⊆ A × B.$$
  Se escribe aRb si (a, b) ∈ R. En particular, si A = B, entonces R se llama una relaci´on binaria en A.
---
## Propiedades de las relaciones binarias

### Reflexiva:
Dada una relación R ⊆ A × A, diremos que R es reflexiva si aRa para todo a ∈ A. ((a, a) ∈ R para todo a ∈ A).
Ejemplos:
- Paralelismo: Sea A en conjunto de todas las rectas de un plano. Si l1, l2 ∈ A, (l1, l2) ∈ R ⇔ l1 es paralela a l2.
- A = {1, 2, 3}, R = {(1, 1),(2, 2),(3, 3),(1, 2),(2, 1)}.
- La igualdad: Si x, y ∈ A y R está definida por (x, y) ∈ R ⇔ x = y.
- La relación “divide” en N. Dados a, b ∈ N definimos la siguiente relación: aRb ⇔ a divide a b, o sea, existe k ∈ N tal que b = k·a. En lugar de aRb notaremos a|b. Esta relación es reflexiva: a|a, para todo a ∈ N, pues a = k·a con k = 1.
_Para ver si R es reflexiva, tengo que analizar si para todo a ∈ A, se tiene (a,a) ∈ R._
De forma sencilla, para que haya reflexividad cada elemento debe estár relacionado consigo mismo.
[DIAGRAMA CARTESIANO], [DIAGRAMA DE FLECHAS]

### Simétrica:
Diremos que una relación R ⊆ A×A es simétrica si se verifica que: Si aRb entonces bRa. $$(a, b) ∈ R ⇒ (b, a) ∈ R.$$
Ejemplos:
- Perpendicularidad: Sea A en conjunto de todas las rectas de un plano. Si l1, l2 ∈ A, entonces (l1, l2) ∈ R ⇔ l1 es perpendicular a l2.
- A = {a, b, c}, R = {(a, b),(a, c),(b, a),(c, a)}.
- A = {1, 2, 3}, R = {(1, 1),(2, 3),(3, 2)}.
_Para ver si R es simétrica, tengo que analizar si para cada (a,b) ∈ R, se tiene (b,a) ∈ R._
De forma simple, para que haya simetría, cada relación que se presente entre elementos debe darse por ambos sentidos, (a,b) y (b,a).
[DIAGRAMA CARTESIANO], 
![[Pasted image 20220823092926.png]]


### Anti-simétrica:
R se dice antisimétrica si se verifica que si aRb y bRa, entonces a = b. Esto se demuestra mediante; $$(a, b) ∈ R ~y~ (b, a) ∈ R ⇒ a = b$$
Equivalentemente: Si a ≠ b entonces aR/b o bien bR/a. (a ≠ b ⇒ (a, b) ∈/ R o bien (b, a) ∈/ R).
_Para demostrar que R **NO es antisimétrica** hay que recorrer la lista de elementos y si se halla un par (a,b) ∈ R con a ≠ B, entonces el par opuesto (b,a) ∈/ R._ 
Ejemplo: 
- R no es antisimétrica.
	- Justificación: (1,2) ∈ R, (2,1) ∈ R, pero 1 ≠ 2.
![[Pasted image 20220823093733.png]]



### Transitividad:
R se dice transitiva si se verifica que __aRb y bRc entonces aRc.__
$$(a, b) ∈ R ~y~ (b, c) ∈ R ⇒ (a, c) ∈ R.$$
Ejemplos:
1. Paralelismo de rectas en el plano.
2. $A = {1,2,3,4}, R = [(1,2),(2,4),(1,4)].$
3. La relación divide en $N$. Si $a|b$ y $b|c$ entonces $a|c$. De a|b resulta que existe k ∈ N tal que b = k·a. De b|c, existe k' ∈ N tal que c = k' · b. Reemplazando se tiene: c = k · k' · a, de donde c = k'' · a, k'' ∈ N, y por lo tanto a|c.
[DIAGRAMA CARTESIANO], [DIAGRAMA DE FLECHAS]
---

## Relaciones de equivalencia.
Una relación R en A es una relación de equivalencia si es __reflexiva, simétrica y transitiva.__
Las siguientes expresiones definen relaciones de equivalencia (en conjuntos apropiados):
- Nació en el mismo mes que
- Tiene tantas sílabas como
- Empieza con el mismo dígito que

### Partición de un conjunto:
Dado un conjunto A, diremos que una familia $[Ai]_{i∈I}$ de subconjuntos de A constituye una partición de A si:
1. $Ai ≠ ∅$, para todo $i ∈ I$,
2. Si $i ≠ j$ entonces $Ai ∩ Aj = ∅$,
3. $∪_{i∈I}~Ai=A$ -> donde $∪_{i∈I}~Ai = {x : x ∈ Ai}$, para algún $i ∈ I$.
__Es decir, todos los subconjuntos de la familia son no vacíos, son disjuntos dos a dos y su unión es A.__
[DIAGRAMA DE CONJUNTOS Y SUBCONJUNTOS]
