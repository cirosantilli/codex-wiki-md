<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The SI [volume](../../../../volume.md) [magnetic susceptibility](../../../../magnetic-susceptibility.md) is the weak-field response $\chi_M=\partial M/\partial H$, or $M/H$ for a linear isotropic sample with no spontaneous moment. It is dimensionless; a molar susceptibility would be a different quantity. For weak [magnetization](../../../../magnetization.md), $B\simeq\mu_0H$. Neglect local-field and demagnetizing corrections in this independent-spin model.

A spin-$1/2$ ion has moment projections $\pm g\mu_B/2$. The requested coefficient assumes a spin-only $g\simeq2$, giving projections $\pm\mu_B$ and Zeeman energies $\mp\mu_BB$. With $x=\mu_BB/(k_BT)$, the one-ion [partition function](../../../../canonical-partition-function.md) and [magnetization](../../../../magnetization.md) are

$$
Z_1=e^x+e^{-x}=2\cosh x,\qquad
M=N\mu_B\frac{e^x-e^{-x}}{e^x+e^{-x}}=N\mu_B\tanh x.
$$

For $|x|\ll1$, $\tanh x\simeq x$, so

$$
\boxed{\chi_M\simeq\mu_0\frac{\partial M}{\partial B}
=\frac{N\mu_0\mu_B^2}{k_BT}.}
$$

Here $N$ is a [number density](../../../../number-density.md), as specified, rather than total ion number. The small-field condition is

$$
\boxed{\mu_B|B|\ll k_BT,}
$$

meaning the Zeeman splitting $2\mu_BB$ is small compared with the thermal scale up to an irrelevant order-one convention. It is not a temperature-independent absolute upper bound on $B$. For a different $g$ value the coefficient contains $(g\mu_B/2)^2$ instead of $\mu_B^2$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
