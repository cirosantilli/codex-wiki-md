<h1 id="question-4/b/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

**The truncated [Fourier cosine series](../../../../../../../fourier-cosine-series.md) gives the better approximation on the closed interval**, in the senses of [uniform convergence](../../../../../../../uniform-convergence.md) and the asymptotic [L2 norm](../../../../../../../l2-norm.md) error. To make the comparison precise, let $C_N$ and $S_N$ retain the frequencies $1\leq n\leq N$, with the constant term also included in $C_N$.

The cosine [Fourier coefficients](../../../../../../../fourier-coefficient.md) are $O(n^{-2})$. In fact, [absolute convergence](../../../../../../../absolute-convergence.md) gives the uniform tail bound

$$
\sup_{0\leq x\leq\pi}|f(x)-C_N(x)|
\leq\frac4\pi\sum_{n>N}\frac1{n^2}
\leq\frac4{\pi N}\longrightarrow0.
$$

For the [Fourier sine series](../../../../../../../fourier-sine-series.md), every [Fourier partial sum](../../../../../../../fourier-partial-sum.md) satisfies $S_N(0)=S_N(\pi)=0$. Thus

$$
\boxed{\sup_{0\leq x\leq\pi}|f(x)-S_N(x)|\geq1+\pi},
$$

so there is no [uniform convergence](../../../../../../../uniform-convergence.md) to $f$ on the closed interval. Its [odd extension](../../../../../../../odd-extension.md) has [jump discontinuities](../../../../../../../jump-discontinuity.md), producing the [Gibbs phenomenon](../../../../../../../gibbs-phenomenon.md) near the endpoints; its [Fourier coefficients](../../../../../../../fourier-coefficient.md) decrease only like $1/n$.

The advantage persists in the [L2 norm](../../../../../../../l2-norm.md), which ignores individual endpoint values. By [Parseval's identity](../../../../../../../parseval-identity.md) and [Fourier orthogonality](../../../../../../../fourier-orthogonality.md),

$$
\|f-C_N\|_2^2=\frac\pi2\sum_{n>N}a_n^2=O(N^{-3}),\qquad
\|f-S_N\|_2^2=\frac\pi2\sum_{n>N}b_n^2=O(N^{-1}).
$$

The nonzero odd cosine coefficients and both parity classes of sine coefficients also give matching lower bounds of these orders by comparison with the corresponding [p-series](../../../../../../../p-series.md). Hence their [L2 norm](../../../../../../../l2-norm.md) errors decrease respectively like $N^{-3/2}$ and $N^{-1/2}$. This is a comparison of approximation quality in specified norms, not a claim that one finite sum has smaller error at every individual interior point.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [b](../../b.md)
3. [Question 4](../../../question-4.md)
4. [Mathematics V resit](../../../../mathematics-v-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
