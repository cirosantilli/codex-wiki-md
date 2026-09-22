<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the positive-integer convention for the [geometric distribution](../../../../../../geometric-distribution.md):

$$
\mathbb P(K=k)=p(1-p)^{k-1},\quad k\geq1,\qquad\mathbb EK=1/p.
$$

Conditional on $K=k$, [independence](../../../../../../independent-random-variables.md) gives $\mathbb E[S\mid K=k]=k/\lambda$. Taking [expectations](../../../../../../expected-value.md) gives

$$
\boxed{\mathbb ES=\frac1{p\lambda}.}
$$

This is the convention required below because a chain starting at $i$ makes at least one visit to $i$. If instead $K$ counts failures on $\{0,1,\ldots\}$, its mean is $(1-p)/p$, and the corresponding answer for that different random sum is $(1-p)/(p\lambda)$.

For the chain of part (b), let $K_i$ count visits to $i$, including the initial visit, before absorption. After a departure to $i-1$, [gambler's ruin](../../../../../../gambler-s-ruin.md) on $\{0,\ldots,i\}$ gives probability $1/i$ of reaching zero before returning to $i$. After a departure to $i+1$, the analogous probability of reaching $N$ before returning is $1/(N-i)$. The departure is equally likely in either direction, so the probability of absorption before a return is

$$
p_i=\frac12\left(\frac1i+\frac1{N-i}\right)
=\frac{N}{2i(N-i)}.
$$

At every return to $i$, the [Strong Markov property](../../../../../../strong-markov-property.md) resets these alternatives. Hence the [geometric return count before absorption](../../../../../../geometric-return-count-before-absorption.md) gives $K_i\sim\operatorname{Geom}(p_i)$ on positive integers. One may construct the chain from its embedded jump chain and a separate sequence of fresh [independent](../../../../../../independent-random-variables.md) exponential clocks. Then its successive [holding times](../../../../../../holding-time.md) at $i$ are [independent and identically distributed](../../../../../../independent-and-identically-distributed-random-variables.md) rate-$\lambda_i$ [exponential random variables](../../../../../../exponential-distribution.md), independently of $K_i$, and

$$
I=\sum_{j=1}^{K_i}E_j^{(i)}.
$$

Using the first calculation gives the [occupation time at an interior state of a variable-rate symmetric walk](../../../../../../occupation-time-at-an-interior-state-of-a-variable-rate-symmetric-walk.md):

$$
\boxed{\mathbb E_iI=\frac1{p_i\lambda_i}
=\frac{2i(N-i)}{N\lambda_i}.}
$$

For $N=2,i=1$, $p_i=1$ and the only visit is the initial one; the degenerate positive-integer [geometric distribution](../../../../../../geometric-distribution.md) at one handles this case. Other states' rates affect the time of each excursion, but not its probability of return, which explains why only $\lambda_i$ appears in this [expectation](../../../../../../expected-value.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
