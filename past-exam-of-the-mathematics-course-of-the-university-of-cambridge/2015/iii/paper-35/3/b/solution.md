<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In [discrete back-calculation with endpoint cohorts](../../../../../../discrete-back-calculation-with-endpoint-cohorts.md), for equal-width intervals $I_k=[t_{k-1},t_k)$, write $\Delta=t_k-t_{k-1}$, $h_i$ for the expected infection count assigned to time $t_i$ under the end-of-interval approximation, and $\mu_k$ for the expected onset count in $I_k$. Define

$$
q_\ell=\Pr((\ell-1)\Delta\leq T<\ell\Delta),\qquad \ell=1,2,\ldots.
$$

An infection assigned to $t_i$ can first contribute to $I_{i+1}$, so **the discrete convolution with this timing convention is**

$$
\boxed{\mu_k\approx\sum_{i<k}h_iq_{k-i}.}
$$

The sum includes any infection cohorts before the observation window. With no infections before $t_0$ and cohorts beginning at $i=1$, it is $\sum_{i=1}^{k-1}$ and the first mean is zero in this endpoint approximation.

For unequal intervals use $q_{ik}=\Pr(t_{k-1}-t_i\leq T<t_k-t_i)$, truncating negative endpoints at zero, and $\mu_k\approx\sum_i h_iq_{ik}$. An alternative approximation assigning cohort $i$ to $t_{i-1}$ gives $\sum_{i\leq k}h_iq_{k-i+1}$. Both are legitimate discretisations; the subsequent solutions use the end-of-interval convention explicitly specified in part (d), so the index shift is essential.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
