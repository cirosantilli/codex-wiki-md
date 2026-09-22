<h1 id="o/o5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a fixed alternative $0<\lambda<\lambda_0$, the joint [likelihood ratio](../../../../../likelihood-ratio.md) is

$$
\frac{L(\lambda)}{L(\lambda_0)}
=\left(\frac\lambda{\lambda_0}\right)^n
\exp\left((\lambda_0-\lambda)\sum_i x_i\right).
$$

It is strictly increasing in $S=\sum_i x_i$. By the [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md), the most powerful level-$\alpha$ rejection region is therefore $S\geq c_\alpha$. Under the null, $S\sim\operatorname{Gamma}(n,\lambda_0)$ with the second parameter interpreted as a rate. Its continuous distribution gives

$$
\boxed{c_\alpha=q(1-\alpha;n,\lambda_0).}
$$

This threshold depends on the null and $\alpha$, but not on the particular smaller alternative $\lambda$. Thus the same test is most powerful for every $0<\lambda<\lambda_0$, making it [uniformly most powerful](../../../../../uniformly-most-powerful-test.md).

Under a true alternative $\lambda$, $S\sim\operatorname{Gamma}(n,\lambda)$, so its attained power is

$$
\boxed{Q(\lambda)=1-F(q(1-\alpha;n,\lambda_0);n,\lambda).}
$$

For each $\lambda<\lambda_0$, the [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) bounds the power of every other level-$\alpha$ test by this value. Hence the displayed function is not only an upper bound but the attainable power envelope on the specified alternative.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
