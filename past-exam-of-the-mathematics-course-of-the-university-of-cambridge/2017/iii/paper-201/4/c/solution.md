<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Gaussian process](../../../../../../gaussian-process.md) assumption and the covariance formula give a centered Gaussian increment with [variance](../../../../../../variance-split.md)

$$
\mathbb E|\xi_t-\xi_s|^2=t+s-2\min(s,t)=|t-s|.
$$

For every finite $p>1$, a standard normal variable $Z$ therefore gives

$$
\|\xi_t-\xi_s\|_p=\|Z\|_p|t-s|^{1/2}.
$$

For any $0<\alpha<1/2$, choose $p>\max(2,(1/2-\alpha)^{-1})$. Then $\alpha<1/2-1/p$, so parts (a) and (b) give a [Hölder continuous function](../../../../../../holder-condition.md) of exponent $\alpha$ as an extension. To obtain one extension with every required exponent, take a countable sequence $\alpha_j\uparrow1/2$ and apply the construction with suitable $p_j$. Intersect the probability-one [events](../../../../../../event.md). Their continuous extensions agree on the dense set $D$ and hence agree everywhere. For each smaller exponent choose $j$ with $\alpha<\alpha_j$; since $|t-s|\leq1$, the bound with $\alpha_j$ also implies the bound with $\alpha$. Thus

$$
\boxed{X\in C^{0,\alpha}([0,1])\quad\text{almost surely, simultaneously for every }0<\alpha<\tfrac12.}
$$

The exponent constants may depend on $\alpha$ and the sample path. This proves [Brownian Hölder regularity](../../../../../../brownian-holder-regularity.md) for the continuous Gaussian extension without making an uncountable intersection of unrelated full-probability [events](../../../../../../event.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
