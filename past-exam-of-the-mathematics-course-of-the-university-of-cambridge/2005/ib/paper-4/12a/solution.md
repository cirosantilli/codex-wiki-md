<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

At $P=\sigma(u,v)$, regularity makes $\sigma_u,\sigma_v$ linearly independent. The [tangent space](../../../../../tangent-space.md) is $T_PU=\operatorname{span}\{\sigma_u,\sigma_v\}$, and an oriented unit [normal vector](../../../../../normal-vector.md) is

$$
\boldsymbol n=\frac{\sigma_u\times\sigma_v}{|\sigma_u\times\sigma_v|}.
$$

Reversing its sign chooses the opposite orientation. The [first fundamental form](../../../../../first-fundamental-form.md) is the squared length of a tangent displacement:

$$
|\sigma_u\,du+\sigma_v\,dv|^2=E\,du^2+2F\,du\,dv+G\,dv^2,
$$

where $E=\sigma_u\cdot\sigma_u$, $F=\sigma_u\cdot\sigma_v$, $G=\sigma_v\cdot\sigma_v$. Its determinant $EG-F^2=|\sigma_u\times\sigma_v|^2$ is positive.

Use $N_{\rm II}=\sigma_{vv}\cdot\boldsymbol n$ to distinguish the scalar coefficient of the [second fundamental form](../../../../../second-fundamental-form-split.md) from the [normal vector](../../../../../normal-vector.md). Since $\boldsymbol n\cdot\boldsymbol n=1$, its derivatives are perpendicular to it and hence tangent. Write $\boldsymbol n_u=a\sigma_u+b\sigma_v$ and $\boldsymbol n_v=c\sigma_u+d\sigma_v$. Differentiating $\boldsymbol n\cdot\sigma_u=\boldsymbol n\cdot\sigma_v=0$ gives

$$
\boldsymbol n_u\cdot\sigma_u=-L,\quad \boldsymbol n_u\cdot\sigma_v=-M,\quad
\boldsymbol n_v\cdot\sigma_u=-M,\quad \boldsymbol n_v\cdot\sigma_v=-N_{\rm II}.
$$

Substitution of the tangent expansions proves

$$
\boxed{-\begin{pmatrix}L&M\\M&N_{\rm II}\end{pmatrix}=\begin{pmatrix}a&b\\c&d\end{pmatrix}\begin{pmatrix}E&F\\F&G\end{pmatrix}.}
$$

The [shape operator](../../../../../shape-operator.md) is $-d\boldsymbol n$; its [matrix](../../../../../matrix.md) in the parametrized tangent basis is the negative transpose of the coefficient [matrix](../../../../../matrix.md) shown. Its determinant, the product of the principal curvatures, is therefore

$$
\boxed{ad-bc=\frac{LN_{\rm II}-M^2}{EG-F^2}=K,}
$$

the [Gaussian curvature](../../../../../gaussian-curvature.md). Transposition and the two minus signs do not change this determinant.

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
