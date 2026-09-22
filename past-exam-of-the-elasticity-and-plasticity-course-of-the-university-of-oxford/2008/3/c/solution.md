<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Linearization](../../../../linearization.md) gives $\theta''+\pi^2\lambda\theta=0$. The two homogeneous Dirichlet conditions select $\boxed{\lambda=n^2,\quad\theta=A\sin(n\pi\xi),\quad n=1,2,\ldots}$. For any small trial [amplitude](../../../../wave-amplitude.md) in this mode, $\int_0^1\sin^2(n\pi\xi)=\int_0^1\cos^2(n\pi\xi)=1/2$, so

$$
\boxed{U[A\sin(n\pi\xi)]=\frac{\pi^2EIA^2}{4L}(n^2-\lambda)+O(A^4).}
$$

For $\lambda<1$ every nonzero quadratic [variation](../../../../variation.md) is positive by the sharp [Poincaré inequality](../../../../poincare-inequality.md). For $\lambda>1$, the first mode gives negative energy at sufficiently small [amplitude](../../../../wave-amplitude.md), so zero cannot be a [local minimum](../../../../local-minimum.md).

**The printed strict “only if” conclusion omits the critical case.** At $\lambda=1$ the quadratic test is degenerate, not negative. In fact zero is still the unique minimum of the full displayed [functional](../../../../functional.md): use $1-\cos\theta\leq\theta^2/2$ and $\int\theta'^2\geq\pi^2\int\theta^2$ to get $U\geq0$, with strict inequality for a nonzero continuous function because $1-\cos t<t^2/2$ when $t\ne0$. In particular on the critical first mode,

$$
\boxed{U[A\sin\pi\xi]=\frac{\pi^2EI}{64L}A^4+O(A^6)>0\quad\text{for small }A\ne0.}
$$

Thus strict positivity of the [second variation](../../../../second-variation.md) holds for $\lambda<1$, while local minimality of the full energy holds also at $\lambda=1$. This is the distinction captured by [critical-load minimality of the angular Euler strut](../../../../critical-load-minimality-of-the-angular-euler-strut.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
