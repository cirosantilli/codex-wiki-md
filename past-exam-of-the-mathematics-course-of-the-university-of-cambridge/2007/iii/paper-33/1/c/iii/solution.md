<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The event $A_{n,\varepsilon}=\{Y_n\leq\varepsilon\}$ belongs to $\mathcal F_n$. Its $\nu$-measure can therefore be computed using the finite-level density:

$$
\nu(A_{n,\varepsilon})=\int_{A_{n,\varepsilon}}Y_n\,d\lambda\leq\varepsilon\lambda(A_{n,\varepsilon})\leq\varepsilon.
$$

Let $H=\{\limsup_nY_n=0\}$. Because the chosen versions satisfy $Y_n\geq0$ everywhere, every point of $H$ eventually lies in all the $A_{n,\varepsilon}$. For each $N$, the set $\bigcap_{n\geq N}A_{n,\varepsilon}$ has $\nu$-measure at most $\varepsilon$; these sets increase as $N$ increases. Continuity from below gives

$$
\nu(H)\leq\nu\left(\bigcup_N\bigcap_{n\geq N}A_{n,\varepsilon}\right)\leq\varepsilon.
$$

Letting $\varepsilon\downarrow0$ yields **$\nu(H)=0$**. In contrast, the preceding part says $\lambda(H)=1$. Thus $\nu$ is concentrated on the $\lambda$-null set $H^c$. This proves that $\nu$ and $\lambda$ are [mutually singular measures](../../../../../../../mutually-singular-measures.md), and completes the [martingale construction of Lebesgue decomposition](../../../../../../../martingale-construction-of-lebesgue-decomposition.md):

$$
\boxed{\mu=X_\infty\lambda+\nu,\qquad\nu\perp\lambda.}
$$

The key step is that the density identity is available on each $\mathcal F_n$ even though $\nu$ need not have a density on the full Borel [sigma-algebra](../../../../../../../sigma-algebra.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
