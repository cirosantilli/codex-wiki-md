<h1 id="19/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\epsilon_k=E_0(k+\tfrac12)$ and use [Lagrange multipliers](../../../../../lagrange-multiplier.md) $\alpha,\beta$ for the particle-number and energy constraints. The stationary equations are

$$
\frac{\partial}{\partial n_k}\left[-\sum_j(n_j\ln n_j-n_j)-\alpha\left(\sum_jn_j-N\right)-\beta\left(\sum_j\epsilon_jn_j-E\right)\right]
=-\ln n_k-\alpha-\beta\epsilon_k=0.
$$

Thus $n_k=e^{-\alpha}e^{-\beta\epsilon_k}$. Finite normalization over infinitely many levels requires $\beta>0$. Put $q=e^{-\beta E_0}$, so $0<q<1$. The [geometric series](../../../../../geometric-series.md) gives

$$
N=e^{-\alpha}\frac{e^{-\beta E_0/2}}{1-q},\qquad
e^{-\alpha}=N(1-q)e^{\beta E_0/2}=2N\sinh\frac{\beta E_0}{2}.
$$

Therefore

$$
\boxed{n_k=2N\sinh\left(\frac{\beta E_0}{2}\right)e^{-\beta E_0(k+1/2)}.}
$$

For the energy constraint, use $n_k=N(1-q)q^k$ and $\sum kq^k=q/(1-q)^2$, obtained by differentiating the [geometric series](../../../../../geometric-series.md). This yields

$$
\frac E{NE_0}=(1-q)\sum_{k=0}^\infty\left(k+\frac12\right)q^k
=\frac12+\frac q{1-q}=\frac{1+q}{2(1-q)}.
$$

Recognizing the [hyperbolic cotangent](../../../../../hyperbolic-cotangent.md) gives

$$
\boxed{E=\frac{NE_0}{2}\coth\left(\frac{\beta E_0}{2}\right).}
$$

The strict positivity of all occupations requires $E>NE_0/2$; the paper's positivity assumptions alone do not guarantee this feasibility condition. For admissible energy the multiplier is uniquely $\beta=E_0^{-1}\ln[(2E+NE_0)/(2E-NE_0)]>0$. Equality $E=NE_0/2$ is only the limiting state with all occupation in level zero, outside the stipulated strictly positive family; lower energy is impossible.

For rigor beyond formal multiplier equations, $p_k=n_k/N$ has fixed mean $E/(NE_0)-1/2$. The objective differs from $N$ times its [information entropy](../../../../../information-entropy-split.md) only by the fixed constant $N-N\ln N$. The [maximum entropy distribution on the nonnegative integers](../../../../../maximum-entropy-distribution-on-the-nonnegative-integers.md) is uniquely geometric at that mean, confirming the stationary family and its maximum character.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
