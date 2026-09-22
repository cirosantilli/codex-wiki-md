<h1 id="h/h2/solution">Solution</h1>

↑ **Parent:** [H2](../h2.md)

Write $q=(x,X)^T$, $M=\begin{pmatrix}a&b\\b&c\end{pmatrix}$ and $K=\begin{pmatrix}\alpha&\beta\\\beta&\gamma\end{pmatrix}$. The linear equations are $M\ddot q+Kq=0$. A [normal mode](../../../../normal-mode.md) has all coordinates oscillating with one frequency and fixed relative amplitudes, $q=v\cos(\omega t+\varphi)$. Its squared frequency solves

$$
\det(K-\omega^2M)=(\alpha-a\omega^2)(\gamma-c\omega^2)-(\beta-b\omega^2)^2=0,
$$

and its amplitude vector is a nonzero null vector of $K-\omega^2M$. The assumed distinct positive roots give two normal frequencies, their positive square roots.

For the rods let $\theta_1,\theta_2$ be their small inclinations from the downward vertical. To first order, $\theta_1=x/a$ and $\theta_2=(X-x)/(2a)$. The first rod has kinetic [energy](../../../../energy-split.md) $m\dot x^2/6$. The second has centre-of-mass horizontal velocity $(\dot x+\dot X)/2$ and angular velocity $(\dot X-\dot x)/(2a)$, giving

$$
T_2=\frac m4(\dot x+\dot X)^2+\frac m{12}(\dot X-\dot x)^2.
$$

Together these give $T=m(3\dot x^2+2\dot x\dot X+2\dot X^2)/6$. The centre-of-mass height changes give

$$
V=\frac{mga}{4}\theta_1^2+mga(\theta_1^2+\theta_2^2)
=\frac{mg}{4a}(6x^2-2xX+X^2),
$$

proving the displayed quadratic [Lagrangian](../../../../lagrangian.md).

Here $M=(m/3)\begin{pmatrix}3&1\\1&2\end{pmatrix}$ and $K=(mg/(2a))\begin{pmatrix}6&-1\\-1&1\end{pmatrix}$. Set $\lambda=2a\omega^2/(3g)$. The [determinant](../../../../determinant.md) equation reduces to $5\lambda^2-17\lambda+5=0$, so

$$
\boxed{\omega_\pm^2=\frac{3g}{20a}(17\pm3\sqrt{21})}.
$$

The first row of the mode equation gives $X/x=(6-3\lambda)/(1+\lambda)$. The actual rod-angle ratio is therefore

$$
\frac{\theta_2}{\theta_1}=\frac{5-4\lambda}{2(1+\lambda)}.
$$

It is positive for the smaller root and negative for the larger root. Thus **the low-frequency mode has the rods in phase, and the high-frequency mode has them out of phase**. Using the rod-angle ratio is necessary because $X$ is the displacement of the end of the second rod, not that rod's inclination.

## ↑ Ancestors (12)

1. [H2](../h2.md)
2. [H](../../h.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
