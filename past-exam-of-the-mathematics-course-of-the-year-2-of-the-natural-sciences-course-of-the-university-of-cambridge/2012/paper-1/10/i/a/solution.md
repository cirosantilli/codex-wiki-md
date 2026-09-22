<h1 id="10/i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One suitable choice is homogeneous [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md), $\psi(\alpha)=\psi(\beta)=0$, with variations vanishing there. Assume real $q$ and the stated positive $p,w$. Introduce a [Lagrange multiplier](../../../../../../lagrange-multiplier.md) $\mu$ for $N[\psi]=1$. For real variations, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\delta(Q-\mu N)=2[p\psi'\eta]_\alpha^\beta+2\int_\alpha^\beta[-(p\psi')'+q\psi-\mu w\psi]\eta\,dx.
$$

The boundary term vanishes, so the [fundamental lemma of the calculus of variations](../../../../../../fundamental-lemma-of-the-calculus-of-variations.md) yields

$$
\boxed{-(p\psi')'+q\psi=\mu w\psi.}
$$

Multiplying this equation by $\psi$, integrating, and using the boundary conditions gives $Q[\psi]=\mu N[\psi]=\mu$. Thus the multiplier, the eigenvalue, and the constrained stationary value coincide. Conversely every normalized eigenfunction makes the first variation vanish for all tangent variations satisfying $\delta N=0$.

Homogeneous [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md), $p\psi'=0$ at both endpoints, or mixed Dirichlet and Neumann conditions also work with this energy form. General [Robin boundary conditions](../../../../../../robin-boundary-condition.md) require the corresponding boundary terms in the form; they cannot simply be inserted into the displayed unmodified integral.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [I](../../i.md)
3. [10](../../../10.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
