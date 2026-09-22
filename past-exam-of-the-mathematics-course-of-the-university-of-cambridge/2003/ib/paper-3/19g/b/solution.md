<h1 id="19g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [normal operator](../../../../../../normal-operator.md) $\phi$, the [adjoint operator](../../../../../../adjoint-operator.md) identity and $\phi^*\phi=\phi\phi^*$ give

$$
\|\phi u\|^2=\langle\phi^*\phi u,u\rangle=\langle\phi\phi^*u,u\rangle=\|\phi^*u\|^2.
$$

Positive definiteness implies $\ker\phi=\ker\phi^*$. Also $(\operatorname{im}\phi)^\perp=\ker\phi^*$, since orthogonality to every $\phi v$ means $\langle\phi^*u,v\rangle=0$ for every $v$. In finite dimension this gives $\operatorname{im}\phi=(\ker\phi)^{\perp}$.

The [idempotent linear map](../../../../../../projection-linear-algebra.md) decomposes $U=\ker\phi\oplus\operatorname{im}\phi$ as in part (a), now orthogonally, and acts as zero on its [kernel](../../../../../../kernel-of-a-linear-map.md) and identity on its [image](../../../../../../image-of-a-function.md). Writing $u=k+w$ and $v=k'+w'$ in these orthogonal summands,

$$
\langle\phi u,v\rangle=\langle w,w'\rangle=\langle u,\phi v\rangle.
$$

Thus $\phi$ is [self-adjoint](../../../../../../self-adjoint-operator.md), and together with idempotence this proves **$\phi$ is an orthogonal projection**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19G](../../19g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
