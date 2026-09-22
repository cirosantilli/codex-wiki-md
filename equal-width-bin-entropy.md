# Equal-width bin entropy

↑ **Parent:** [Differential entropy](differential-entropy.md)

Partition $(0,1)$ into $n$ bins of width $\delta=1/n$, and let the [discrete random variable](discrete-random-variable.md) $Q_n$ record the bin containing $X$. This is a [quantization](quantization-signal-processing.md) of $X$. Its [probability mass function](probability-mass-function.md) is

$$
p_j=\int_{j/n}^{(j+1)/n}f(x)\,dx,\qquad 0\leq j<n,
$$

and its discrete [information entropy](information-entropy-split.md) is $H_e(Q_n)=-\sum_jp_j\ln p_j$. Let $\bar f_j=p_j/\delta$ be the average [probability density](probability-density.md) within bin $j$. Rearrangement gives the exact finite-bin identity

$$
H_e(Q_n)+\ln\delta=-\sum_j\delta\bar f_j\ln\bar f_j.
$$

For a [continuous](continuous-function.md) [probability density](probability-density.md) on $[0,1]$, [uniform continuity](uniform-continuity.md) makes the bin averages converge uniformly to the density. Since $t\ln t$ is [continuous](continuous-function.md) at zero with the stated convention, the right-hand side converges to $h_e(X)$. Thus the increasing resolution cost is $\ln n$; [differential entropy](differential-entropy.md) is the remaining offset, rather than the entire discrete encoding cost.

For a [continuous uniform distribution](continuous-uniform-distribution.md), every bin has [probability](probability.md) $1/n$, and $H_e(Q_n)=\ln n$ exactly. For the [continuous uniform distribution](continuous-uniform-distribution.md)'s squared transformation above, the exact bin probabilities are

$$
p_j=\sqrt{\frac{j+1}{n}}-\sqrt{\frac jn}.
$$

The diagram computes these masses directly, including the bin next to the integrable singularity. It compares their corrected [information entropy](information-entropy-split.md) with the analytic [differential entropy](differential-entropy.md) $\ln2-1$.

<a id="image-removing-the-bin-resolution-cost-reveals-differential-entropy"></a>
![](differential-entropy-fine-bin-resolution.png)

**[Figure 4](#image-removing-the-bin-resolution-cost-reveals-differential-entropy). Removing the bin-resolution cost reveals differential entropy**. The left plot shows discrete [information entropy](information-entropy-split.md) increasing with the number of equal-width bins. The right subtracts $\ln n$ and compares with the exact [differential entropy](differential-entropy.md) of a uniform input and its squared transformation. Every plotted point comes from the stated exact [probability mass functions](probability-mass-function.md); no observations are fitted.

## ↑ Ancestors (7)

1. [Differential entropy](differential-entropy.md)
2. [Information entropy](information-entropy-split.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Differential entropy](differential-entropy.md)
