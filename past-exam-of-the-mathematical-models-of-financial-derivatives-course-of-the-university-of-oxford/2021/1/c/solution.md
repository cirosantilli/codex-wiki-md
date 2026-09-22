<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The discounted stock over the remaining horizon satisfies

$$
e^{-r\tau}S_T=s+\sigma\int_t^T e^{-r(u-t)}\,dW_u^{\mathbb Q}.
$$

The [Itô integral](../../../../ito-integral.md) on the right is a centered [normal random variable](../../../../gaussian-random-variable.md) with [variance](../../../../variance-split.md) $a_\tau=(1-e^{-2r\tau})/(2r)$. Therefore $\mathbb Q(S_T\geq0\mid S_t=s)=\Phi(d)$, where $d=s/(\sigma\sqrt{a_\tau})$. The [digital option](../../../../binary-option.md) price and its [option delta](../../../../option-delta.md) are

$$
\boxed{V(t,s)=e^{-r\tau}\Phi(d),\qquad
\Delta(t,s)=\frac{e^{-r\tau}\phi(d)}{\sigma\sqrt{a_\tau}}.}
$$

The formula also shows $V(t,0)=e^{-r\tau}/2$ for every $t<T$. At maturity use the specified step payoff, including its chosen value one at zero; the terminal discontinuity is not removed by the earlier-time smoothing.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
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
