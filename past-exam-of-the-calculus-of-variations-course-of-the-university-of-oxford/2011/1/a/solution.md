<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the supporting inequality, assume first that $F$ is convex and fix $z,z_0$. For $0<t\leq1$,

$$
F(z_0+t(z-z_0))\leq(1-t)F(z_0)+tF(z).
$$

Subtract $F(z_0)$, divide by $t$ and let $t\downarrow0$. [Differentiability](../../../../differentiability.md) gives

$$
\boxed{F(z)\geq F(z_0)+DF(z_0)\cdot(z-z_0).}
$$

Conversely assume this inequality for every pair. Put $w=(1-t)z_0+tz$ and apply it with base point $w$ to both $z_0$ and $z$. Multiply those two inequalities by $1-t$ and $t$ and add. The [gradient](../../../../gradient.md) terms cancel, proving $F(w)\leq(1-t)F(z_0)+tF(z)$. Thus the supporting inequality characterizes a differentiable [convex function](../../../../convex-function.md).

For the [integral](../../../../integral-split.md) inequality let $\bar z=|\Omega|^{-1}\int_\Omega u$. Apply the supporting inequality at $\bar z$ to $u(x)$ and integrate. Its affine term has [integral](../../../../integral-split.md) $DF(\bar z)\cdot(\int_\Omega u-|\Omega|\bar z)=0$, yielding

$$
\boxed{F\left(\frac1{|\Omega|}\int_\Omega u\right)
\leq\frac1{|\Omega|}\int_\Omega F(u).}
$$

This is [Jensen's inequality](../../../../jensen-s-inequality.md). Since $u$ is integrable, the supporting affine lower bound has integrable negative part, so the right side is well-defined as an extended real [integral](../../../../integral-split.md). If its positive part is infinite, the inequality remains valid.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the calculus of variations course of the University of Oxford](../../../split.md)
5. [Calculus of variations course of the University of Oxford](../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
