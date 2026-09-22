<h1 id="s31/2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For an error [Fourier mode](../../../../../fourier-mode.md) $e_j^n=\widehat e^n e^{i\theta j}$, the periodic [discrete Laplacian](../../../../../discrete-laplacian.md) has eigenvalue $-4\sin^2(\theta/2)/h^2$. The [Backward Euler method](../../../../../backward-euler-method.md) therefore has amplification factor

$$
\boxed{g(\theta)=\frac1{1+4r\sin^2(\theta/2)},\qquad0<g\le1\quad(r\ge0).}
$$

[von Neumann stability analysis](../../../../../von-neumann-stability-analysis.md) thus imposes no upper limit on positive $\Delta\tau$. The constant mode has $g=1$ and is not damped; compatible forcing and a gauge condition remain necessary as discussed in part (e). Large steps can accelerate relaxation of nonconstant modes, but require a suitably accurate [linear solver](../../../../../linear-solver.md) and can worsen its conditioning. Unconditional linear stability is not a statement about time accuracy or cost.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
3. [S31](../../../s31.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
