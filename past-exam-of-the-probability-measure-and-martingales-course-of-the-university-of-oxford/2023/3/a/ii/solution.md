<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $P_n=X_nY_nZ_n$. Before $\tau$, all three players are active. Each unordered pair is selected with [probability](../../../../../probability.md) $1/3$, and each direction of transfer then has [conditional probability](../../../../../conditional-probability.md) $1/2$. Given the current holdings $(x,y,z)$, a transfer within the first pair has mean product

$$
\frac{(x+1)(y-1)z+(x-1)(y+1)z}{2}=xyz-z.
$$

For transfers within the other two pairs the analogous values are $xyz-y$ and $xyz-x$. Averaging over pairs gives

$$
\mathbb E[P_{n+1}-P_n\mid\mathcal F_n]=-\frac{x+y+z}{3}=-\frac N3
\quad\text{on }\{n<\tau\}.
$$

At and after elimination the product is zero, since an eliminated player never re-enters. In particular the [stopped process](../../../../../stopped-process.md) has increment

$$
M_{(n+1)\wedge\tau}-M_{n\wedge\tau}
=\mathbf1_{\{n<\tau\}}\left(P_{n+1}-P_n+\frac N3\right).
$$

The [indicator function](../../../../../indicator-function.md) is $\mathcal F_n$-[measurable](../../../../../measurability.md), and the expression in parentheses has zero [conditional expectation](../../../../../conditional-expectation.md) on its support. The [stopped process](../../../../../stopped-process.md) is [adapted](../../../../../adapted-process.md) and [integrable](../../../../../integrability.md): at fixed $n$, its absolute value is bounded by $N^3+nN/3$. Hence

$$
\boxed{(M_{n\wedge\tau})_{n\geq0}\text{ is a martingale},\qquad M_0=abc.}
$$

This is the [product martingale for three-player token exchange](../../../../../product-martingale-for-three-player-token-exchange.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
