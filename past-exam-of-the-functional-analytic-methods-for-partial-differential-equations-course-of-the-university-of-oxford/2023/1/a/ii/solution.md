<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here [Morrey's inequality](../../../../../morrey-s-inequality.md) has [Hölder exponent](../../../../../holder-exponent.md) $1-3/6=1/2$. Every $u\in W^{1,6}(\mathbb R^3)$ has a unique continuous representative $u^*$ such that

$$
\boxed{\|u^*\|_{C^{0,1/2}(\mathbb R^3)}\leq C\|u\|_{W^{1,6}(\mathbb R^3)},\qquad
[u^*]_{C^{0,1/2}(\mathbb R^3)}\leq C\|\nabla u\|_6.}
$$

We use the [Hölder norm](../../../../../holder-norm.md) $\|f\|_{C^{0,1/2}}=\|f\|_\infty+[f]_{C^{0,1/2}}$, where the [Hölder seminorm](../../../../../holder-seminorm.md) is $\sup_{x\ne y}|f(x)-f(y)|/|x-y|^{1/2}$. The second bound is the homogeneous form of [Morrey's inequality](../../../../../morrey-s-inequality.md); the first includes control of the values themselves.

Let $u_j=\rho_{1/j}*u$ be the [mollifications](../../../../../mollification.md) from (i). They converge to $u$ in the [Sobolev norm](../../../../../sobolev-norm.md). Apply the assumed smooth version of [Morrey's inequality](../../../../../morrey-s-inequality.md) to the differences $u_j-u_\ell$:

$$
\|u_j-u_\ell\|_{C^{0,1/2}}\leq C\|u_j-u_\ell\|_{W^{1,6}}\longrightarrow0.
$$

Thus $(u_j)$ is a [Cauchy sequence](../../../../../cauchy-sequence.md) in the complete [Hölder space](../../../../../holder-space.md) $C^{0,1/2}(\mathbb R^3)$ and converges there to a function $w$. In particular the convergence is uniform. On every [bounded set](../../../../../bounded-set.md) $K$ of finite volume,

$$
\|w-u\|_{L^6(K)}
\leq |K|^{1/6}\|w-u_j\|_\infty+\|u_j-u\|_{L^6(\mathbb R^3)}\longrightarrow0.
$$

Exhausting $\mathbb R^3$ by [balls](../../../../../ball-mathematics.md) proves $w=u$ [almost everywhere](../../../../../almost-everywhere.md). Set $u^*=w$. Taking limits in the smooth [Hölder norm](../../../../../holder-norm.md) bound gives the first boxed estimate. For any fixed $x\ne y$, taking limits in

$$
|u_j(x)-u_j(y)|\leq C|x-y|^{1/2}\|\nabla u_j\|_6
$$

gives the second boxed estimate after taking the supremum. Finally, two continuous representatives equal [almost everywhere](../../../../../almost-everywhere.md) must coincide everywhere, since a nonzero continuous difference would remain nonzero on an [open ball](../../../../../open-ball.md) of positive volume.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../../split.md)
6. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
