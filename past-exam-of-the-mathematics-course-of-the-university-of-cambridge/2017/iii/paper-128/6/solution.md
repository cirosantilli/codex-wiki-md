<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [derivation of an algebra](../../../../../derivation-of-an-algebra.md) is a $k$-linear map $D:A\to A$ satisfying $D(ab)=D(a)b+aD(b)$. The [commutator](../../../../../commutator.md) $[D,E]=D\circ E-E\circ D$ is again a [derivation](../../../../../derivation-of-an-algebra.md): expanding $[D,E](ab)$ cancels the two mixed terms and leaves $[D,E](a)b+a[D,E](b)$. The [commutator](../../../../../commutator.md) on [endomorphisms](../../../../../endomorphism.md) is bilinear, antisymmetric, and satisfies the [Jacobi identity](../../../../../jacobi-identity.md) by cancellation of its twelve triple-composition terms. Therefore **$\operatorname{Der}_k(A)$ is a [Lie algebra](../../../../../lie-algebra-split.md)**.

In degree zero of the [Hochschild cochain complex](../../../../../hochschild-cochain-complex.md), $\delta a(b)=ba-ab$, so $HH^0(A,A)=Z(A)=A$ for commutative $A$. In degree one, $\delta D=0$ is precisely the [derivation](../../../../../derivation-of-an-algebra.md) rule; the boundaries are [inner derivations](../../../../../inner-derivation.md), which vanish for commutative $A$. Hence

$$
\boxed{HH^0(A,A)=A,\qquad HH^1(A,A)=\operatorname{Der}_k(A).}
$$

For cochains $f\in C^p(A,A)$, $g\in C^q(A,A)$, the [Hochschild cup product](../../../../../hochschild-cup-product.md) is

$$
(f\smile g)(a_1,\ldots,a_{p+q})=f(a_1,\ldots,a_p)g(a_{p+1},\ldots,a_{p+q}).
$$

Define the insertion operation by

$$
f\circ g=\sum_{i=0}^{p-1}(-1)^{i(q-1)}f(a_1,\ldots,a_i,g(a_{i+1},\ldots,a_{i+q}),a_{i+q+1},\ldots,a_{p+q-1}).
$$

A degree-zero cochain is an element of $A$, inserted with no arguments; for $p=0$ the sum is empty. For the [Gerstenhaber bracket](../../../../../gerstenhaber-bracket.md) we use the left [graded Leibniz rule](../../../../../graded-leibniz-rule.md) convention, compatible with the unsigned [Hochschild cup product](../../../../../hochschild-cup-product.md) just displayed:

$$
\boxed{[f,g]=(-1)^{(p-1)(q-1)}f\circ g-g\circ f.}
$$

Both degree-zero inputs have bracket zero. Another common insertion convention writes $f\circ g-(-1)^{(p-1)(q-1)}g\circ f$; the two brackets differ by $(-1)^{(p-1)(q-1)}$. With an unsigned [Hochschild cup product](../../../../../hochschild-cup-product.md), that convention uses the corresponding right [graded Leibniz rule](../../../../../graded-leibniz-rule.md). The distinction matters for a degree-two cochain bracketed with a function. Either consistent convention gives the same degree-one [Lie bracket](../../../../../lie-bracket.md) and the same [derivation](../../../../../derivation-of-an-algebra.md) action on functions.

If $m(a,b)=ab$, this convention gives $\delta f=[m,f]$. The shifted [Jacobi identity](../../../../../jacobi-identity.md) and $[m,m]=0$ therefore show that the [Gerstenhaber bracket](../../../../../gerstenhaber-bracket.md) respects [Hochschild cocycles](../../../../../hochschild-cocycle.md) and the images of the [coboundary map](../../../../../coboundary-map.md). The [Hochschild cup product](../../../../../hochschild-cup-product.md) and [Gerstenhaber bracket](../../../../../gerstenhaber-bracket.md) induce operations on [Hochschild cohomology](../../../../../hochschild-cohomology.md). A [Gerstenhaber algebra](../../../../../gerstenhaber-algebra.md) is a [graded algebra](../../../../../graded-algebra.md) $H$ with an associative degree-zero product with the [graded commutative algebra](../../../../../graded-commutative-algebra.md) rule $uv=(-1)^{pq}vu$, and a degree-minus-one [graded Lie bracket](../../../../../graded-lie-bracket.md) making the shifted degrees $|u|-1$ into a [graded Lie algebra](../../../../../graded-lie-algebra.md). In particular,

$$
[u,v]=-(-1)^{(p-1)(q-1)}[v,u],\qquad
[u,vw]=[u,v]w+(-1)^{(p-1)q}v[u,w]
$$

for [homogeneous elements of a graded algebra](../../../../../homogeneous-element-of-a-graded-algebra.md) of degrees $p,q$. The shifted [Jacobi identity](../../../../../jacobi-identity.md) is

$$
[u,[v,w]]=[[u,v],w]+(-1)^{(p-1)(q-1)}[v,[u,w]].
$$

