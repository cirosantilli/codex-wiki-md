<h1 id="22f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each positive integer $i$, apply the [Stone-Weierstrass theorem](../../../../../../stone-weierstrass-theorem.md) on the closed ball $\overline B(0,i)$ to choose a polynomial $p_i$ in $n$ variables satisfying

$$
\sup_{|x|\leq i}|p_i(x)-f(x)|<\frac1i.
$$

Every compact $B\subset\mathbb R^n$ lies in some such ball, so the same estimate for all sufficiently large $i$ proves that $p_i|_B\to f|_B$ uniformly.

Now suppose instead that $p_i\to f$ uniformly on all of $\mathbb R^n$. For sufficiently large $i,j$, the polynomial $p_i-p_j$ is bounded on $\mathbb R^n$, and every nonconstant real polynomial is unbounded along a suitable line. Hence $p_i-p_j$ is constant. A tail of the sequence is therefore one fixed polynomial plus a uniformly convergent sequence of constants, and its limit is a polynomial. The converse is immediate from the constant sequence. Thus

$$
\boxed{\ f\text{ is a globally uniform limit of polynomials}\iff f\text{ is a polynomial}.\ }
$$

This is the [globally uniform limit of real polynomials](../../../../../../globally-uniform-limit-of-real-polynomials.md) criterion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22F](../../22f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
