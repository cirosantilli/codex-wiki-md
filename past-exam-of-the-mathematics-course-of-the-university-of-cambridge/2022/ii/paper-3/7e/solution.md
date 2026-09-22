<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Taking the [Laplace transform](../../../../../laplace-transform.md) in $t$ and using the zero initial condition gives

$$
p\widetilde T=\kappa\widetilde T_{xx}.
$$

The solution bounded as $x\to\infty$ is

$$
\widetilde T(x,p)=\widetilde T_0(p)
\exp\left(-x\sqrt{\frac p\kappa}\right).
$$

The transformed boundary condition is

$$
\boxed{\widetilde T_0(p)=\frac{\omega}{p^2+\omega^2}},
$$

so this is the [sinusoidally forced heat equation on a half-line](../../../../../sinusoidally-forced-heat-equation-on-a-half-line.md). Integrating in $x$ gives

$$
\boxed{
\widetilde I(p)
=\int_0^\infty\widetilde T(x,p)\,dx
=\frac{\omega\sqrt\kappa}
{\sqrt p\,(p^2+\omega^2)}
}.
$$

Use the principal square root, with a [branch cut](../../../../../branch-cut.md) along the negative real axis. The [Bromwich contour](../../../../../bromwich-contour.md) is a vertical line to the right of $p=\pm i\omega$ and the branch point $p=0$. For $t>0$, close it in the left half-plane, indent around the cut, and let the large semicircle recede. The simple poles at $p=\pm i\omega$ contribute

$$
\sqrt{\frac{\kappa}{\omega}}
\cos\left(\omega t-\frac{3\pi}{4}\right)
=-\sqrt{\frac{\kappa}{2\omega}}\cos\omega t
+\sqrt{\frac{\kappa}{2\omega}}\sin\omega t.
$$

Hence

$$
\boxed{A=-\sqrt{\frac{\kappa}{2\omega}}},
\qquad
\boxed{B=\sqrt{\frac{\kappa}{2\omega}}}.
$$

On the upper and lower sides of the cut, put $p=-s$; the two values of $\sqrt p$ are $i\sqrt s$ and $-i\sqrt s$. Their jump and the opposite contour orientations combine to give

$$
\frac1\pi\int_0^\infty
\frac{\omega\sqrt\kappa\,e^{-st}}
{(s^2+\omega^2)\sqrt s}\,ds.
$$

This is precisely [Bromwich inversion with a square-root branch cut](../../../../../bromwich-inversion-with-a-square-root-branch-cut.md): the residues produce the permanent periodic response, while the cut integral is the transient that decays with time.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
