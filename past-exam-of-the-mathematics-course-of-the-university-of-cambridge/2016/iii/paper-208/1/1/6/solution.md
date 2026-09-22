<h1 id="1/1/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the original-noise coefficients $\psi_0=1$ and $\psi_j=-11\cdot4^{-j}$ for $j\geq1$. The [autocovariance function](../../../../../../../autocovariance.md) of a causal linear process is $\gamma_X(h)=\sum_{j\geq0}\psi_j\psi_{j+|h|}$, since the original noise has [variance](../../../../../../../variance-split.md) $1$. Thus

$$
\gamma_X(0)=1+121\sum_{j\geq1}16^{-j}=1+\frac{121}{15}=\frac{136}{15}.
$$

For $h\geq1$,

$$
\gamma_X(h)=4^{-h}\left(-11+121\sum_{j\geq1}16^{-j}\right)=-\frac{44}{15}\,4^{-h}.
$$

By [covariance](../../../../../../../covariance.md) symmetry,

$$
\boxed{\gamma_X(h)=\begin{cases}136/15,&h=0,\\-(44/15)4^{-|h|},&h\ne0.\end{cases}}
$$

In particular, all nonzero-lag [covariances](../../../../../../../covariance.md) are negative, despite the positive autoregressive coefficient.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 208](../../../../paper-208-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
