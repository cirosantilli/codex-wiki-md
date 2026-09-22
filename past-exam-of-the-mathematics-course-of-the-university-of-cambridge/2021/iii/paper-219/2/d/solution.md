<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For draw $m$, let $C_m$ be the observed covariance matrix, $k_{*m}=(k_{\theta_m}(t_*,t_i))_i$, and

$$
m_{*m}=\mu_m+k_{*m}^TC_m^{-1}(y-\mu_m\mathbf1),\qquad
v_{*m}=A_m-k_{*m}^TC_m^{-1}k_{*m}.
$$

The posterior predictive distribution is a mixture of these conditional Gaussians. Its Monte Carlo mean and variance are

$$
\boxed{\widehat m_*=\frac1M\sum_mm_{*m},\qquad
\widehat v_*=\frac1M\sum_m(v_{*m}+m_{*m}^2)-\widehat m_*^2.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
