<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

There is a sign issue in the printed problem. Part (c) constructs the inverse of $\Delta-1$, whereas the second equation printed in part (e) contains $\Delta+1$. The latter operator is invertible with homogeneous Dirichlet data only when $1$ is not a [Dirichlet Laplacian eigenvalue](../../../../../../dirichlet-laplacian-eigenvalue.md). Thus the assertion as printed needs this nonresonance hypothesis; with a minus sign it follows directly from parts (c) and (d).

Under either the intended minus sign or the stated nonresonance condition, let $G_0$ and $G_1$ be the bounded Dirichlet solution operators for the two linear equations. Choose $s>n/2$ and work with $u,v\in H^{s+2}(\Omega)\cap H_0^1(\Omega)$. Since $H^s(\Omega)$ is a [Sobolev algebra](../../../../../../sobolev-algebra.md),

$$
\|(\partial_{11}v)^2\|_{H^s}\leq C\|v\|_{H^{s+2}}^2,\qquad
\|(\partial_{22}u)^2\|_{H^s}\leq C\|u\|_{H^{s+2}}^2.
$$

Define

$$
\mathcal T(u,v)=
\left(
G_0\big((\partial_{11}v)^2+\varepsilon f\big),
G_1\big((\partial_{22}u)^2\big)
\right).
$$

Elliptic regularity gives, on a ball of radius $R$,

$$
\|\mathcal T(u,v)\|_{H^{s+2}\times H^{s+2}}
\leq C(R^2+\varepsilon\|f\|_{H^s}),
$$

and the difference estimate has Lipschitz constant at most $CR$. Choose $R$ small and then $\varepsilon_0$ so that $C(R^2+\varepsilon_0\|f\|_{H^s})\leq R$. The [contraction mapping theorem](../../../../../../contraction-mapping-theorem.md) gives a solution for $0\leq\varepsilon<\varepsilon_0$. Repeated elliptic regularity and smoothness of $f$ bootstrap the solution to $C^\infty$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
