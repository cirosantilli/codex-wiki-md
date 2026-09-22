<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The finite-temperature gap equation is

$$
\frac1{vg}
=\int_{|\mathbf k|<\Lambda}
\frac{d^2k}{(2\pi)^2}
\frac1{2E_k}\coth\left(\frac{E_k}{2T}\right).
$$

With $E=\sqrt{v^2k^2+m^2}$, the radial measure obeys $k\,dk=E\,dE/v^2$, so

$$
\frac1{vg}
=\frac{T}{2\pi v^2}
\left[
\log\sinh\left(\frac{E}{2T}\right)
\right]_{m}^{\sqrt{v^2\Lambda^2+m^2}}.
$$

As $\Lambda\to\infty$, subtraction of the massless, zero-temperature equation at $g_c$ leaves

$$
\frac1{vg}-\frac1{vg_c}
=-\frac{T}{2\pi v^2}
\log\left[2\sinh\left(\frac{m}{2T}\right)\right].
$$

The zero-temperature relation with $m=\Delta$ is

$$
\frac1{vg}-\frac1{vg_c}
=-\frac{\Delta}{4\pi v^2}.
$$

Equating the finite parts gives

$$
2\sinh\left(\frac{m}{2T}\right)=e^{\Delta/(2T)},
$$

and therefore

$$
\boxed{
m(T)=2T\operatorname{arsinh}
\left(\frac12e^{\Delta/(2T)}\right).}
$$

The subtraction is a [renormalization condition](../../../../../../renormalization-condition.md): it trades the cutoff-dependent bare coupling for the physical zero-temperature gap.

## ↑ Ancestors (11)

1. [E](../e.md)
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
