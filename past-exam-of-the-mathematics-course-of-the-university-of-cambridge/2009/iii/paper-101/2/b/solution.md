<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every $X_n$ is integrable: induction gives $|X_n|\leq a^n|x|+\sum_{j=0}^{n-1}a^j$. Since the innovation has [expectation](../../../../../../expected-value.md) zero, the recursion implies

$$
\mathbb EX_{n+1}=a\mathbb EX_n+\mathbb E\theta_{n+1}=a\mathbb EX_n.
$$

Starting from $\mathbb EX_0=x$, induction therefore gives

$$
\boxed{\mathbb EX_n=a^nx\qquad(n\geq0).}
$$

This holds for every $a>0$, including $a=1$. The [independence](../../../../../../independent-random-variables.md) of the signs also identifies this as an [autoregressive process of order one](../../../../../../autoregressive-process-of-order-one.md), although zero mean of each sign already suffices for the displayed [expectation](../../../../../../expected-value.md) recursion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
