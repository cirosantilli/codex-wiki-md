<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

For a [binary linear code](../../../../../binary-linear-code.md) $C\leq\mathbb F_2^n$, its rank is its [dimension of a vector space](../../../../../dimension-vector-space.md) $r$. Use the [weight enumerator](../../../../../weight-enumerator.md) convention

$$
W_C(s,t)=\sum_{c\in C}s^{w(c)}t^{n-w(c)},
$$

where $w(c)$ is the [Hamming weight](../../../../../hamming-weight.md). This convention is essential here: $W_C(1,0)$ counts words of weight $n$, rather than zero words. There are $2^r$ codewords, so $\boxed{W_C(1,1)=2^r}$.

There is only one binary word of weight $n$, namely $\mathbf1=(1,\ldots,1)$. Thus $W_C(1,0)=1$ precisely when $\mathbf1\in C$. If this holds, the [linear map](../../../../../linear-map.md) $c\mapsto c+\mathbf1$ is a bijection of $C$ and replaces weight $w$ by $n-w$; hence $W_C(s,t)=W_C(t,s)$. Conversely this symmetry gives $W_C(1,0)=W_C(0,1)=1$, because the zero word is the unique word of weight zero.

The [repetition code](../../../../../repetition-code.md) consists of $\mathbf0,\mathbf1$, giving

$$
\boxed{W_{\rm rep}(s,t)=t^n+s^n.}
$$

The [single parity-check code](../../../../../single-parity-check-code.md) consists of all words of even weight. Exactly $\binom nj$ words have weight $j$, so the [binomial theorem](../../../../../binomial-theorem.md) gives

$$
\boxed{W_{\rm parity}(s,t)=\sum_{j\text{ even}}\binom nj s^jt^{n-j}=\frac{(t+s)^n+(t-s)^n}{2}.}
$$

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
