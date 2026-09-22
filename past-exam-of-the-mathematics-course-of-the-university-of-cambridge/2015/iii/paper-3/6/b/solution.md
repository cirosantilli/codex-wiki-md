<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Number the vertices consecutively along the underlying chain. Orientation does not affect the quadratic [Tits form of a quiver](../../../../../../tits-form-of-a-quiver.md):

$$
q_Q(\mathbf n)=\sum_{i=1}^m n_i^2-\sum_{i=1}^{m-1}n_in_{i+1}=\frac12\sum_{i=0}^m(n_{i+1}-n_i)^2,\qquad n_0=n_{m+1}=0.
$$

If $\mathbf n$ has nonnegative integer coordinates and $q_Q(\mathbf n)=1$, the sum of integer squares on the right is $2$. There are therefore exactly two nonzero consecutive differences, each of absolute value one. Their sum is zero, so one is $+1$ and the other $-1$. Nonnegativity forces the $+1$ to occur first. Thus the [positive roots of type A](../../../../../../positive-roots-of-type-a.md) are exactly the vectors with **a single nonempty interval of ones and zeros elsewhere**.

There is one such vector for every pair of endpoints $1\leq a\leq b\leq m$, giving

$$
\boxed{\#\{\text{positive roots of type }A_m\}=\frac{m(m+1)}2.}
$$

For $A_3$, the full list is

$$
\boxed{(1,0,0),\ (0,1,0),\ (0,0,1),\ (1,1,0),\ (0,1,1),\ (1,1,1).}
$$

The difference-of-coordinates proof includes $m=1$ and is independent of the chosen arrow orientation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
