<h1 id="o/o5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a fixed $\lambda<\lambda_0$, the [likelihood ratio](../../../../../likelihood-ratio.md) against the null is

$$
\frac{L(\lambda)}{L(\lambda_0)}=\left(\frac\lambda{\lambda_0}\right)^n\exp\left((\lambda_0-\lambda)\sum_i x_i\right),
$$

strictly increasing in $S=\sum_i x_i$. The Neyman–Pearson [critical region](../../../../../rejection-region.md) is therefore an upper tail in $S$, and its null threshold depends only on the desired size, not on which $\lambda<\lambda_0$ was chosen. Thus the same test is uniformly most powerful for the entire one-sided alternative.

Under the null $S\sim\operatorname{Gamma}(n,\lambda_0)$ with the second parameter interpreted as rate. Its [continuous](../../../../../continuous-function.md) distribution permits the exact threshold

$$
\boxed{c_\alpha=q(1-\alpha;n,\lambda_0).}
$$

Under any fixed alternative its rejection probability is $\boxed{Q(\lambda)=1-F(c_\alpha;n,\lambda)}$. Applying the lemma separately to each such $\lambda$ shows that every level-$\alpha$ test has [power](../../../../../power-function-of-a-statistical-test.md) at most this value there. The constructed test attains the bound for all $\lambda<\lambda_0$ simultaneously.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
