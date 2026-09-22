<h1 id="9f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed real $x$, define $u_0=x$ and $u_n=\sin(0.99u_{n-1})$. This makes $u_n$ exactly the summand containing $n$ nested sines. The elementary inequality $|\sin t|\le|t|$ gives inductively

$$
|u_n|\le0.99|u_{n-1}|\le0.99^n|x|.
$$

The fact that an [iterated contraction gives a summable orbit](../../../../../../iterated-contraction-gives-a-summable-orbit.md) applies here. Comparison with a [geometric series](../../../../../../geometric-series.md) therefore gives

$$
\sum_{n\ge1}|u_n|\le |x|\frac{0.99}{1-0.99}=99|x|<\infty.
$$

Thus **the nested-sine [series](../../../../../../series-mathematics.md) converges absolutely for every real $x$; there are no divergent or merely conditionally convergent cases**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
