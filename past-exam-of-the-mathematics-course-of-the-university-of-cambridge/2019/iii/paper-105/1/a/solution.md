<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $u_Q=|Q|^{-1}\int_Qu$. Since $u-u_Q$ has [arithmetic mean](../../../../../../arithmetic-mean.md) zero,

$$
\|u\|_{L^2(Q)}^2=|Q|u_Q^2+\|u-u_Q\|_{L^2(Q)}^2,
$$

and the pairwise-difference identity gives

$$
\|u-u_Q\|_{L^2(Q)}^2
=\frac1{2|Q|}\int_Q\int_Q|u(x)-u(y)|^2\,dx\,dy.
$$

First take $u$ [smooth](../../../../../../smooth-function.md). Join $x$ to $y$ by changing one coordinate at a time and apply the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md):

$$
|u(x)-u(y)|^2
\leq n\sum_{i=1}^n
|u(x_1,\ldots,x_i,y_{i+1},\ldots,y_n)-u(x_1,\ldots,x_{i-1},y_i,\ldots,y_n)|^2.
$$

For a one-dimensional slice $v$, the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) yields

$$
|v(s)-v(t)|^2\leq |s-t|\int_{\min(s,t)}^{\max(s,t)}|v'(r)|^2\,dr
\leq L\int_0^L|v'(r)|^2\,dr.
$$

Integrating the $i$th summand over $x,y\in Q$ therefore gives at most $L^{n+2}\|D_i u\|_{L^2(Q)}^2$. Hence

$$
\|u-u_Q\|_{L^2(Q)}^2\leq\frac n2L^2\|Du\|_{L^2(Q)}^2.
$$

The [density of smooth functions in a Sobolev space](../../../../../../density-of-smooth-functions-in-a-sobolev-space.md) extends the estimate to every $u\in H^1(\mathbb R^n)$. Thus

$$
\boxed{\|u\|_{L^2(Q)}^2\leq |Q|u_Q^2+\frac n2L^2\|Du\|_{L^2(Q)}^2.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
