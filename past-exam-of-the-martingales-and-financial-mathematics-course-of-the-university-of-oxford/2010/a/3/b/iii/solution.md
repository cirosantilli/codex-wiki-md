<h1 id="a/3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Since $X_n>0$, the pointwise inequality

$$
\mathbf1_{\{X_\infty=0\}}\leq\frac{(X_n-X_\infty)^2}{X_n^2}
$$

holds: on that event both sides equal one, and elsewhere the left side is zero. Take [conditional expectation](../../../../../../conditional-expectation.md) and pull out the positive $\mathcal F_n$-measurable denominator to obtain the requested bound. The supplied variance estimate improves it to

$$
0\leq\mathbb P(X_\infty=0\mid\mathcal F_n)
\leq\frac1{(m+n)X_n}=\frac1{B_n}\longrightarrow0
$$

almost surely, by part (ii). These conditional probabilities are bounded by one. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) and [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) give

$$
\boxed{\mathbb P(X_\infty=0)=\lim_n\mathbb E[\mathbb P(X_\infty=0\mid\mathcal F_n)]
=\mathbb E[\lim_n\mathbb P(X_\infty=0\mid\mathcal F_n)]=0.}
$$

This proves [Positivity of the limiting Pólya urn proportion](../../../../../../positivity-of-the-limiting-polya-urn-proportion.md) without needing its explicit beta distribution.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
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
