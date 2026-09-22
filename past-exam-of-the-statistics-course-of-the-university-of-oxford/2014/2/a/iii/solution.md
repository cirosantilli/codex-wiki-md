<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $T=\sum_iX_i$. For interior parameters $0<\theta_0<\theta_1<1$, the alternative-to-null [likelihood ratio](../../../../../likelihood-ratio.md) is

$$
\frac{L(\theta_1)}{L(\theta_0)}
=\left(\frac{1-\theta_1}{1-\theta_0}\right)^n
\left(\frac{\theta_1(1-\theta_0)}{\theta_0(1-\theta_1)}\right)^T.
$$

The second base is greater than one, so this is strictly increasing in $T$. The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) therefore gives **an upper-tail rejection rule**. Under the [null hypothesis](../../../../../null-hypothesis.md), $T\sim\operatorname{Bin}(n,\theta_0)$, and an ordinary conservative threshold can be chosen as

$$
C=\{x:T(x)\geq c_\alpha\},\qquad
\Pr_{\theta_0}(T\geq c_\alpha)\leq\alpha.
$$

There is an important discrete qualification: an integer cutoff need not have [test size](../../../../../size-of-a-statistical-test.md) exactly $\alpha$. To obtain exact size, choose an integer $b$ with $\Pr_0(T>b)\leq\alpha\leq\Pr_0(T\geq b)$, reject certainly when $T>b$, and at $T=b$ reject with probability

$$
\boxed{\gamma=\frac{\alpha-\Pr_0(T>b)}{\Pr_0(T=b)}.}
$$

This [randomized statistical test](../../../../../randomized-statistical-test.md) is a [most powerful test](../../../../../most-powerful-test.md) at exact size $\alpha$; when a binomial upper tail equals $\alpha$, no randomization is needed and the stated region is literal. Otherwise the unrandomized upper-tail region has size at most $\alpha$, and the exact-size result includes the boundary randomization. Endpoint parameter cases retain the same upper-tail ordering by taking limits, with ties resolved on the null-supported outcomes.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
