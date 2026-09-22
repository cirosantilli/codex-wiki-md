<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a nonnegative integer $r$, a [Cr field](../../../../../../ci-field.md) is a field over which every [homogeneous polynomial](../../../../../../homogeneous-polynomial.md) of positive degree $d$ in $N>d^r$ variables has a nontrivial zero. Thus a [C1 field](../../../../../../c1-field.md) uses the bound $N>d$, and a [C2 field](../../../../../../c2-field.md) uses $N>d^2$.

The required field theorems are as follows. The [Chevalley-Warning theorem](../../../../../../chevalley-warning-theorem.md) implies that every [finite field](../../../../../../finite-field.md) is $C_1$: the number of zeros of a polynomial with degree smaller than its number of variables is divisible by the characteristic, and for a [homogeneous polynomial](../../../../../../homogeneous-polynomial.md) the origin is already a zero. The [Lang-Nagata theorem for Ci fields](../../../../../../lang-nagata-theorem-for-ci-fields.md) states that a finitely generated extension of transcendence degree $s$ of a $C_r$ field is $C_{r+s}$. The [Tsen theorem](../../../../../../tsen-theorem.md) states that the function field of a curve over an [algebraically closed field](../../../../../../algebraically-closed-field.md) is $C_1$. In particular, [finite fields](../../../../../../finite-field.md), algebraically closed fields and fields such as $\mathbb C(t)$ are examples of $C_1$ fields. A function field of one variable over a [finite field](../../../../../../finite-field.md) is $C_2$ by the Lang theorem. These are statements of the theorems; no theorem proof is needed here.

For the requested [finite extension stability of C1 fields](../../../../../../finite-extension-stability-of-c1-fields.md), let $m=[L:K]$ and choose a $K$-basis $u_1,\ldots,u_m$ of $L$. Given a homogeneous $f\in L[X_1,\ldots,X_N]$ of degree $d$ with $N>d$, substitute $X_i=\sum_jx_{ij}u_j$ and take the [field norm](../../../../../../field-norm.md):

$$
F((x_{ij}))=N_{L/K}\left(f\left(\sum_jx_{1j}u_j,\ldots,\sum_jx_{Nj}u_j\right)\right).
$$

The [field norm](../../../../../../field-norm.md) is the [determinant](../../../../../../determinant.md) of multiplication on the $m$-dimensional $K$-space $L$, hence a [homogeneous polynomial](../../../../../../homogeneous-polynomial.md) of degree $m$ in its coordinates. Consequently $F$ is homogeneous of degree $md$ in $mN>md$ variables over $K$. The $C_1$ property gives a nonzero coordinate vector $(x_{ij})$ with $F=0$. Its corresponding vector $(X_i)\in L^N$ is nonzero, since the $u_j$ are a basis. The norm of a field element vanishes only for the zero element, so $f(X_1,\ldots,X_N)=0$. **Every finite extension of a $C_1$ field is $C_1$.** This proof includes inseparable finite extensions, because the [determinant](../../../../../../determinant.md) definition of the [field norm](../../../../../../field-norm.md) requires no separability.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
