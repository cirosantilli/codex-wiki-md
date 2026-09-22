<h1 id="3k/solution">Solution</h1>

↑ **Parent:** [3K](../3k.md)

Let $\alpha$ be a primitive $n$th root of unity in an extension of $\mathbb F_q$, where $\gcd(n,q)=1$. A [BCH code](../../../../../bch-code.md) of length $n$, initial exponent $b$, and design distance $\delta$ is the cyclic code whose generator polynomial is the least common multiple over $\mathbb F_q$ of the minimal polynomials of

$$
\alpha^b,\alpha^{b+1},\ldots,\alpha^{b+\delta-2}.
$$

Thus every codeword polynomial $c(X)$ vanishes at these $\delta-1$ consecutive powers.

Suppose a nonzero codeword has weight $w<\delta$, with

$$
c(X)=\sum_{\ell=1}^w c_\ell X^{i_\ell},
$$

where the positions $i_\ell$ are distinct modulo $n$ and every $c_\ell$ is nonzero. The first $w$ root conditions give

$$
\sum_{\ell=1}^w c_\ell\alpha^{i_\ell(b+j)}=0,
\qquad j=0,1,\ldots,w-1.
$$

The coefficient matrix is a Vandermonde matrix in the distinct elements $\alpha^{i_1},\ldots,\alpha^{i_w}$, followed by multiplication of its columns by the nonzero factors $\alpha^{bi_\ell}$. Its determinant is therefore

$$
\left(\prod_{\ell=1}^w\alpha^{bi_\ell}\right)
\prod_{r<s}(\alpha^{i_s}-\alpha^{i_r})\ne0.
$$

Hence all $c_\ell$ would be zero, a contradiction. The minimum distance consequently satisfies $d\geq\delta$.

A code of minimum distance $d$ detects every pattern of at most $d-1$ errors and uniquely corrects every pattern of at most $\lfloor(d-1)/2\rfloor$ errors, because Hamming balls of that radius are disjoint. A BCH code of design distance $\delta$ is therefore guaranteed to detect $\delta-1$ errors and to correct

$$
\left\lfloor\frac{\delta-1}{2}\right\rfloor
$$

errors; its actual capabilities may be larger if $d>\delta$.

## ↑ Ancestors (10)

1. [3K](../3k.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
