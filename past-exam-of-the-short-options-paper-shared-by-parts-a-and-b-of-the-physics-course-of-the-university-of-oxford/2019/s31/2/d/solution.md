<h1 id="s31/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A backward [Euler method](../../../../../euler-method.md) with spatial [second-order central differences](../../../../../second-order-central-difference.md) gives

$$
\boxed{\frac{\Phi_j^{n+1}-\Phi_j^n}{\Delta\tau}=\frac{\Phi_{j+1}^{n+1}-2\Phi_j^{n+1}+\Phi_{j-1}^{n+1}}{h^2}-4\pi G\rho_j.}
$$

The source is fixed in pseudo-time; if it were evolving, its evaluation would also need specifying. Each pseudo-time step therefore requires a [linear system](../../../../../system-of-linear-equations.md) solve rather than a purely local explicit update.

## ↑ Ancestors (12)

1. [D](../d.md)
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
