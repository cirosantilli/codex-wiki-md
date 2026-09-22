<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

The Möbius [function](../../../../../function-split.md) is

$$
\mu(n)=\begin{cases}
1,&n=1,\\
(-1)^r,&n\text{ is a product of }r\text{ distinct primes},\\
0,&n\text{ is divisible by a square}.
\end{cases}
$$

Möbius inversion says that

$$
g(n)=\sum_{d\mid n}f(d)
\quad\Longleftrightarrow\quad
f(n)=\sum_{d\mid n}\mu(d)g(n/d).
$$

Now

$$
\sum_{d^k\mid n}\mu(d)
$$

is the sum of $(-1)^{|S|}$ over subsets of the primes whose $k$th powers divide $n$. It is one if there are no such primes and zero otherwise, proving the power-free criterion.

Let

$$
c_n=\sum_{\substack{1\leq d\leq n\\(d,n)=1}}e^{2\pi i d/n}.
$$

Grouping all $n$th roots of unity by their exact order gives

$$
\sum_{m\mid n}c_m=\begin{cases}1,&n=1,\\0,&n>1.
\end{cases}
$$

Möbius inversion therefore yields $c_n=\mu(n)$.

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
