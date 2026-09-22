<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [logarithm](../../../../logarithm.md) of the geometric average is

$$
\log\overline S_T=\log S_0+\frac12(r-\sigma^2/2)T+\frac\sigma T\int_0^T W_u^{\mathbb Q}\,du.
$$

By [stochastic Fubini theorem](../../../../stochastic-fubini-theorem.md), $\int_0^TW_u\,du=\int_0^T(T-v)\,dW_v$, a centered [Gaussian random variable](../../../../gaussian-random-variable.md) with [variance](../../../../variance-split.md) $T^3/3$. Therefore

$$
\log((\overline S_T)^p)\sim N(m,v),\qquad
m=p\left[\log S_0+\frac12(r-\sigma^2/2)T\right],\quad v=\frac{p^2\sigma^2T}{3}.
$$

The [Geometric Asian option](../../../../geometric-asian-option.md) is consequently a call on this [lognormal random variable](../../../../lognormal-random-variable.md). Completing the square as in part [c](../c.md) gives

$$
\boxed{e^{-rT}\left[e^{m+v/2}\Phi(d_1)-K\Phi(d_2)\right],\qquad
d_2=\frac{m-\log K}{\sqrt v},\quad d_1=d_2+\sqrt v.}
$$

The averaging changes both the log-mean and log-variance; replacing $S_T$ by an ordinary stock price at a shorter maturity without these adjustments would give the wrong formula.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
