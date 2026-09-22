<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

A [simple hypothesis](../../../../../simple-hypothesis.md) specifies a single probability distribution. For a test with rejection region $R$, its [size of a statistical test](../../../../../size-of-a-statistical-test.md) is the rejection probability under the simple [null hypothesis](../../../../../null-hypothesis.md), while its [statistical power](../../../../../statistical-power.md) against the simple alternative is the rejection probability under that alternative. The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) states that among tests of size at most $\alpha$, a test rejecting for the largest values of the [likelihood ratio](../../../../../likelihood-ratio.md) $f_1/f_0$ has greatest power, with boundary randomization if needed.

Here

$$
\frac{f_1(x)}{f_0(x)}=\frac32(1-x^2),
$$

which decreases with $|x|$. The best test therefore rejects for $|X|\leq c$. Under $H_0$, $\mathbb P_0(|X|\leq c)=c$, so size $0.05$ requires $c=0.05=1/20$. Its power is

$$
\boxed{\mathbb P_1(|X|\leq1/20)
=\int_{-1/20}^{1/20}\frac34(1-x^2)\,dx
=\frac{1199}{16000}=0.0749375.}
$$

**Thus reject $H_0$ exactly when $|X|\leq0.05$.**

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
