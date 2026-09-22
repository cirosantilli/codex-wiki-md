<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $u\in C_c^\infty(\mathbb R^d)$, the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) along the $j$th coordinate line gives

$$
|u(x)|\leq\int_{\mathbb R}|\partial_ju(x_1,\ldots,x_{j-1},t,x_{j+1},\ldots,x_d)|\,dt.
$$

Take $f=|u|$ and $s_j=|\partial_ju|$ in the introductory result. It follows that

$$
\boxed{\|u\|_{d/(d-1)}\leq\prod_{j=1}^d\|\partial_ju\|_1^{1/d}\leq\frac1d\sum_{j=1}^d\|\partial_ju\|_1}.
$$

The last step is the [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md). This bounds the target norm by the [first-order Sobolev space](../../../../../../first-order-sobolev-space.md) norm. Approximate any $u\in W^{1,1}(\mathbb R^d)=L_1^1(\mathbb R^d)$ by compactly supported smooth functions, using cutoffs and [mollification](../../../../../../mollification.md) as in Question 4. The estimate applied to differences gives convergence in $L^{d/(d-1)}$, and subsequences of the simultaneous $L^1$ and target-norm convergence identify the two limits almost everywhere. **Thus $W^{1,1}$ embeds continuously into $L^{d/(d-1)}$.** The coordinate-derivative product bound also passes to the limit. For $d=1$, the line argument instead gives $\|u\|_\infty\leq\|u'\|_1$ and the embedding into $L^\infty$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
