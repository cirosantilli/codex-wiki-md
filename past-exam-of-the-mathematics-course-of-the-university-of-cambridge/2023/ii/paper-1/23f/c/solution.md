<h1 id="23f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Compact support and the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) give, for every $(x,y)$,

$$
\begin{aligned}
|u(x,y)|^2
&=\left|\int_{-\infty}^y\partial_t|u(x,t)|^2\,dt\right|\\
&\leq2\int_{\mathbb R}|u(x,t)|\,|\partial_2u(x,t)|\,dt
\leq2A(x),
\end{aligned}
$$

where

$$
A(x)=\int_{\mathbb R}|u(x,t)|\,|\nabla u(x,t)|\,dt.
$$

Applying the same argument in the other coordinate gives

$$
|u(x,y)|^2\leq2B(y),
\qquad
B(y)=\int_{\mathbb R}|u(t,y)|\,|\nabla u(t,y)|\,dt.
$$

Multiplication and [Fubini's theorem](../../../../../../fubini-s-theorem.md) now yield

$$
\begin{aligned}
\int_{\mathbb R^2}|u(x,y)|^4\,dx\,dy
&\leq4\int_{\mathbb R^2}A(x)B(y)\,dx\,dy\\
&=4\left(\int_{\mathbb R^2}|u|\,|\nabla u|\right)^2.
\end{aligned}
$$

Finally, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\left(\int_{\mathbb R^2}|u|\,|\nabla u|\right)^2
\leq
\left(\int_{\mathbb R^2}|u|^2\right)
\left(\int_{\mathbb R^2}|\nabla u|^2\right).
$$

**Thus the required estimate holds with $C=4$; it is the [Ladyzhenskaya inequality in two dimensions](../../../../../../ladyzhenskaya-inequality-in-two-dimensions.md).**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [23F](../../23f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
