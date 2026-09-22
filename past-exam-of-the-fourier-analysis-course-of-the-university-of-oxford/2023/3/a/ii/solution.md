<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [distribution](../../../../../distribution-mathematical-analysis.md) $u$ is a $2\pi$ [periodic distribution](../../../../../periodic-distribution.md) when

$$
\boxed{\langle u,\theta(\cdot+2\pi)\rangle=\langle u,\theta\rangle\qquad(\theta\in C_c^\infty(\mathbb R)).}
$$

Iteration gives invariance under all integer multiples of $2\pi$. For a [tempered distribution](../../../../../tempered-distribution.md) the identity also holds for every [Schwartz function](../../../../../schwartz-function.md), since [test functions](../../../../../test-function.md) are dense in the [Schwartz space](../../../../../schwartz-space.md): multiplying by [cutoff functions](../../../../../cutoff-function.md) $\chi(x/R)$ equal to one near zero gives such an approximation in every [Schwartz seminorm](../../../../../schwartz-seminorm.md).

For $\phi\in\mathcal S(\mathbb R)$ define $a_k(x)=\Psi(x+2\pi k)\phi(x)$. The [smooth periodic partition of unity](../../../../../smooth-periodic-partition-of-unity.md) gives $\phi=\sum_ka_k$ with convergence in the [Schwartz space](../../../../../schwartz-space.md). Indeed, each $a_k$ is supported where $|x+2\pi k|\leq2\pi$, and the [generalized Leibniz rule](../../../../../generalized-leibniz-rule.md) and arbitrarily rapid decay of the [derivatives](../../../../../derivative.md) of $\phi$ give, for every $m,n,M$,

$$
p_{m,n}(a_k)\leq C_{m,n,M,\phi}(1+|k|)^{-M}.
$$

Consequently continuity and periodicity of the [tempered distribution](../../../../../tempered-distribution.md) give

$$
\begin{aligned}
\langle u,\phi\rangle
&=\sum_k\langle u,\Psi(\cdot+2\pi k)\phi\rangle\\
&=\sum_k\langle u,\Psi(\cdot)\phi(\cdot-2\pi k)\rangle\\
&=\left\langle u,\Psi(\cdot)\sum_k\phi(\cdot-2\pi k)\right\rangle
=\boxed{\langle u,\Psi P\phi\rangle}.
\end{aligned}
$$

For the last interchange, all summands have the fixed [compact support](../../../../../compact-support.md) of $\Psi$ and their [derivatives](../../../../../derivative.md) decrease faster than any power of $|k|$. Hence the series converges in the [space of test functions](../../../../../space-of-test-functions.md), as well as in the [Schwartz space](../../../../../schwartz-space.md). Notice that $P\phi$ itself need not be a [Schwartz function](../../../../../schwartz-function.md); the factor $\Psi$ makes the pairing legitimate.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
