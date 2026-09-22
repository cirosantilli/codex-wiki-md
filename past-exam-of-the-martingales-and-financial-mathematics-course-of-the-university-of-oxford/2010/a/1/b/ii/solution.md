<h1 id="a/1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The Cauchy assumption lets us choose $n_k$ recursively, increasing strictly, so that $\mu(|f_n-f_m|>2^{-k})<2^{-k}$ for all $m,n\geq n_k$. In particular the measurable events

$$
E_k=\{|f_{n_{k+1}}-f_{n_k}|>2^{-k}\}
$$

have summable measures. The measure of $\bigcup_{k\geq K}E_k$ is at most $\sum_{k\geq K}2^{-k}\to0$, so $\limsup E_k$ is a null set. Outside it, the successive differences are eventually bounded by a summable geometric series. Hence $f_{n_k}$ is pointwise Cauchy and has a finite real limit.

Define $f$ to be that limit wherever the sequence converges, and zero elsewhere. The convergence set is measurable by the countable Cauchy criterion, and the limit is measurable as a limit of measurable functions on that set. Thus there is no need to assume the measure is complete. Part (a)(ii), or the corresponding finite-measure implication, gives $f_{n_k}\to f$ in measure.

For the full sequence use

$$
\mu(|f_n-f|>\varepsilon)\leq
\mu(|f_n-f_{n_k}|>\varepsilon/2)+\mu(|f_{n_k}-f|>\varepsilon/2).
$$

Choose a sufficiently late subsequence index so the second term is small; the Cauchy property then bounds the first uniformly for all large $n$. Therefore **$f_n\to f$ in measure**. This proves [completeness of convergence in measure on a finite measure space](../../../../../../completeness-of-convergence-in-measure-on-a-finite-measure-space.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
