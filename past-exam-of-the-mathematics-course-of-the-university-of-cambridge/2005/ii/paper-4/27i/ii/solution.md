<h1 id="27i/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $\alpha,\beta,\kappa>0$, with the given gamma using shape and rate. Put

$$
m_i=\frac{\kappa}{1+\kappa}X_i,\qquad
A=\alpha+\frac n2,\qquad
B=\beta+\frac{\kappa}{2(1+\kappa)}\sum_iX_i^2.
$$

The joint posterior density before normalization is

$$
\pi(\theta,\tau\mid X)\propto
\tau^{\alpha+n-1}
\exp\!\left[-\tau\left\{\beta+\frac12\sum_i[\theta_i^2+\kappa(X_i-\theta_i)^2]\right\}\right].
$$

Complete each square and integrate over all $\theta_i$. The Gaussian integral contributes $\tau^{-n/2}$, giving

$$
\boxed{\tau\mid X\sim\operatorname{Gamma}(A,B),\qquad
\theta\mid\tau,X\sim
N_n\!\left(m,\frac1{(1+\kappa)\tau}I_n\right)}.
$$

This hierarchical form completely specifies the [normal-gamma distribution](../../../../../../normal-gamma-distribution.md) of the posterior. For comparison, $\tau\mid\theta,X$ has shape $\alpha+n$ and rate $\beta+\tfrac12\sum_i[\theta_i^2+\kappa(X_i-\theta_i)^2]$; confusing this conditional shape with the marginal shape would lose the Gaussian-integration factor.

Marginally $\theta$ has a multivariate Student distribution with $2A=2\alpha+n$ degrees of freedom and scale [matrix](../../../../../../matrix.md) $B/[A(1+\kappa)]\,I_n$. The coordinates are conditionally independent given $\tau$, but are generally dependent after integrating their shared precision. This is conjugate shrinkage with uncertainty in the overall noise scale.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [27I](../../27i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
