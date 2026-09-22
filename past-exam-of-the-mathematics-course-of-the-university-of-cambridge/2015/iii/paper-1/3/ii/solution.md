<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The key is a [Laurent normalization by a monomial change of variables](../../../../../../laurent-normalization-by-a-monomial-change-of-variables.md). We prove the slightly stronger assertion that every nonzero quotient of a [Laurent polynomial ring](../../../../../../laurent-polynomial-ring.md) in $r$ variables is finite as a [module](../../../../../../module-mathematics.md) over an embedded [Laurent polynomial ring](../../../../../../laurent-polynomial-ring.md) in some number $m\leq r$ of variables.

Induct on $r$. If the defining [ideal](../../../../../../ideal.md) is zero, the ring itself works. Otherwise choose a nonzero Laurent polynomial

$$
f=\sum_{\mathbf a\in F}c_{\mathbf a}X^{\mathbf a}
$$

in that [ideal](../../../../../../ideal.md), with nonzero coefficients. For a sufficiently large positive integer $N$, the weights

$$
N a_1+N^2a_2+\cdots+N^{r-1}a_{r-1}+a_r
$$

are distinct for all $\mathbf a\in F$. Indeed, each difference gives a nonzero polynomial in $N$, which has only finitely many integer roots. Make the invertible [monomial](../../../../../../monomial.md) substitution

$$
X_j=Y_jY_r^{N^j}\ (j<r),\qquad X_r=Y_r.
$$

Its inverse is $Y_j=X_jX_r^{-N^j}$, so it is an [automorphism](../../../../../../automorphism.md) of the [Laurent polynomial ring](../../../../../../laurent-polynomial-ring.md). When $r=1$ there is no substitution and distinct exponents already give distinct weights.

As a Laurent polynomial in $Y_r$, the transformed relation has unique lowest and highest exponents. Their coefficients are nonzero [scalar](../../../../../../scalar.md) multiples of [monomials](../../../../../../monomial.md) in $Y_1,\ldots,Y_{r-1}$, hence units in

$$
B_0=k[Y_1^{\pm1},\ldots,Y_{r-1}^{\pm1}].
$$

Multiplying by a power of $Y_r$ and the inverse leading coefficient gives

$$
Y_r^d+b_{d-1}Y_r^{d-1}+\cdots+b_0=0,\qquad b_j\in B_0,\quad b_0\in B_0^\times.
$$

Here $d>0$: a single-term Laurent polynomial would be a unit and the quotient would be zero. Reversing the equation and dividing by $b_0Y_r^d$ gives a monic equation for $Y_r^{-1}$. Thus both $Y_r$ and $Y_r^{-1}$ are integral over the image $B$ of $B_0$ in $T$. In fact $b_0$ being a unit also expresses $Y_r^{-1}$ as a polynomial in $Y_r$, so $T$ is generated as a $B$-[module](../../../../../../module-mathematics.md) by $1,Y_r,\ldots,Y_r^{d-1}$. 

The ring $B$ is itself a nonzero quotient of an $(r-1)$-variable [Laurent polynomial ring](../../../../../../laurent-polynomial-ring.md). By induction, it is finite over an embedded [Laurent polynomial ring](../../../../../../laurent-polynomial-ring.md) in $m\leq r-1$ variables. Finiteness of [modules](../../../../../../module-mathematics.md) is transitive, so the same is true of $T$; a finite ring extension is an [integral extension](../../../../../../integral-extension.md), by the [determinant trick](../../../../../../determinant-trick.md) applied to multiplication by an element.

Applying this to $r=3$ yields **an embedded subring**

$$
\boxed{k[Y_1^{\pm1},\ldots,Y_m^{\pm1}]\subseteq T,\qquad T\text{ integral over it}.}
$$

The base case $m=0$ means the subring $k$; finiteness over it would make $T$ a finite-dimensional [vector space](../../../../../../vector-space-split.md). The hypothesis excludes this, so **$1\leq m\leq3$**, as required. No infinitude assumption on $k$ is used.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
