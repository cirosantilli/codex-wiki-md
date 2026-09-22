<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Morse lemma](../../../../../morse-lemma.md) states that if $p$ is a [nondegenerate critical point](../../../../../nondegenerate-critical-point.md) of a smooth real function $f$ on an $m$-dimensional [smooth manifold](../../../../../smooth-manifold.md), there are smooth coordinates $y_1,\ldots,y_m$, centered at $p$, such that

$$
\boxed{f(y)=f(p)-\sum_{i=1}^{\lambda}y_i^2+\sum_{i=\lambda+1}^m y_i^2.}
$$

Here $\lambda$ is the [Morse index](../../../../../morse-index.md), the number of negative directions of the [Hessian matrix](../../../../../hessian-matrix.md) at $p$. The equality is exact on a neighborhood, not merely a second-order expansion.

To prove it, start with any coordinates putting $p=0$. Since $df(0)=0$, integral [Taylor theorem](../../../../../taylor-theorem.md) gives

$$
f(x)-f(0)=\sum_{i,j=1}^m a_{ij}(x)x_ix_j,\qquad a_{ij}(x)=\int_0^1(1-t)\,\partial_i\partial_jf(tx)\,dt.
$$

The [matrix](../../../../../matrix.md) $A(x)=(a_{ij}(x))$ is smooth and symmetric, with $A(0)=\tfrac12\operatorname{Hess}f(0)$. By [Sylvester's law of inertia](../../../../../sylvester-s-law-of-inertia.md), a constant invertible linear coordinate change makes $A(0)=\operatorname{diag}(-I_\lambda,I_{m-\lambda})$.

We perform completion of squares with coefficients depending smoothly on the original $x$. The first pivot $a_{11}(x)$ stays nonzero and keeps its sign on a sufficiently small neighborhood. Algebraically,

$$
x^TA(x)x=a_{11}(x)\left(x_1+\sum_{j>1}\frac{a_{1j}(x)}{a_{11}(x)}x_j\right)^2+\sum_{i,j>1}\left(a_{ij}(x)-\frac{a_{i1}(x)a_{1j}(x)}{a_{11}(x)}\right)x_ix_j.
$$

The remaining coefficient matrix is the [Schur complement](../../../../../schur-complement.md). At zero it is the remaining signed diagonal matrix, so its first pivot is also nonzero nearby. Continue recursively, shrinking the neighborhood finitely many times. Every pivot $d_i(x)$ is smooth and nonzero, with sign $\epsilon_i=-1$ for $i\leq\lambda$ and $+1$ thereafter. Absorb $|d_i(x)|$ into the square by its smooth positive square root. This produces a smooth triangular matrix $B(x)$ with nonzero diagonal such that

$$
x^TA(x)x=\sum_i\epsilon_i\bigl(B(x)x\bigr)_i^2.
$$

All coefficients here are functions of the original $x$; no circular coordinate substitution is involved. Define $\Phi(x)=B(x)x$. Its derivative at zero is $D\Phi(0)=B(0)$, which is invertible. The [inverse function theorem](../../../../../inverse-function-theorem.md) makes $y=\Phi(x)$ a smooth coordinate system and gives the asserted exact quadratic form. The number of negative squares agrees with the [Hessian matrix](../../../../../hessian-matrix.md) signature and hence with the [Morse index](../../../../../morse-index.md). This is the [smooth completing-square proof of the Morse lemma](../../../../../smooth-completing-square-proof-of-the-morse-lemma.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
