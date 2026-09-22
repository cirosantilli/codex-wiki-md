<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $\Delta_0=f(x^0)-f(x^*)$. Dividing the corrected estimate from part (c) by $k/(2L)$ gives the [averaged stationarity bound for stochastic gradient descent](../../../../averaged-stationarity-bound-for-stochastic-gradient-descent.md)

$$
\frac1k\sum_{j=0}^{k-1}\mathbb E\|\nabla f(X^j)\|^2\leq M+\frac{2L\Delta_0}{k}.
$$

The [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md), first within each [expectation](../../../../expected-value-split.md) and then over the $k$ indices, gives

$$
\frac1k\sum_{j=0}^{k-1}\mathbb E\|\nabla f(X^j)\|
\leq\left(\frac1k\sum_{j=0}^{k-1}\mathbb E\|\nabla f(X^j)\|^2\right)^{1/2}.
$$

Thus

$$
\boxed{\min_{0\leq j<k}\mathbb E\|\nabla f(X^j)\|\leq\sqrt{M+\frac{2L\Delta_0}{k}}\leq\sqrt M+\sqrt{\frac{2L\Delta_0}{k}}.}
$$

Equivalently, if $J$ is chosen independently of the run with the [discrete uniform distribution](../../../../discrete-uniform-distribution.md) on $\{0,\ldots,k-1\}$, then $\mathbb E\|\nabla f(X^J)\|^2\leq M+2L\Delta_0/k$. The same bound for the expected [Euclidean norm](../../../../euclidean-norm.md) follows by the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md).

**The guarantee is averaged or best-iterate stationarity.** It does not assert that every last iterate converges, or that the limiting [Euclidean norm](../../../../euclidean-norm.md) equals $\sqrt M$. The squared [gradient](../../../../gradient.md) bound has excess $O(k^{-1})$ above $M$; the displayed expected [Euclidean norm](../../../../euclidean-norm.md) bound is within $O(k^{-1/2})$ of $\sqrt M$, including the zero-noise case. For fixed $M>0$, it is sharper:

$$
\sqrt{M+\frac{2L\Delta_0}{k}}-\sqrt M
=\frac{2L\Delta_0/k}{\sqrt{M+2L\Delta_0/k}+\sqrt M}
\leq\frac{L\Delta_0}{k\sqrt M}.
$$

For example, to ensure $\min_{j<k}\mathbb E\|\nabla f(X^j)\|\leq\sqrt M+\varepsilon$ with $\varepsilon>0$, it suffices that $k\geq2L\Delta_0/(2\sqrt M\,\varepsilon+\varepsilon^2)$. The [big O notation](../../../../big-o-notation.md) here concerns these upper bounds, rather than an asserted asymptotic equality for the [stochastic gradient noise floor](../../../../stochastic-gradient-noise-floor.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the optimisation for data science course of the University of Oxford](../../../split.md)
5. [Optimisation for data science course of the University of Oxford](../../../../optimisation-for-data-science-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
