<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First justify the dependence structure rather than assume that adjacent squares behave like an ordinary lag-one ARCH model. Write $Z_t=X_t^2$. Iterating its nonnegative recurrence gives

$$
Z_t=\alpha_0\sum_{k=0}^{m-1}\alpha_2^k\prod_{j=0}^k\varepsilon_{t-2j}^2
+\alpha_2^m\left(\prod_{j=0}^{m-1}\varepsilon_{t-2j}^2\right)Z_{t-2m}.
$$

The product coefficient has [expected value](../../../../../../expected-value.md) $\alpha_2^m$, so it tends to zero in probability. The stationary $Z_{t-2m}$ are a tight family; consequently the remainder tends to zero in probability, without needing [independence](../../../../../../independent-random-variables.md) between that remainder's factors. The increasing partial sums therefore give the representation

$$
Z_t=\alpha_0\sum_{k\geq0}\alpha_2^k\prod_{j=0}^k\varepsilon_{t-2j}^2\quad\text{almost surely}.
$$

This proves the [parity decomposition of a lag-two ARCH process](../../../../../../parity-decomposition-of-a-lag-two-arch-process.md): even and odd observations are functions of disjoint noise families. It also shows that the positive scale $\sigma_t$ is a function of past noise, independent of $\varepsilon_t$. The [conditional expectation](../../../../../../conditional-expectation.md) of $X_t$ given past noise is zero, and the second-moment recursion is $m_2=\alpha_0+\alpha_2m_2$. [independence](../../../../../../independent-random-variables.md) of the parity families gives the adjacent-square [covariance](../../../../../../covariance.md). Thus

$$
\boxed{\mathbb EX_t=0,\qquad m_2=\mathbb EX_t^2=\frac{\alpha_0}{1-\alpha_2},\qquad
\operatorname{Cov}(X_t^2,X_{t+1}^2)=0.}
$$

To establish finiteness of the [fourth moment](../../../../../../fourth-moment.md) before using its recursion, note that the $L^2$ norm of the $k$th term in the positive series for $Z_t$ is $\alpha_0\sqrt3(\alpha_2\sqrt3)^k$. The [triangle inequality](../../../../../../triangle-inequality.md) in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) makes the series square-integrable when $3\alpha_2^2<1$. [independence](../../../../../../independent-random-variables.md) of the current noise and past scale then yields

$$
m_4=3\mathbb E(\alpha_0+\alpha_2X_{t-2}^2)^2
=3\alpha_0^2+6\alpha_0\alpha_2m_2+3\alpha_2^2m_4,
$$

and hence

$$
\boxed{\mathbb EX_t^4=\frac{3\alpha_0^2(1+\alpha_2)}{(1-\alpha_2)(1-3\alpha_2^2)}\quad\text{if }3\alpha_2^2<1.}
$$

If $3\alpha_2^2\geq1$, a finite $m_4$ would make $(1-3\alpha_2^2)m_4=3\alpha_0^2+6\alpha_0\alpha_2m_2>0$, which is impossible. Its [fourth moment](../../../../../../fourth-moment.md) is then infinite. The adjacent-square product remains integrable by parity [independence](../../../../../../independent-random-variables.md), even in that case.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
