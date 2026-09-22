<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A syndrome determines a phase-error set only up to multiplication by $\overline X=Z_1\cdots Z_n$: an error of weight $w$ and its complement of weight $n-w$ have the same [error syndrome](../../../../../../error-syndrome.md). Their probability ratio is

$$
\frac{p^w(1-p)^{n-w}}{p^{n-w}(1-p)^w}
=\left(\frac p{1-p}\right)^{2w-n}.
$$

For $p<1/2$, [maximum likelihood](../../../../../../maximum-likelihood-estimation.md) therefore chooses the representative of smaller weight. This is exactly [majority-vote decoding of a repetition code](../../../../../../majority-vote-decoding-of-a-repetition-code.md): correction succeeds when fewer than half the qubits are flipped, with a random tie-break at $w=n/2$ when $n$ is even.

If $W\sim\operatorname{Bin}(n,p)$, then $\mathbb EW=np$ and $\operatorname{sd}(W)=\sqrt{np(1-p)}$. For every fixed $p<1/2$, the distance from the mean to the decision boundary in standard deviations is

$$
\frac{n/2-np}{\sqrt{np(1-p)}}
=\sqrt n\,\frac{1/2-p}{\sqrt{p(1-p)}}\longrightarrow\infty.
$$

Thus the logical failure probability $\Pr(W>n/2)$ tends to zero, in fact exponentially by a [Chernoff bound](../../../../../../chernoff-bound.md). At $p=1/2$ the two representatives are equiprobable and decoding cannot improve with $n$. Hence

$$
\boxed{p_c=\frac12.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
