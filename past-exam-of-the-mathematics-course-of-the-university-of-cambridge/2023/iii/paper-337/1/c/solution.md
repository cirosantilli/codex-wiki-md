<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At zero temperature, the [Matsubara sum](../../../../../../bosonic-matsubara-sum.md) becomes a frequency integral:

$$
\frac1{vg}
=\int_{|\mathbf k|<\Lambda}\frac{d^2k}{(2\pi)^2}
\int_{-\infty}^{\infty}\frac{d\omega}{2\pi}
\frac1{\omega^2+v^2k^2+m^2}.
$$

The frequency integral is $1/(2\sqrt{v^2k^2+m^2})$, and radial momentum integration gives

$$
\frac1{vg}
=\frac{\sqrt{v^2\Lambda^2+m^2}-m}{4\pi v^2}.
$$

Define the [critical coupling](../../../../../../critical-coupling.md) by the massless equation

$$
\frac1{vg_c}=\frac{\Lambda}{4\pi v}.
$$

Taking the cutoff to infinity in the difference gives

$$
\frac1g-\frac1{g_c}=-\frac{m}{4\pi v},
$$

and hence

$$
\boxed{m=\frac{4\pi v(g-g_c)}{gg_c}.}
$$

A positive mass solution exists only for $g>g_c$. For $g<g_c$, the symmetric saddle cannot enforce the constraint with $m^2>0$; instead the $O(N)$ symmetry is [spontaneously broken](../../../../../../spontaneous-symmetry-breaking.md) to $O(N-1)$, the field acquires [Néel order](../../../../../../neel-state.md), and the ordered phase contains massless [Goldstone bosons](../../../../../../goldstone-boson.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
