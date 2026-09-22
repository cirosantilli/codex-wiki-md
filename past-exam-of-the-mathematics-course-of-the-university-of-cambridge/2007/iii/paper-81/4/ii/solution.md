<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With $x=\cos\theta$ and $D_r=0$, the [Fokker-Planck equation](../../../../../../fokker-planck-equation.md) becomes the probability-transport equation

$$
Bf_t+(1-x^2)f_x-2xf=0,
\qquad
\partial_tf+\partial_x\left[\frac{1-x^2}{B}f\right]=0.
$$

Its characteristic obeys $\dot x=(1-x^2)/B$. Writing $s=t/B$ and $q=\tanh s$ gives

$$
x=\frac{x_0+q}{1+qx_0},\qquad x_0=\frac{x-q}{1-qx},\qquad
\frac{dx_0}{dx}=\frac{1-q^2}{(1-qx)^2}.
$$

Conservation of orientation probability pushes the initially uniform density forward by this Jacobian. Thus

$$
f(x,t)=\frac{1-q^2}{4\pi(1-qx)^2}.
$$

Since $q=(1-\alpha)/(1+\alpha)$ with $\alpha=e^{-2t/B}$, the [deterministic alignment of an initially isotropic orientation distribution](../../../../../../deterministic-alignment-of-an-initially-isotropic-orientation-distribution.md) is

$$
\boxed{f(\theta,t)=\frac{\alpha}{\pi[1+\alpha-(1-\alpha)\cos\theta]^2}.}
$$

At $t=0$, $\alpha=1$ and $f=1/(4\pi)$; the characteristic Jacobian preserves $2\pi\int_{-1}^1f\,dx=1$ at every finite time. Its reciprocal is quadratic in $x$, as in the suggested substitution.

To compute the mean, integrate explicitly:

$$
\begin{aligned}
\langle x\rangle
&=\frac{1-q^2}{2}\int_{-1}^1\frac{x\,dx}{(1-qx)^2}\\
&=\frac1q+\frac{1-q^2}{2q^2}\log\frac{1-q}{1+q}
=\coth s-s\operatorname{csch}^2s.
\end{aligned}
$$

Consequently

$$
\boxed{\mathbf V_c(t)=V_s\left[\coth(t/B)-\frac{t}{B}\operatorname{csch}^2(t/B)\right]\mathbf k.}
$$

The apparent singularity at $t=0$ is removable: $\langle x\rangle=2t/(3B)+O((t/B)^3)$, so the initial mean is zero. At late times,

$$
1-\langle x\rangle=(4t/B-2)e^{-2t/B}+O((t/B)e^{-4t/B}).
$$

Except for the exactly downward initial orientation, which has zero probability in the initial smooth distribution, every characteristic aligns upward. The infinite-time orientation distribution is a point mass at the upward pole.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
