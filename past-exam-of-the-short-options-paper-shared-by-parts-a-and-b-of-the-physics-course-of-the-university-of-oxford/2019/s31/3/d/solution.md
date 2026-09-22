<h1 id="s31/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Backward [Euler method](../../../../../euler-method.md) has update $\mathbf y^{n+1}=(I-hM)^{-1}\mathbf y^n$ and amplification eigenvalues $g_\pm=(1-h\lambda_\pm)^{-1}$. Hence

$$
\boxed{|g_\pm|^2=\frac1{(1+\gamma h)^2+(k^2-\gamma^2)h^2}=\frac1{1+2\gamma h+k^2h^2}\le1}
$$

for every $h\ge0$. It is therefore unconditionally stable for this [linear system](../../../../../system-of-linear-equations.md). Even with $\gamma=0$, it damps every nonzero numerical mode: stability is obtained at the cost of artificial damping and phase error. Large $h$ does not accurately resolve the oscillation period.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
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
