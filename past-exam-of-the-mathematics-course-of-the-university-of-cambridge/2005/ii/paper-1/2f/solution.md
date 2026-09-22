<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

The [hyperbolic cosine](../../../../../hyperbolic-cosine.md) has the absolutely convergent expansion $\cosh(1/2)=\sum_{k\ge0}1/[4^k(2k)!]$. Suppose its value were a rational $a/b$, with $b>0$. For sufficiently large $N$, $b\mid(2N)!$. Multiplying by $4^N(2N)!$ makes the assumed value an integer, and every term of the partial sum through $k=N$ is also an integer. Their difference is the positive remainder

$$
R_N=\sum_{j=1}^\infty\frac{(2N)!}{4^j(2N+2j)!}.
$$

Let $q=[4(2N+1)(2N+2)]^{-1}$. Every new pair of factorial factors is at least $(2N+1)(2N+2)$, so $0<R_N\le\sum_{j\ge1}q^j=q/(1-q)<1$ for $N\ge1$. No integer lies strictly between zero and one. This contradiction proves **$\cosh(1/2)$ is irrational**. The argument uses a finite integer partial sum and a controlled tail; it does not infer irrationality merely from an infinite expansion.

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
