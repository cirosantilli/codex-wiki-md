<h1 id="b/7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At zero the quadratic form is

$$
\delta^2I(0)[\phi,\phi]=2Q_\lambda(\phi),\qquad Q_\lambda(u)=\int_0^1(u'^2+\lambda u^2).
$$

For $\lambda\geq0$ it dominates $\int u'^2$. For $-\pi^2<\lambda<0$ set $\mu=\sqrt{-\lambda}<\pi$ and $z(x)=\cos(\mu(x-1/2))$, positive on the closed interval and satisfying $z''+\mu^2z=0$. The Jacobi identity gives $Q_\lambda(u)=\int z^2[(u/z)']^2$. To obtain a uniform lower bound, let $m=\min z>0$, $K=\max|z'|$ and $v=u/z$. Since $\max z=1$ and $\int v^2\leq\tfrac12\int v'^2$,

$$
\int u'^2\leq2K^2\int v^2+2\int v'^2\leq(K^2+2)\int v'^2,
$$

so $Q_\lambda(u)\geq m^2\int u'^2/(K^2+2)$.

Finally $I(u)=Q_\lambda(u)+O(\int u^4)$ near zero, because $\sin^2u=u^2+O(u^4)$. The remainder is at most a constant times $\|u\|_\infty^2\int u^2\leq\tfrac12\|u\|_\infty^2\int u'^2$. It is dominated by the coercive bound for small perturbations. Thus **the [second variation](../../../../../../second-variation.md) is positive and zero is a strict weak local minimizer for every $\lambda>-\pi^2$**. This argument has not assumed the sharp [Poincaré inequality](../../../../../../poincare-inequality.md) that is to be deduced next.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [B](../../../../b.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../split.md)
7. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
