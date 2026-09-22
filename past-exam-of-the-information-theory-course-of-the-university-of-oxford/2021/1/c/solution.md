<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [maximum entropy distribution on the nonnegative integers](../../../../maximum-entropy-distribution-on-the-nonnegative-integers.md), use the [geometric distribution](../../../../geometric-distribution.md) counting failures before the first success. Write $r=a/(a+1)$ and define

$$
\boxed{g_i=(1-r)r^i=\frac1{a+1}\left(\frac a{a+1}\right)^i,\qquad i=0,1,\ldots.}
$$

The [geometric series](../../../../geometric-series.md) gives $\sum_i g_i=1$. [Termwise differentiation of a power series](../../../../termwise-differentiation-of-a-power-series.md) applied to that [geometric series](../../../../geometric-series.md) for $0<r<1$ gives $\sum_iir^i=r/(1-r)^2$, hence $\sum_iig_i=r/(1-r)=a$.

For any competing [probability mass function](../../../../probability-mass-function.md) $p$ of mean $a$, its [cross-entropy](../../../../cross-entropy.md) against $g$ is

$$
-\sum_{i\geq0}p_i\log_2g_i
=\log_2(a+1)+a\log_2\frac{a+1}{a}
=(a+1)\log_2(a+1)-a\log_2a.
$$

This is finite. The fact that [finite cross entropy bounds countable information entropy](../../../../finite-cross-entropy-bounds-countable-information-entropy.md) must be justified without assuming in advance that $H(p)$ is finite. Use $\ln u\leq u-1$ with $u=g_i/p_i$ when $p_i>0$. Including zero terms by their limiting convention yields, for every finite $N$,

$$
\sum_{i=0}^N-p_i\log_2p_i\leq\sum_{i=0}^N-p_i\log_2g_i+\frac1{\ln2}\sum_{i=0}^N(g_i-p_i).
$$

Let $N\to\infty$. The [information entropy](../../../../information-entropy-split.md) partial sums increase, the [cross-entropy](../../../../cross-entropy.md) partial sums converge to the finite value above, and the final mass difference tends to zero. This proves finiteness and the upper bound. We may now write

$$
D(p\|g)=H(g)-H(p)\geq0.
$$

[Relative entropy nonnegativity](../../../../relative-entropy-nonnegativity.md) has equality exactly when $p=g$. Therefore the displayed geometric [probability mass function](../../../../probability-mass-function.md) is the **unique maximizer**, and

$$
\boxed{H_{\max}=(a+1)\log_2(a+1)-a\log_2a\ \text{bits}.}
$$

The mean constraint is essential: without it, [uniform distributions](../../../../continuous-uniform-distribution.md) on longer initial intervals have unbounded [information entropy](../../../../information-entropy-split.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
