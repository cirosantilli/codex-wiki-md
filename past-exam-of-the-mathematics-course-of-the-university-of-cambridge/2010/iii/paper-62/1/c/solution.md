<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $m$ and take $n\ge m$. On $[0,1]$, every factor $x-r/n$ and every factor $x$ has absolute value at most one. Replacing the factors successively and applying the [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\|f_{nm}-x^m\|_\infty\le\sum_{r=0}^{m-1}\frac rn=\frac{m(m-1)}{2n},\qquad |f_{nm}(1)-1|\le\frac{m(m-1)}{2n}.
$$

Using the [supremum norm](../../../../../../supremum-norm.md) contraction in (a) and the [Bernstein falling-factorial identity](../../../../../../bernstein-falling-factorial-identity.md) in (b),

$$
\begin{aligned}
\|B_n(x^m)-x^m\|_\infty
&\le\|B_n(x^m-f_{nm})\|_\infty+\|B_n(f_{nm})-x^m\|_\infty\\
&\le\|x^m-f_{nm}\|_\infty+|f_{nm}(1)-1|\le\frac{m(m-1)}n.
\end{aligned}
$$

For $m=0,1$, the [monomials](../../../../../../monomial.md) are reproduced exactly. For every fixed $m$, **$B_n(x^m)\to x^m$ uniformly on $[0,1]$**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
