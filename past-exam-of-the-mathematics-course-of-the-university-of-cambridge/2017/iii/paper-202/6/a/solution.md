<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $V(x)=(1+x^2)^{-1}$ and $A_t=\int_0^tV(B_s)ds$. On a fixed horizon $T$, the [Itô formula](../../../../../../ito-s-lemma.md) and [Itô product rule](../../../../../../ito-product-rule.md) give

$$
d\bigl(e^{A_t}u(T-t,B_t)\bigr)=e^{A_t}\bigl(-u_t+\tfrac12u_{xx}+Vu\bigr)(T-t,B_t)dt+e^{A_t}u_x(T-t,B_t)dB_t.
$$

The drift vanishes by the [partial differential equation](../../../../../../partial-differential-equation-split.md). This makes $M$ a [continuous local martingale](../../../../../../continuous-local-martingale.md). Since $0\leq A_t\leq T$,

$$
\boxed{|M_t|\leq e^T\sup_{0\leq s\leq T,\,y\in\mathbb R}|u(s,y)|\quad(0\leq t\leq T).}
$$

The right side is a finite deterministic bound under the stated boundedness assumption, so the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) removes a [localizing sequence](../../../../../../localizing-sequence.md) and $M$ is a true [martingale](../../../../../../martingale-split.md). If the derivatives are also bounded, the [Itô isometry](../../../../../../ito-isometry.md) alternatively proves the stochastic integral is [square-integrable](../../../../../../square-integrable-function.md) because $\mathbb E\int_0^Te^{2A_s}|u_x(T-s,B_s)|^2ds\leq Te^{2T}\|u_x\|_\infty^2$.

For the [bounded parabolic differentiability class](../../../../../../bounded-parabolic-differentiability-class.md), distinguish global bounds from bounds on each finite time slab. Only the latter are needed here; a single global bound on the [classical solution](../../../../../../classical-solution.md) $u$ would conflict with its requested long-time growth in part (c).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
