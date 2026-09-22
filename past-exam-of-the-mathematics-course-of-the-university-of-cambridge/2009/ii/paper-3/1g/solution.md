<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

For every [prime number](../../../../../prime-number.md) $p$ with $n<p\le2n$, the numerator $(2n)!$ contains one factor $p$, whereas neither copy of $n!$ contains one. Consequently the product of these [prime numbers](../../../../../prime-number.md) divides the [binomial coefficient](../../../../../binomial-coefficient.md) $\binom{2n}{n}$. Since this [binomial coefficient](../../../../../binomial-coefficient.md) is one positive summand of $\sum_{j=0}^{2n}\binom{2n}{j}=2^{2n}$, and other summands are positive,

$$
\theta(2n)-\theta(n)=\log\prod_{n<p\le2n}p\le\log\binom{2n}{n}<2n\log2.
$$

For $x\ge2$, choose $k$ with $2^{k-1}<x\le2^k$. The [Chebyshev function](../../../../../chebyshev-function.md) is increasing, so telescoping gives

$$
\theta(x)\le\theta(2^k)=\sum_{j=1}^k\bigl(\theta(2^j)-\theta(2^{j-1})\bigr)<(2^{k+1}-2)\log2<4x\log2.
$$

For $x=1$ the inequality follows from $\theta(1)=0$. Thus $\boxed{\theta(x)<4(\log2)x}$ throughout the stated range.

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
