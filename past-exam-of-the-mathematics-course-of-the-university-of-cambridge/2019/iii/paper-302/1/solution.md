<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [Lie group](../../../../../lie-group.md) is a [group](../../../../../group-split.md) that is also a [smooth manifold](../../../../../smooth-manifold.md), with [differentiable](../../../../../differentiable-function.md) multiplication and inversion. A [Lie algebra](../../../../../lie-algebra-split.md) is a [vector space](../../../../../vector-space-split.md) with a bilinear alternating [Lie bracket](../../../../../lie-bracket.md) satisfying the [Jacobi identity](../../../../../jacobi-identity.md).

For a [Matrix Lie group](../../../../../matrix-lie-group.md) $G$, put $\mathfrak g=T_I G$. If $X,Y\in\mathfrak g$, the matrix [commutator](../../../../../commutator.md) $[X,Y]=XY-YX$ again lies in $\mathfrak g$: the group commutator $e^{tX}e^{sY}e^{-tX}e^{-sY}$ lies in $G$, and the coefficient of $ts$ in its [matrix logarithm](../../../../../matrix-logarithm.md) is $[X,Y]$. Bilinearity and antisymmetry are immediate, while associativity of matrix multiplication gives the Jacobi identity. Thus $T_I G$, with the commutator bracket, is the [Lie algebra of a matrix Lie group](../../../../../lie-algebra-of-a-matrix-lie-group.md) $\mathcal L(G)$.

The [special linear group](../../../../../special-linear-group.md) $SL(2,\mathbb R)$ is the inverse image of the regular value $1$ under the smooth [determinant](../../../../../determinant.md) map, and multiplication and inversion are smooth. Differentiating $\det(I+tA)=1+t\operatorname{tr}A+O(t^2)$ shows that

$$
\mathcal L(SL(2,\mathbb R))=\mathfrak{sl}_2(\mathbb R)
=\left\{\begin{pmatrix}a&b\\c&-a\end{pmatrix}:a,b,c\in\mathbb R\right\}.
$$

The [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem.md) applied to a trace-zero two-by-two matrix gives

$$
\boxed{A^2=-\det(A)I_2.}
$$

The [exponential map of a matrix Lie group](../../../../../exponential-map-of-a-matrix-lie-group.md) is the [matrix exponential](../../../../../matrix-exponential.md)

$$
\operatorname{Exp}(A)=e^A=\sum_{n=0}^{\infty}\frac{A^n}{n!}.
$$

Since $\det(e^A)=e^{\operatorname{tr}A}=1$, its image lies in $SL(2,\mathbb R)$. Put $d=\det A$. The identity $A^2=-dI$ sums the series explicitly. If $d>0$, with $r=\sqrt d$,

$$
e^A=\cos r\,I+\frac{\sin r}{r}A,
\qquad \operatorname{tr}(e^A)=2\cos r\geq-2.
$$

If $d=0$, the trace is $2$, while if $d<0$, with $r=\sqrt{-d}$,

$$
e^A=\cosh r\,I+\frac{\sinh r}{r}A,
\qquad \operatorname{tr}(e^A)=2\cosh r\geq2.
$$

Hence

$$
\boxed{\operatorname{tr}(\operatorname{Exp}A)\geq-2.}
$$

But $\operatorname{diag}(-2,-1/2)\in SL(2,\mathbb R)$ has trace $-5/2$. It is therefore outside the image, so **the exponential map is not surjective**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
