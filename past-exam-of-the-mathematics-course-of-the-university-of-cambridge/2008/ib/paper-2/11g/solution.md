<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

We prove the needed [Hilbert basis theorem](../../../../../hilbert-basis-theorem.md) step rather than assuming it. Suppose $A$ is a commutative [Noetherian ring](../../../../../noetherian-ring.md) and $I\subseteq A[X]$ is an ideal. The set $J$ of leading coefficients of elements of $I$, together with zero, is an ideal of $A$: align degrees with powers of $X$ before addition, and use scalar multiplication. Choose finitely many generators of $J$, represented by polynomials $f_1,\ldots,f_s\in I$, and let $d$ be the maximum of their degrees. If $J=0$ then $I=0$ and there is nothing to prove.

For each $0\le j<d$, let $J_j$ consist of the coefficients of $X^j$ of elements of $I$ of degree at most $j$. This is also an ideal of $A$; choose finitely many generating coefficients and representing polynomials $g_{j,l}\in I$ of degree at most $j$. The finite collection of all $f_i$ and $g_{j,l}$ generates $I$: for any $h\in I$ of degree $m\ge d$, express its leading coefficient using those of $f_i$ and subtract the matching combination of $X^{m-\deg f_i}f_i$ to lower degree. When the degree becomes $j<d$, use the representatives of $J_j$ to lower it again. Induction on degree eventually leaves zero.

A field is Noetherian because its only ideals are zero and the whole field. Repeatedly applying the proved step gives **every ideal of $\boxed{F[X_1,\ldots,X_n]}$ finitely generated.**

The coefficient restriction in the second ring says precisely

$$
R=F+XYF[X,Y].
$$

It contains one and is closed under addition, additive inverses and multiplication: $(a+XYp)(b+XYq)=ab+XY(aq+bp+XYpq)$. To show it is not Noetherian, consider the ideals in $R$

$$
I_d=(XY,XY^2,\ldots,XY^d)_R,\qquad d\ge1.
$$

They form an ascending chain. In any $\sum_{j=1}^d r_jXY^j$ with $r_j\in R$, the coefficient of $X^1$ is a polynomial in $Y$ of degree at most $d$, since the nonconstant part of $r_j$ introduces at least $X^2$. It cannot equal $XY^{d+1}$; hence $I_d\subsetneq I_{d+1}$. If the union ideal were finitely generated, all its generators would lie in one $I_d$, forcing the chain to stabilize. This contradiction proves $\boxed{R\text{ is not Noetherian}}$, the [constant-plus-ideal non-Noetherian subring](../../../../../constant-plus-ideal-non-noetherian-subring.md) example.

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
