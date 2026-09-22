<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Joseph Fourier](../../../joseph-fourier.md)'s [Théorie analytique de la chaleur by Joseph Fourier](../../../theorie-analytique-de-la-chaleur-by-joseph-fourier.md) (1822) makes [trigonometric series](../../../trigonometric-series.md) instruments for solving problems of [heat conduction](../../../thermal-conduction.md). A prescribed [temperature](../../../temperature-split.md) distribution need not be given by one [power series](../../../power-series.md): it may describe different heating on different parts of a body. The extract occurs in Chapter III, §233, where the earlier assumption of an odd-power expansion is relaxed. The innovation concerns both representation and what can count as a [function](../../../function-split.md) in an analytical calculation.[§233, integral formula; §§163–169, the boundary-value problem motivating the expansions](../../../theorie-analytique-de-la-chaleur-by-joseph-fourier/propagation-de-la-chaleur-dans-un-solide-rectangle-infini.md)

Use a separate integration variable $t$ to unpack the printed notation. The proposed [Fourier sine series](../../../fourier-sine-series.md) has [coefficients](../../../coefficient.md)

$$
\boxed{b_n=\frac{2}{\pi}\int_0^\pi f(t)\sin(nt)\,dt,\qquad
f(x)\sim\sum_{n=1}^{\infty}b_n\sin(nx).}
$$

The integral signs in the extract denote [definite integrals](../../../definite-integral.md) over $[0,\pi]$, not [antiderivatives](../../../antiderivative.md); the author explicitly supplies these bounds in the surrounding sentence. Their absent printed bounds are a notational convention, not permission to choose arbitrary constants of integration.

The key calculation is the [orthogonality](../../../orthogonal-vectors.md) relation

$$
\int_0^\pi\sin(nt)\sin(mt)\,dt=
\begin{cases}\pi/2&n=m,\\0&n\ne m.\end{cases}
$$

The [product-to-sum formulas](../../../product-to-sum-formula.md) prove this by integrating cosines of integer multiples of $t$. If an expansion can be integrated term by term, multiplication by $\sin(mt)$ followed by integration selects exactly one [coefficient](../../../coefficient.md). This derives the only possible [coefficients](../../../coefficient.md), but does not by itself prove the expansion converges to the proposed [function](../../../function-split.md). That distinction is central to assessing the extract's claim.

For a revealing example take $f(x)=1$ on $0<x<\pi$. Direct integration gives $b_n=2(1-(-1)^n)/(\pi n)$, and therefore

$$
1=\frac4\pi\left(\sin x+\frac{\sin3x}{3}+\frac{\sin5x}{5}+\cdots\right),\qquad0<x<\pi.
$$

Every term is zero at $0$ and $\pi$, so the [series](../../../series-mathematics.md) cannot take the value $1$ at those endpoints. Its natural interpretation uses the [odd extension](../../../odd-extension.md) followed by [periodic extension](../../../periodic-extension.md); the endpoints become [jump discontinuities](../../../jump-discontinuity.md). More generally, for a piecewise continuously differentiable [function](../../../function-split.md), the [Fourier series](../../../fourier-series-split.md) converges at an interior jump to the average of the two [one-sided limits](../../../one-sided-limit.md), irrespective of an individually assigned value there. Changing one value also leaves the [integrals](../../../integral-split.md) unchanged. Consequently the unqualified assertion of representation for every arbitrary [function](../../../function-split.md) cannot be a modern pointwise theorem. [Dirichlet's theorem on Fourier series](../../../dirichlet-s-theorem-on-fourier-series.md) supplies sufficient conditions and the correct distinction between continuity points and jumps; its 1829 source explicitly addresses the proof problem.[1829, opening discussion and concluding convergence statement](../../../sur-la-convergence-des-series-trigonometriques-qui-servent-a-representer-une-fonction-arbitraire-entre-des-limites-donnees-by-peter-gustav-lejeune-dirichlet.md)

The physical payoff is explicit. For a rod scaled to $0<x<\pi$ with zero end [temperature](../../../temperature-split.md), [separation of variables](../../../separation-of-variables.md) in the [heat equation](../../../heat-equation.md) produces

$$
u(x,\tau)=\sum_{n=1}^{\infty}b_n e^{-\kappa n^2\tau}\sin(nx),\qquad\kappa>0.
$$

Each mode solves $u_\tau=\kappa u_{xx}$ and the end [boundary conditions](../../../boundary-condition.md); the [Fourier sine coefficients](../../../fourier-sine-coefficient.md) encode the initial [temperature](../../../temperature-split.md). This rod is an explanatory example, distinct from the stationary rectangular-solid problem opening [Joseph Fourier](../../../joseph-fourier.md)'s Chapter III. The factor $e^{-\kappa n^2\tau}$ damps high modes rapidly for positive time. **The representation of arbitrary data makes the physical solution possible; the proof of that representation remains a separate task.**

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2023](../../2023-split.md)
3. [Past exam of the history of mathematics course of the University of Oxford](../../split.md)
4. [History of mathematics course of the University of Oxford](../../../history-of-mathematics-course-of-the-university-of-oxford.md)
5. [Year 3 of the mathematics course of the University of Oxford](../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
