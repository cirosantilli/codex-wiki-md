<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the proposed [joint probability density](../../../../../joint-probability-density.md) $\rho$, define the acceptance [indicator function](../../../../../indicator-function.md)

$$
A_i:=\mathbf1_{\{V_i\leq w(Y_i)/M\}}.
$$

On the proposal's [support](../../../../../support.md) the [importance weight](../../../../../importance-weight.md) is $\pi(Y_i,V_i)/\rho(Y_i,V_i)=MA_i$. Therefore the requested augmented-space [importance sampling](../../../../../importance-sampling.md) estimator is

$$
\boxed{\widehat\theta_n^{\mathrm{IS}}=\frac Mn\sum_{i=1}^nA_i\phi(Y_i).}
$$

Its [expected value](../../../../../expected-value-split.md) is $\theta$, provided $\mathbb E_p|\phi(X)|<\infty$. This is not the ordinary estimator $n^{-1}\sum_iw(Y_i)\phi(Y_i)$ from question 1. Taking the [conditional expectation](../../../../../conditional-expectation.md) of this augmented estimator given all $Y_i$ produces that ordinary estimator, because $\mathbb E[A_i\mid Y_i]=w(Y_i)/M$. This is the [Rao-Blackwell identity for a fixed-denominator rejection estimator](../../../../../rao-blackwell-identity-for-a-fixed-denominator-rejection-estimator.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
