# Two-by-two positive-definiteness test

↑ **Parent:** [Positive definiteness](positive-definiteness.md)

For a real [symmetric matrix](symmetric-matrix.md) $A=\begin{pmatrix}a&b\\b&c\end{pmatrix}$, [completing the square](completing-the-square.md) gives, when $a\ne0$,

$$
q(x,y)=ax^2+2bxy+cy^2=a\left(x+\frac ba y\right)^2+\frac{ac-b^2}{a}y^2.
$$

Thus $A$ is a [positive-definite matrix](positive-definite-matrix.md) exactly when $a>0$ and $\det A=ac-b^2>0$. For necessity, test $(1,0)$ first, then $(-b/a,1)$; for sufficiency, the displayed two positive squares give the result. These are the first two leading [principal minors](principal-minor.md) in [Sylvester's criterion](sylvester-s-criterion.md). A positive [determinant](determinant.md) alone is insufficient: $-I_2$ has [determinant](determinant.md) $1$ but is a [negative-definite matrix](negative-definite-matrix.md).

The [eigenvalues](eigenvalue.md) provide an equivalent test under the same real-symmetric hypothesis:

$$
\lambda_\pm=\frac{a+c\pm\sqrt{(a-c)^2+4b^2}}2,\qquad A\text{ positive definite}\ \Longleftrightarrow\ \lambda_+>0\text{ and }\lambda_->0.
$$

The [spectral theorem for real symmetric matrices](spectral-theorem-for-real-symmetric-matrices.md) supplies [coordinates](coordinate-linear-algebra.md) in an [orthonormal basis](orthonormal-basis.md) in which $q=\lambda_+u^2+\lambda_-v^2$. More generally, a complex [Hermitian matrix](hermitian-operator.md) has an [orthonormal eigenbasis](orthonormal-eigenbasis.md) and $q(z)=\sum_j\lambda_j|w_j|^2$, so it is a [Hermitian positive-definite matrix](hermitian-positive-definite-matrix.md) exactly when every [eigenvalue](eigenvalue.md) is positive. This is a short proof outline: test the [eigenvectors](eigenvector.md) for necessity, and sum the positive squared [absolute values](absolute-value.md) for sufficiency.[Appendix A.5.2, pp. 646–647: symmetric eigenvalue decomposition and definiteness](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

For a real [positive semidefinite matrix](positive-semidefinite-matrix.md), the condition is instead $q(x,y)\geq0$ for all [vectors](vector.md), equivalent here to $a\geq0$, $c\geq0$, and $ac-b^2\geq0$. If $a>0$, the same [completing the square](completing-the-square.md) proves this; if $a=0$, nonnegativity forces $b=0$ and leaves $cy^2$ with $c\geq0$. Merely replacing the strict inequalities on the leading [principal minors](principal-minor.md) by nonstrict ones fails: $\operatorname{diag}(0,-1)$ has both leading [principal minors](principal-minor.md) zero yet gives $q(0,1)=-1$. An [indefinite quadratic form](indefinite-quadratic-form.md) takes both positive and negative values; its real [symmetric matrix](symmetric-matrix.md) has [eigenvalues](eigenvalue.md) of both signs.

## ↑ Ancestors (9)

1. [Positive definiteness](positive-definiteness.md)
2. [Positive-definite bilinear form](positive-definite-bilinear-form.md)
3. [Symmetric bilinear form](symmetric-bilinear-form.md)
4. [Bilinear form](bilinear-form.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
