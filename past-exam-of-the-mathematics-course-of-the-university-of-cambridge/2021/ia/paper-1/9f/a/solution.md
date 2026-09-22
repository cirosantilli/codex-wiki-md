<h1 id="9f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) states that if $f:[a,b]\to\mathbb R$ is continuous and $y$ lies between $f(a)$ and $f(b)$, then $f(c)=y$ for some $c\in[a,b]$.

Let $x_1<x_2<x_3$. If, for example, $f(x_2)$ exceeded both $f(x_1)$ and $f(x_3)$, choose $y$ strictly between $f(x_2)$ and $\max\{f(x_1),f(x_3)\}$. Applying the theorem on both $[x_1,x_2]$ and $[x_2,x_3]$ would give two distinct preimages of $y$, contradicting injectivity. The analogous argument excludes $f(x_2)$ below both endpoint values. Since the three values are distinct,

$$
\boxed{
f(x_1)<f(x_2)<f(x_3)
\quad\text{or}\quad
f(x_1)>f(x_2)>f(x_3)}.
$$

Fix $a<b$. If $f(a)<f(b)$, applying the displayed betweenness property to triples containing $a,b$ forces the same increasing order for every pair $x<y$; an order reversal would create a triple whose middle value is not between the other two. Thus $f$ is strictly increasing. If $f(a)>f(b)$, the same argument shows that it is strictly decreasing. This proves that every [continuous bijection of the real line is monotone](../../../../../../continuous-bijection-of-the-real-line-is-monotone.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
