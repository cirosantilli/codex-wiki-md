<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

Since $a_j=S_j-S_{j-1}$, shifting an index yields the [summation by parts](../../../../../abel-s-summation-formula.md) identity

$$
\begin{aligned}
\sum_{j=m}^n a_jb_j&=\sum_{j=m}^nS_jb_j-\sum_{j=m}^nS_{j-1}b_j\\
&=S_nb_n-S_{m-1}b_m+\sum_{j=m}^{n-1}S_j(b_j-b_{j+1}).
\end{aligned}
$$

The sum on the last line is empty when $m=n$, so the identity also covers that case.

**The series with a bounded monotone multiplier converges.** Here is a proof that also permits conditional convergence. Choose $M>0$ with $|b_j|\leq M$. The [Cauchy sequence](../../../../../cauchy-sequence.md) criterion for the convergent series $\sum a_j$ ensures that, for any $\eta>0$ and sufficiently large $m$, all the partial tails $T_j=\sum_{k=m}^j a_k$ satisfy $|T_j|<\eta$. Apply [summation by parts](../../../../../abel-s-summation-formula.md) to these partial tails:

$$
\sum_{j=m}^n a_jb_j=T_nb_n+\sum_{j=m}^{n-1}T_j(b_j-b_{j+1}).
$$

Since the multiplier is a [monotone sequence](../../../../../monotone-sequence.md), $\sum_{j=m}^{n-1}|b_j-b_{j+1}|=|b_m-b_n|$. Consequently

$$
\left|\sum_{j=m}^n a_jb_j\right|\leq\eta\bigl(|b_n|+|b_m-b_n|\bigr)\leq3M\eta.
$$

Taking $\eta=\varepsilon/(3M)$ proves that the weighted partial sums form a [Cauchy sequence](../../../../../cauchy-sequence.md), and hence converge. This is a special case of [bounded-variation multipliers of a convergent series](../../../../../bounded-variation-multipliers-of-a-convergent-series.md).

**The series $\sum n^{1/n}a_n$ also converges.** The multiplier need only be monotone eventually, since a finite initial segment cannot affect convergence. For $h(x)=\log x/x$,

$$
h'(x)=\frac{1-\log x}{x^2}<0\qquad(x\geq3).
$$

Thus $n^{1/n}=\exp(h(n))$ decreases for $n\geq3$; it is bounded and tends to $1$, because $\log n/n\to0$. Apply the proved multiplier result to the tail beginning at $3$. The fact that the first few values are not monotone causes no difficulty.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
