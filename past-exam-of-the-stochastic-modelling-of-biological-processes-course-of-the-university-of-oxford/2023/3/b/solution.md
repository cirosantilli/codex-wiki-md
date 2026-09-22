<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $c_1=2$, $c_2=4$, $c_3=5$, the friction [memory kernel](../../../../memory-kernel.md) and its [Laplace transform](../../../../laplace-transform.md) are

$$
\kappa(t)=2(1+4t)e^{-5t},
\qquad
\widetilde\kappa(s)=\frac2{s+5}+\frac8{(s+5)^2}
=\frac{2(s+9)}{(s+5)^2}.
$$

Using the [generalized fluctuation-dissipation relation](../../../../generalized-fluctuation-dissipation-relation.md) with equilibrium [velocity](../../../../velocity.md) [variance](../../../../variance-split.md) $5$, the [velocity](../../../../velocity.md) [autocorrelation function](../../../../autocorrelation.md) has [Laplace transform](../../../../laplace-transform.md)

$$
\begin{aligned}
\widetilde\chi(s)
&=\frac5{s+\widetilde\kappa(s)}\\
&=\frac{5(s+5)^2}{s(s+5)^2+2(s+9)}\\
&=\frac{5(s+5)^2}{s^3+10s^2+27s+18}\\
&=\frac{5(s+5)^2}{(s+1)(s+3)(s+6)}.
\end{aligned}
$$

All three poles are negative, so the stationary relaxation is stable. A [partial fraction decomposition](../../../../partial-fraction-decomposition.md) gives

$$
\widetilde\chi(s)=\frac8{s+1}-\frac{10/3}{s+3}+\frac{1/3}{s+6}.
$$

Taking the inverse [Laplace transform](../../../../laplace-transform.md) gives

$$
\boxed{\chi(\tau)=8e^{-\tau}-\frac{10}3e^{-3\tau}+\frac13e^{-6\tau},\qquad \tau\geq0.}
$$

The negative middle coefficient is compatible with an [autocorrelation function](../../../../autocorrelation.md); individual terms in a [partial fraction decomposition](../../../../partial-fraction-decomposition.md) need not themselves be separate physical modes with positive weights. Several useful checks follow directly:

$$
\chi(0)=8-\frac{10}3+\frac13=5,
\qquad
\chi'(0)=-8+10-2=0,
\qquad
\chi''(0)=8-30+12=-10.
$$

The [Volterra integral equation](../../../../volterra-integral-equation.md) for $\chi$ predicts exactly $\chi'(0)=0$ and $\chi''(0)=-\kappa(0)\chi(0)=-10$. Its [integral](../../../../integral-split.md) is also $8-10/9+1/18=125/18=5/\widetilde\kappa(0)$, agreeing with the [Green-Kubo formula for diffusion](../../../../green-kubo-formula-for-diffusion.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the stochastic modelling of biological processes course of the University of Oxford](../../../split.md)
5. [Stochastic modelling of biological processes course of the University of Oxford](../../../../stochastic-modelling-of-biological-processes-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
