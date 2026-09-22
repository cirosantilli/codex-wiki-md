<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

For events with $P(B)>0$, the [conditional probability](../../../../../conditional-probability.md) is $P(A\mid B)=P(A\cap B)/P(B)$. Applying the definition in both orders gives [Bayes' theorem](../../../../../bayes-theorem.md):

$$
P(B\mid A)=\frac{P(A\cap B)}{P(A)}=P(A\mid B)\frac{P(B)}{P(A)}.
$$

Conditionally on $N=n$, independent fair tosses give a [binomial distribution](../../../../../binomial-distribution.md) for the head count, so $P(H=1\mid N=n)=n2^{-n}$. The joint [probability mass function](../../../../../probability-mass-function.md) is consequently

$$
P(N=n,H=1)=n4^{-n}.
$$

Use the [law of total probability](../../../../../law-of-total-probability.md) and the differentiated [geometric series](../../../../../geometric-series.md), $\sum_{n\geq1}nr^n=r/(1-r)^2$, to obtain $P(H=1)=4/9$. The [posterior coin count after exactly one head](../../../../../posterior-coin-count-after-exactly-one-head.md) is therefore

$$
\boxed{P(N=n\mid H=1)=\frac{9n}{4^{n+1}},\qquad n\geq1}.
$$

These [probabilities](../../../../../probability.md) sum to one by the same series identity. The conditioning weights possible coin counts by their likelihood of producing exactly one head.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
