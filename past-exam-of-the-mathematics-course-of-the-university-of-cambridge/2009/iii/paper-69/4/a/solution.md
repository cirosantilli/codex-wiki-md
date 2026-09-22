<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $u\in\mathcal U$, $r=f-u$, $M=\|r\|_\infty$, and $E=\{x\in[0,1]:|r(x)|=M\}$. The [Kolmogorov criterion for uniform approximation](../../../../../../kolmogorov-criterion-for-uniform-approximation.md) says

$$
\boxed{u\text{ is a best approximant}
\iff\forall v\in\mathcal U,\quad
\min_{x\in E}r(x)v(x)\le0.}
$$

Equivalently, no available perturbation $v$ has strictly the same sign as the nonzero residual at every extremal point. This statement concerns a candidate $u$ in the [linear subspace](../../../../../../vector-subspace.md); it does not assume every subspace has an attained best approximation. If $M=0$, $u=f$ is already exact and the criterion is automatic.

To see sufficiency, for any competitor $u+v$, the criterion supplies an $x\in E$ with $r(x)v(x)\le0$. Then $|f(x)-u(x)-v(x)|\ge|r(x)|=M$, so the competitor cannot have smaller [supremum norm](../../../../../../supremum-norm.md) error.

For necessity, suppose $M>0$ and some $v\in\mathcal U$ has $r(x)v(x)>0$ on $E$. Since $E$ is compact, this product has a positive minimum there. By [continuity](../../../../../../continuous-function.md), a neighborhood $O$ of $E$ has $rv\ge\eta>0$. For sufficiently small $\varepsilon>0$,

$$
|r-\varepsilon v|^2=r^2-2\varepsilon rv+\varepsilon^2v^2<M^2\quad\text{on }O.
$$

On the compact complement of $O$, $|r|$ has a strict gap below $M$, and taking $\varepsilon\|v\|_\infty$ smaller than this gap preserves it. Hence $u+\varepsilon v$ improves the uniform error everywhere, contradicting [best uniform approximation](../../../../../../best-uniform-approximation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