The [Hochschild cup product](../../../../../hochschild-cup-product.md) does not make the cochains a [graded commutative algebra](../../../../../graded-commutative-algebra.md) in general, but does make their [cohomology](../../../../../cohomology-split.md) a [graded commutative algebra](../../../../../graded-commutative-algebra.md); the insertion operation supplies the homotopy for this assertion and for the [graded Leibniz rule](../../../../../graded-leibniz-rule.md). Thus these axioms describe the induced [Gerstenhaber algebra](../../../../../gerstenhaber-algebra.md), not a claim of a [graded commutative algebra](../../../../../graded-commutative-algebra.md) structure on the cochain multiplication itself.

For $A=k[X]$, the enveloping [algebra](../../../../../algebra-split.md) is $A^e=k[X_\ell,X_r]$, and

$$
0\longrightarrow A^e\xrightarrow{\ X_\ell-X_r\ }A^e\longrightarrow A\longrightarrow0
$$

is a [projective resolution](../../../../../projective-resolution.md). The first map is injective since $A^e$ is an [integral domain](../../../../../integral-domain.md), and its [cokernel](../../../../../cokernel.md) is $A$. Applying $\operatorname{Hom}_{A^e}(-,A)$ gives a zero [coboundary map](../../../../../coboundary-map.md). Consequently

$$
\boxed{HH^*(k[X],k[X])=k[X]\otimes_k\Lambda(\partial_X),\qquad |\partial_X|=1.}
$$

The [Hochschild cup product](../../../../../hochschild-cup-product.md) is ordinary multiplication of functions and scalar multiplication of [derivations](../../../../../derivation-of-an-algebra.md), with the product of two [derivations](../../../../../derivation-of-an-algebra.md) zero because $HH^2=0$. Every [derivation](../../../../../derivation-of-an-algebra.md) is $f\partial_X$, since it is determined by its value on $X$. The [Gerstenhaber bracket](../../../../../gerstenhaber-bracket.md) is

$$
[f\partial_X,g\partial_X]=(fg'-gf')\partial_X,\qquad [f\partial_X,h]=fh',\qquad [h_1,h_2]=0,
$$

with all other orders fixed by graded antisymmetry. These formulas fully determine the [Gerstenhaber algebra](../../../../../gerstenhaber-algebra.md).

For $A=k[X,Y]$, the [Hochschild-Kostant-Rosenberg theorem](../../../../../hochschild-kostant-rosenberg-theorem.md) identifies

$$
\boxed{HH^*(A,A)=\bigwedge_A^*\operatorname{Der}_k(A)=A\otimes_k\Lambda(\partial_X,\partial_Y).}
$$

Thus the degrees zero, one, and two are $A$, $A\partial_X\oplus A\partial_Y$, and $A(\partial_X\wedge\partial_Y)$, and all higher groups vanish. The [Hochschild-Kostant-Rosenberg](../../../../../hochschild-kostant-rosenberg-theorem.md) map sends a wedge of $p$ [derivations](../../../../../derivation-of-an-algebra.md) to the cochain

$$
\frac1{p!}\sum_{\sigma\in S_p}\operatorname{sgn}(\sigma)\prod_{j=1}^p D_{\sigma(j)}(a_j).
$$

The factorial is invertible in [characteristic](../../../../../characteristic-of-a-field.md) zero. Equivalently, the groups follow from the [Koszul resolution](../../../../../koszul-resolution.md) on the [regular sequence](../../../../../regular-sequence.md) $X_\ell-X_r,Y_\ell-Y_r$ in $A^e$, whose dual [coboundary maps](../../../../../coboundary-map.md) vanish on $A$.

The [Hochschild cup product](../../../../../hochschild-cup-product.md) becomes the [exterior product](../../../../../exterior-product.md), and our [Gerstenhaber bracket](../../../../../gerstenhaber-bracket.md) becomes the left [Schouten-Nijenhuis bracket](../../../../../schouten-nijenhuis-bracket.md). It is determined by the [commutator](../../../../../commutator.md) of [derivations](../../../../../derivation-of-an-algebra.md), $[D,f]=D(f)$, zero brackets of functions, and the displayed graded antisymmetry and left [graded Leibniz rule](../../../../../graded-leibniz-rule.md). For explicit signs, put $\Pi=\partial_X\wedge\partial_Y$ and $D=F\partial_X+G\partial_Y$. Then

$$
[h\Pi,f]=h(f_Y\partial_X-f_X\partial_Y),\qquad [D,h\Pi]=(D(h)-h(F_X+G_Y))\Pi,\qquad [h\Pi,j\Pi]=0.
$$

The last bracket has degree three, whose [exterior power](../../../../../exterior-power.md) is zero. For two [derivations](../../../../../derivation-of-an-algebra.md), the coefficient functions of their [commutator](../../../../../commutator.md) give the remaining formula. This specifies the entire [Gerstenhaber algebra](../../../../../gerstenhaber-algebra.md); under the alternate insertion convention mentioned above, the first displayed bracket changes sign, together with the Leibniz convention. No smoothness of a general finitely generated commutative [algebra](../../../../../algebra-split.md) was assumed: the [Hochschild-Kostant-Rosenberg theorem](../../../../../hochschild-kostant-rosenberg-theorem.md) is invoked here only for the smooth [polynomial ring](../../../../../polynomial-ring.md) $k[X,Y]$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 128](../../paper-128-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
