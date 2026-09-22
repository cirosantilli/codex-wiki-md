<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

For nonnegative insect density assume $N_0>0$. Substitution of $N=e^{\alpha t}R$ gives $R_t=D e^{2\alpha t}(R^2R_x)_x$, so choose

$$
\boxed{\tau(t)=\begin{cases}\dfrac{D}{2\alpha}(e^{2\alpha t}-1)&\alpha\ne0,\\Dt&\alpha=0.\end{cases}}
$$

Then $\tau'=De^{2\alpha t}>0$ and the [porous medium equation](../../../../../porous-medium-equation.md) is $R_\tau=(R^2R_x)_x$. Its total mass is conserved when the flux vanishes at infinity. For the mass-preserving [similarity solution](../../../../../similarity-solution.md), direct differentiation gives

$$
R_\tau=-\frac14\tau^{-5/4}(F+\xi F'),\qquad
(R^2R_x)_x=\tau^{-5/4}(F^2F')',
\qquad \int_{\mathbb R}F\,d\xi=N_0.
$$

On the positive support, integrating once with zero boundary flux gives $F^2F'=-\xi F/4$ and hence $F^2=(\xi_0^2-\xi^2)/4$. The semicircle mass [integral](../../../../../integral.md) is $\pi\xi_0^2/4=N_0$, confirming the profile and its symmetric [compact support](../../../../../compact-support.md).

The front is at $|x|=\xi_0\tau^{1/4}$. When $\alpha<0$, $\tau(t)$ increases towards $D/(2|\alpha|)$, so the supremum of the distance reached is

$$
\boxed{x_{\max}=\sqrt{\frac{4N_0}{\pi}}\left(\frac{D}{2|\alpha|}\right)^{1/4}}.
$$

It is approached as $t\to\infty$, rather than attained at a finite time. If $N_0=0$, the nonnegative solution is identically zero and the corresponding distance is zero.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
