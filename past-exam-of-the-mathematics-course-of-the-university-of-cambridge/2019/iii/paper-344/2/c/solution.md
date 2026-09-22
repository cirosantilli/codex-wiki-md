<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Fourier transform](../../../../../../fourier-transform.md) turns $\nabla^2$ into multiplication by $-q^2$. Each Cartesian component is an [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md):

$$
\dot p_{q,i}=-r(q)p_{q,i}+f_{q,i},\qquad\boxed{r(q)=\Gamma(a+\kappa q^2).}
$$

Since $r(q)>0$, the transient from the remote past vanishes, and the integrating-factor solution is

$$
\boxed{p_q(t)=\int_{-\infty}^t f_q(s)e^{-r(q)(t-s)}\,ds.}
$$

Using the stated [Gaussian white noise](../../../../../../gaussian-white-noise.md) covariance and assuming $t_1\geq t_2$,

$$
\begin{aligned}
\langle p_{q,i}(t_1)p_{-q,j}(t_2)\rangle
&=2\Gamma k_BT\,\delta_{ij}\int_{-\infty}^{t_2}e^{-r(q)(t_1+t_2-2s)}\,ds\\
&=\delta_{ij}\frac{\Gamma k_BT}{r(q)}e^{-r(q)(t_1-t_2)}.
\end{aligned}
$$

Interchanging the times gives the stationary two-time [correlation function](../../../../../../correlation-function.md)

$$
\boxed{\langle p_{q,i}(t_1)p_{-q,j}(t_2)\rangle=\delta_{ij}\frac{k_BT}{a+\kappa q^2}e^{-\Gamma(a+\kappa q^2)|t_1-t_2|}.}
$$

At equal times this is the equilibrium [Gaussian field theory](../../../../../../gaussian-field-theory.md) covariance, and the decay time is $r(q)^{-1}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
