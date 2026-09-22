<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $S=\sum_iX_i$, which has a [binomial distribution](../../../../../binomial-distribution.md) with parameters $(n,p)$. For $0<p_1<1/2$, the alternative-to-null [likelihood ratio](../../../../../likelihood-ratio.md) of the independent [Bernoulli trials](../../../../../bernoulli-trial.md) is

$$
R(S)=\frac{p_1^S(1-p_1)^{n-S}}{(1/2)^n}
=[2(1-p_1)]^n\left(\frac{p_1}{1-p_1}\right)^S.
$$

Since $p_1/(1-p_1)<1$, this is strictly decreasing in $S$. A threshold on large $R$ is therefore a lower-tail [likelihood-ratio test](../../../../../likelihood-ratio-test.md), and a threshold between $R(2)$ and $R(1)$ gives the stated [critical region](../../../../../rejection-region.md) $S<2$. The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) also proves it is a [most powerful test](../../../../../most-powerful-test.md) at its attained [test size](../../../../../size-of-a-statistical-test.md).

Using the [binomial probability mass](../../../../../binomial-probability-mass.md), its [test size](../../../../../size-of-a-statistical-test.md) and [statistical power](../../../../../statistical-power.md) are respectively

$$
\boxed{\mathbb P_{1/2}(S<2)=\frac{1+n}{2^n}},\qquad
\boxed{\mathbb P_{p_1}(S<2)=(1-p_1)^n+np_1(1-p_1)^{n-1}}.
$$

The associated [power function](../../../../../power-function-of-a-statistical-test.md) is $\pi(p)=(1-p)^n+np(1-p)^{n-1}$. These formulas hold for positive integer $n$; when $n=1$ the test always rejects and has size one. If the boundary value $p_1=0$ is admitted, all alternative [probability](../../../../../probability.md) is at $S=0$; the same test still has [statistical power](../../../../../statistical-power.md) one and can be represented using a threshold with ties in the [likelihood ratio](../../../../../likelihood-ratio.md).

## ↑ Ancestors (13)

1. [I](../i.md)
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
