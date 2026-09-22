<h1 id="1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the same finite truncation $T_m(h)=\sum_{j\leq m}\langle h,e_j\rangle A_j$ for $f$ and $g$. Since $\mathbb E[A_iA_j]=\delta_{ij}$ by [independence](../../../../../independent-random-variables.md), zero [means](../../../../../expected-value-split.md) and unit [variances](../../../../../variance-split.md),

$$
\mathbb E[T_m(f)T_m(g)]
=\sum_{j\leq m}\langle f,e_j\rangle\langle g,e_j\rangle.
$$

Here $\delta_{ij}$ is the [Kronecker delta](../../../../../kronecker-delta.md). The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and [convergence in L2](../../../../../convergence-in-l2.md) justify passing to the limit in the product's [expectation](../../../../../expected-value-split.md). The [Parseval identity for a Hilbertian basis](../../../../../parseval-identity-for-a-hilbertian-basis.md) now gives

$$
\boxed{\mathbb E[(Wf)(Wg)]=\langle f,g\rangle_{\mathcal H}
=\int_0^1f(t)g(t)\,dt.}
$$

Because each $Wh$ has [mean](../../../../../expected-value-split.md) zero, this is also its [covariance](../../../../../covariance.md) identity. Thus $W$ is an [isonormal Gaussian process](../../../../../isonormal-gaussian-process.md) over $\mathcal H$.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
