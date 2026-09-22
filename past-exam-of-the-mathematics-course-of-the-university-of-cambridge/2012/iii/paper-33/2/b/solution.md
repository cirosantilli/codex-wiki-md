<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the unit-rate [exponential distribution](../../../../../../exponential-distribution.md), direct integration gives

$$
\mathbb E e^{\theta Y_1}=\frac1{1-\theta}\quad(\theta<1),\qquad \Lambda(\theta)=-\log(1-\theta).
$$

For $x>0$, maximizing $\theta x+\log(1-\theta)$ gives $\theta=1-1/x$, and therefore $I(x)=x-1-\log x$. For $x\leq0$ the supremum is infinite, as seen by taking $\theta\to-\infty$.

For $a>1$, $I$ is increasing on $[a,\infty)$, and its continuity gives $\inf_{[a,\infty)}I=\inf_{(a,\infty)}I=I(a)$. The closed-set upper bound and open-set lower bound of the [Cramér theorem](../../../../../../cramer-s-theorem.md) squeeze the desired limit to $-I(a)$. For $a=1$, both infima are $0$, because $I(1)=0$ and $I(x)\to0$ as $x\downarrow1$. For $0\leq a<1$, the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $S_n/n\to1$ almost surely, so the tail [probability](../../../../../../probability.md) tends to $1$; at $a=0$ it is identically $1$.

Consequently the [exponential sample-mean upper-tail rate](../../../../../../exponential-sample-mean-upper-tail-rate.md) is

$$
\boxed{\lim_{n\to\infty}\frac1n\log\mathbb P(S_n\geq na)=\begin{cases}0,&0\leq a\leq1,\\-(a-1-\log a),&a>1.\end{cases}}
$$

The threshold case uses the rate-function lower bound on the open half-line, rather than applying the law of large numbers at equality.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
