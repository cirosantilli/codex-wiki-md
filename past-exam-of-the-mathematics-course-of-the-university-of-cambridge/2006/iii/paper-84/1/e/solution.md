<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

An odd number of inhibitory connections gives $\Gamma<0$. Write $r=|\Gamma|^{1/3}>0$. The cube roots of $-r^3$ have arguments $\pi,\pi/3,-\pi/3$, so

$$
\boxed{\lambda_0=\frac{-1-r}\tau,\qquad\lambda_\pm=\frac{-1+r/2\pm i\sqrt3r/2}\tau}.
$$

The real mode is always damped. The pair has negative real part precisely when $r\cos(\pi/3)<1$, giving

$$
\boxed{r<2\quad\Longleftrightarrow\quad -8<\Gamma<0}
$$

for strict linear asymptotic stability. For $r>2$ the origin is unstable to an oscillatory mode.

At $r=2=1/\cos(\pi/3)$ the eigenvalues are $-3/\tau$ and $\pm i\sqrt3/\tau$. Thus the linear oscillation frequency is $\boxed{\omega_H=\sqrt3/\tau}$ and its period is $2\pi\tau/\sqrt3$. Varying $r$ crosses the imaginary axis transversely, since $d\operatorname{Re}\lambda_+/dr=1/(2\tau)>0$.

The [hyperbolic tangent](../../../../../../hyperbolic-tangent.md) has a negative cubic saturation and no quadratic term. To check the nonlinear onset, let $v$ be a critical complex eigenvector of $M=\beta W$ and $p$ its normalized adjoint eigenvector, with $p^*v=1$. For this weighted cycle, $\overline p_i v_i=1/3$. Since $Mv=(1+i\sqrt3)v$, the cubic derivative evaluated on $(v,v,\overline v)$ has projection

$$
p^*C(v,v,\overline v)=-\frac{2\beta^2}{3\tau}(1+i\sqrt3)\sum_i|v_i|^2.
$$

Its real part is strictly negative. With no quadratic contributions, this gives a negative first Lyapunov coefficient: **the generic onset is a supercritical Hopf bifurcation**, with a small attracting periodic orbit just beyond the threshold. Exactly at threshold the linear system has undamped oscillations, but nonlinear cubic damping makes sufficiently small oscillations decay; one must not infer a nonzero sustained cycle at the critical parameter solely from the imaginary eigenvalues.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
