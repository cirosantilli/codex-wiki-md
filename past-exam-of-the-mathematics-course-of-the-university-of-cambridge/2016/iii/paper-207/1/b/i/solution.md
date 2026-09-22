<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The three independent [sample means](../../../../../../../sample-mean.md) satisfy $\overline Y_i\sim\mathcal N(\mu_i,v_i)$. A linear transformation of their joint [multivariate normal distribution](../../../../../../../multivariate-normal-distribution.md) is again normal. The two treatment contrasts have [covariance](../../../../../../../covariance.md)

$$
\operatorname{Cov}(\overline Y_1-\overline Y_0,\overline Y_2-\overline Y_0)=\operatorname{Var}(\overline Y_0)=v_0.
$$

Writing $m_i=\delta_i/s_i$ and $\rho=v_0/(s_1s_2)$, **their joint distribution** is

$$
\boxed{\begin{pmatrix}W_1\\W_2\end{pmatrix}\sim\mathcal N_2\left(\begin{pmatrix}m_1\\m_2\end{pmatrix},\begin{pmatrix}1&\rho\\\rho&1\end{pmatrix}\right).}
$$

The positive [correlation coefficient](../../../../../../../pearson-correlation-coefficient.md) arises from the shared control arm. Under positive variances, $0<\rho<1$. 

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
