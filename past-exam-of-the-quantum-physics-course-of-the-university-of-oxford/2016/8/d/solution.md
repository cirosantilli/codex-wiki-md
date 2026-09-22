<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Direct [integration](../../../../integral-split.md) over [solid angle](../../../../solid-angle.md) gives

$$
1=2\pi|C|^2\int_0^\pi\sin^{2l+1}\theta\,d\theta
=4\pi|C|^2\frac{(2^l l!)^2}{(2l+1)!}.
$$

Thus $|C|=\sqrt{(2l+1)!/(4\pi)}/(2^l l!)$. Choosing the usual alternating sign convention,

$$
\boxed{Y_l^l=(-1)^l\frac{\sqrt{(2l+1)!}}{2^l l!\sqrt{4\pi}}\sin^l\theta\,e^{il\phi}.}
$$

Apply $L_-$ successively and divide by its ladder coefficient at each step. Explicitly,

$$
\boxed{Y_l^m=\sqrt{\frac{(l+m)!}{(2l)!(l-m)!}}\,\hbar^{-(l-m)}(L_-)^{l-m}Y_l^l.}
$$

The [normalization](../../../../normalization.md) follows because the product of the squared ladder coefficients is $\hbar^{2(l-m)}(2l)!(l-m)!/(l+m)!$. This constructs every [magnetic sublevel](../../../../magnetic-sublevel.md), including negative $m$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum physics course of the University of Oxford](../../../split.md)
5. [Quantum physics course of the University of Oxford](../../../../quantum-physics-course-of-the-university-of-oxford.md)
6. [Year 2 of the physics course of the University of Oxford](../../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
