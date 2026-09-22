<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [infinitesimal generator of a semigroup](../../../../../../infinitesimal-generator-of-a-semigroup.md) is the [linear operator](../../../../../../linear-operator.md)

$$
Au=\lim_{h\downarrow0}\frac{U(h)u-u}{h}
$$

with [generator domain](../../../../../../generator-domain.md)

$$
D(A)=\left\{u\in H:\lim_{h\downarrow0}\frac{U(h)u-u}{h}\text{ exists in }H\right\}.
$$

For example, the [Bochner integral](../../../../../../bochner-integral.md)

$$
u_t=\int_0^tU(s)u\,ds
$$

belongs to $D(A)$ for every $u\in H$ and $t>0$, since $Au_t=U(t)u-u$.

To prove that $A$ is a [closed linear operator](../../../../../../closed-linear-operator.md), suppose $u_n\in D(A)$, $u_n\to u$, and $Au_n\to v$. For vectors in the [generator domain](../../../../../../generator-domain.md),

$$
U(t)u_n-u_n=\int_0^tU(s)Au_n\,ds.
$$

Passing to the [limit](../../../../../../limit-of-a-function.md) in the [Banach space](../../../../../../banach-space-split.md) gives

$$
U(t)u-u=\int_0^tU(s)v\,ds.
$$

After division by $t$, [strong continuity](../../../../../../strong-continuity.md) makes the right side converge to $v$ as $t\downarrow0$. Hence $u\in D(A)$ and $Au=v$, so $A$ is closed.

For $\operatorname{Re}z>\omega$, define the [Bochner integral](../../../../../../bochner-integral.md)

$$
R(z)u=\int_0^\infty e^{-zt}U(t)u\,dt.
$$

It converges absolutely because

$$
\|e^{-zt}U(t)u\|\leq Me^{-(\operatorname{Re}z-\omega)t}\|u\|.
$$

Integrating the semigroup difference quotient shows that $R(z)u\in D(A)$ and $(zI-A)R(z)u=u$. The same computation for $u\in D(A)$ gives $R(z)(zI-A)u=u$. Thus the [Laplace-transform formula for a semigroup resolvent](../../../../../../laplace-transform-formula-for-a-semigroup-resolvent.md) proves

$$
\boxed{\{z\in\mathbb C:\operatorname{Re}z>\omega\}\subseteq\rho(A)},
\qquad
\|R(z)\|\leq\frac{M}{\operatorname{Re}z-\omega}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 319](../../../paper-319-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
