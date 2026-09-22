<h1 id="b/6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume that a nonconstant polynomial $f$ has no zero. Then $g=1/f$ is entire. The leading polynomial term makes $|f(z)|\to\infty$ as $|z|\to\infty$, so $g(z)\to0$ there. On any remaining compact disk, continuity and absence of zeros bound $1/|f|$. Consequently $g$ is bounded on the entire plane.

Part (c)(i) makes $u(Z_t)=\operatorname{Re}g(Z_t)$ a bounded [local martingale](../../../../../../local-martingale.md), hence a true bounded martingale. The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) says it converges almost surely as $t\to\infty$.

The harmonic function $u$ cannot be constant. Otherwise the [Cauchy-Riemann equations](../../../../../../cauchy-riemann-equations.md) would make both derivatives of $\operatorname{Im}g$ zero, so $g$ and then $f$ would be constant. Choose points $z_1,z_2$ with $u(z_1)<u(z_2)$. Continuity supplies two disjoint disks on which the ranges of $u$ are separated by a positive gap. By part (b), the Brownian path visits these disks alternately at times tending to infinity. The corresponding subsequences of $u(Z_t)$ then remain separated, contradicting its almost sure convergence.

The zero-free assumption is impossible. Hence  
**Every nonconstant complex polynomial has a complex root.**  
This proves the [fundamental theorem of algebra](../../../../../../fundamental-theorem-of-algebra.md) using recurrence and martingale convergence, without invoking Liouville's theorem as a prior algebraic shortcut.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [B](../../../../b.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../split.md)
7. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
