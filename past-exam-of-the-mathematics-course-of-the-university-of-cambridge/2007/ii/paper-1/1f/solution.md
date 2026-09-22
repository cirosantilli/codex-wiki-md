<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

The [Prime number theorem](../../../../../prime-number-theorem.md) says $\pi(x)\sim x/\log x$ as $x\to\infty$. [Bertrand's postulate](../../../../../bertrand-s-postulate.md) says that for every integer $n\ge2$ there is a [prime number](../../../../../prime-number.md) strictly between $n$ and $2n$.

To count [S-smooth numbers](../../../../../s-smooth-number.md), split each prime exponent into its parity and an even part. This gives the unique expression $n=ab^2$, where $a$ is a [squarefree](../../../../../squarefree-integer.md) product of a subset of $S$. There are $2^{|S|}$ possible $a$, while $b\le\sqrt x$ whenever $n\le x$. The [squarefree-part bound for smooth numbers](../../../../../squarefree-part-bound-for-smooth-numbers.md) therefore gives $f_S(x)\le2^{|S|}\lfloor\sqrt x\rfloor\le2^{|S|}\sqrt x$.

For an integer $x\ge1$, take $S$ to be all [prime numbers](../../../../../prime-number.md) at most $x$. Every positive integer at most $x$ is then [S-smooth](../../../../../s-smooth-number.md), so $x\le2^{\pi(x)}\sqrt x$. Taking [logarithms](../../../../../logarithm.md) yields

$$
\boxed{\pi(x)\ge\frac{\log x}{2\log2}.}
$$

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
