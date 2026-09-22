<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For any fixed $p>1/4$, the alternative-to-null [likelihood ratio](../../../../../likelihood-ratio.md) is

$$
R_p(S)=\left(\frac{1-p}{3/4}\right)^5
\left(\frac{3p}{1-p}\right)^S,
$$

which is strictly increasing in $S$ for $1/4<p<1$. Consequently the [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) selects the same upper-tail ordering for every such [alternative hypothesis](../../../../../alternative-hypothesis.md). At the [null hypothesis](../../../../../null-hypothesis.md) value,

$$
\mathbb P_{1/4}(S\geq4)
=\binom54\left(\frac14\right)^4\frac34+\left(\frac14\right)^5
=\frac{15+1}{1024}=\frac1{64}.
$$

Therefore

$$
\boxed{\text{reject }H_0\text{ exactly when }S\geq4}
$$

is a [uniformly most powerful test](../../../../../uniformly-most-powerful-test.md) of the required exact [test size](../../../../../size-of-a-statistical-test.md). Its [power function](../../../../../power-function-of-a-statistical-test.md) is $5p^4(1-p)+p^5=5p^4-4p^5$. At $p=1$ its [statistical power](../../../../../statistical-power.md) is one, so including that boundary alternative preserves the conclusion.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
