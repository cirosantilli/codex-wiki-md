<h1 id="26k/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Finite independent Gaussian sums are Gaussian; directly, multiplication of their [characteristic functions](../../../../../../characteristic-function.md) gives

$$
\varphi_{Y_n}(t)=\prod_{j=1}^ne^{-\alpha_j^2t^2/2}=\exp\left(-\frac{t^2}{2}\sum_{j=1}^n\alpha_j^2\right)\longrightarrow e^{-\sigma^2t^2/2}.
$$

By [Markov inequality](../../../../../../markov-inequality.md), $\mathbb P(|Y_n-Y|>\epsilon)\leq\epsilon^{-2}\|Y_n-Y\|_2^2\to0$. Part (ii) makes the same sequence converge in distribution to $Y$, and the characteristic-function estimate there makes $\varphi_{Y_n}\to\varphi_Y$. Uniqueness of distributions determined by characteristic functions therefore yields

$$
\boxed{Y\sim N(0,\sigma^2).}
$$

If $\sigma^2=0$, all coefficients vanish and $Y=0$ almost surely; $N(0,0)$ here denotes that degenerate distribution.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [26K](../../26k.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
