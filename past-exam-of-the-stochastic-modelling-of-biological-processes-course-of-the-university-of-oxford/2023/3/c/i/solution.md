<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $c=c_1=c_3$, so the friction [memory kernel](../../../../../memory-kernel.md) is $\kappa_c(t)=ce^{-ct}$ and has area one for every $c>0$. Its [Laplace transform](../../../../../laplace-transform.md) is $\widetilde\kappa_c(s)=c/(s+c)$. The [generalized fluctuation-dissipation relation](../../../../../generalized-fluctuation-dissipation-relation.md) therefore gives

$$
\widetilde\chi_c(s)=\frac5{s+c/(s+c)}
=\frac{5(s+c)}{s^2+cs+c}
\longrightarrow\frac5{s+1}
\quad(c\to\infty).
$$

To verify the pointwise time-domain limit, rather than relying only on [Laplace transform](../../../../../laplace-transform.md) convergence, consider $c>4$. The two roots

$$
\lambda_\pm=\frac{-c\pm\sqrt{c^2-4c}}2
$$

are negative and satisfy $\lambda_+\to-1$, $\lambda_-\to-\infty$. Since $\chi_c(0)=5$ and $\chi_c'(0)=0$, the inverse [Laplace transform](../../../../../laplace-transform.md) is

$$
\chi_c(\tau)=5\frac{-\lambda_-e^{\lambda_+\tau}+\lambda_+e^{\lambda_-\tau}}{\lambda_+-\lambda_-}.
$$

The coefficient of the slow exponential tends to $5$, and that of the fast exponential tends to zero. Hence

$$
\boxed{\lim_{c_1\to\infty}\chi(\tau)=5e^{-\tau},\qquad \tau\geq0.}
$$

This is the [velocity](../../../../../velocity.md) [autocorrelation function](../../../../../autocorrelation.md) of an [Ornstein-Uhlenbeck process](../../../../../ornstein-uhlenbeck-process.md) satisfying $dV=-V\,dt+\sqrt{10}\,dW$. The friction [memory kernel](../../../../../memory-kernel.md) becomes local in time. Consistently, the even noise [autocorrelation](../../../../../autocorrelation.md) $5ce^{-c|\tau|}$ tends to $10\delta(\tau)$ in the sense of [distributions](../../../../../distribution-mathematical-analysis.md), fixing the [white noise](../../../../../white-noise.md) normalization. The finite-$c$ right derivative $\chi_c'(0)=0$ does not converge to the right derivative $-5$ of the limiting function: there is a short initial relaxation layer.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the stochastic modelling of biological processes course of the University of Oxford](../../../../split.md)
6. [Stochastic modelling of biological processes course of the University of Oxford](../../../../../stochastic-modelling-of-biological-processes-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
