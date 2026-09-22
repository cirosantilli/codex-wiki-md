<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $D_r>0$, the steady polar flux satisfies $\partial_\theta(\sin\theta j_\theta)=0$. Regularity at both poles makes its integration constant zero. Thus

$$
D_rf_{0,\theta}=-\frac{\sin\theta}{B}f_0,\qquad
f_0=C e^{\Lambda\cos\theta},\qquad \Lambda=(BD_r)^{-1}.
$$

Normalize with $x=\cos\theta$:

$$
1=2\pi C\int_{-1}^1e^{\Lambda x}dx=4\pi C\frac{\sinh\Lambda}{\Lambda}.
$$

The [zero-flow steady gyrotactic orientation distribution](../../../../../../zero-flow-steady-gyrotactic-orientation-distribution.md) is therefore

$$
\boxed{f_0(\theta)=\frac{\Lambda e^{\Lambda\cos\theta}}{4\pi\sinh\Lambda}.}
$$

Differentiating the logarithm of its normalization integral gives the [Langevin function](../../../../../../langevin-function.md) mean

$$
\langle\cos\theta\rangle_0=\frac{d}{d\Lambda}\log\frac{\sinh\Lambda}{\Lambda}
=\coth\Lambda-\frac1\Lambda,
\qquad
\boxed{\mathbf V_c=V_s\left(\coth\Lambda-\frac1\Lambda\right)\mathbf k.}
$$

As $\Lambda\to0$, $f_0\to1/(4\pi)$ and the mean tends to zero; as $\Lambda\to\infty$, the distribution concentrates at the upward pole and the mean tends to $V_s\mathbf k$. At zero [diffusivity](../../../../../../diffusion-coefficient.md) the pole-concentrated steady state is a probability measure, not a regular density of this formula.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
