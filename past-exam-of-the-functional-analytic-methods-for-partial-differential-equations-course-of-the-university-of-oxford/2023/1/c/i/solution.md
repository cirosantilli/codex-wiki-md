<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $r=|x|$, $u(x)=\bar u(r)$, and let $g(r)$ be the [radial profile](../../../../../radial-profile.md) of the [radial derivative](../../../../../radial-derivative.md) $\nabla u(x)\cdot x/|x|$, which may be assumed to be a [radial function](../../../../../radial-function.md) here. The [spherical coordinate system](../../../../../spherical-coordinate-system.md) gives

$$
\int_A|u|^6\,dx=4\pi\int_1^2|\bar u(r)|^6r^2\,dr,\qquad
4\pi\int_1^2|g(r)|^6r^2\,dr
\leq\int_A|\nabla u|^6\,dx.
$$

Since $1\leq r^2\leq4$, both $\bar u$ and $g$ belong to the [Lp space](../../../../../lp-space.md) $L^6(1,2)$. It remains to identify the [weak derivative](../../../../../weak-derivative.md) of the [radial profile](../../../../../radial-profile.md) directly.

For $\phi\in C_c^\infty(1,2)$, each component of $\phi(r)x/r$ is a [test function](../../../../../test-function.md) on $A$. Sum the three defining [weak derivative](../../../../../weak-derivative.md) identities, using the stated [divergence](../../../../../divergence.md) formula:

$$
\begin{aligned}
4\pi\int_1^2g(r)\phi(r)r^2\,dr
&=\int_A\nabla u\cdot\frac{x}{r}\phi(r)\,dx\\
&=-\int_Au\left(\phi'(r)+\frac2r\phi(r)\right)dx\\
&=-4\pi\int_1^2\bar u(r)\bigl(r^2\phi(r)\bigr)'\,dr.
\end{aligned}
$$

Given an arbitrary [test function](../../../../../test-function.md) $\zeta\in C_c^\infty(1,2)$, choose $\phi(r)=\zeta(r)/r^2$. Dividing by $4\pi$ gives $\int g\zeta=-\int\bar u\zeta'$, exactly the definition of the [weak derivative](../../../../../weak-derivative.md). We have proved

$$
\boxed{\bar u\in W^{1,6}(1,2),\qquad\bar u'=g\ \text{almost everywhere},\qquad
\|\bar u\|_{W^{1,6}(1,2)}\leq C\|u\|_{W^{1,6}(A)}.}
$$

This [radial Sobolev profile on an annulus](../../../../../radial-sobolev-profile-on-an-annulus.md) estimate follows from the two weighted [integrals](../../../../../integral-split.md) above and equivalence of the usual [Sobolev norms](../../../../../sobolev-norm.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
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
