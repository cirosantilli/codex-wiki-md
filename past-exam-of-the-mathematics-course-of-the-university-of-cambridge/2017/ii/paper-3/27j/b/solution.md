<h1 id="27j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The difference of the terminal [European call option](../../../../../../european-call-option.md) and [European put option](../../../../../../european-put-option.md) payoffs is $S_T^1-K$. Replicating that difference by one share and a borrowing position gives conditional [put-call parity](../../../../../../put-call-parity.md)

$$
 c_{t_0}-p_{t_0}=S_{t_0}^1-K(1+r)^{t_0-T}.
$$

Thus the call is more valuable exactly when the right side is positive. With a put selected at equality, the [chooser option](../../../../../../chooser-option.md) payoff is

$$
\boxed{H=(S_T^1-K)^+\mathbf1_{\{S_{t_0}^1>K(1+r)^{t_0-T}\}}
 +(K-S_T^1)^+\mathbf1_{\{S_{t_0}^1\leq K(1+r)^{t_0-T}\}}.}
$$

At equality both choices have the same price, even though their eventual payoffs can differ. [Put-call parity](../../../../../../put-call-parity.md) assumes no dividends or other intermediate stock cash flows, as in the stated asset-price model.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [27J](../../27j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
