<h1 id="29k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the time-inverted Brownian motion $B_u=uW_{1/u}$. For $s>0$, set $u=1/s$. Then

$$
W_s-as\leq b
\quad\Longleftrightarrow\quad
\frac{W_s}{s}-a\leq\frac bs
\quad\Longleftrightarrow\quad
B_u-bu\leq a.
$$

As $0<s\leq t$ corresponds exactly to $u\geq1/t$, and the inequality at $s=0$ is automatic because $b>0$, this is the pathwise identity

$$
\left\{\sup_{0\leq s\leq t}(W_s-as)\leq b\right\}
=\left\{\sup_{u\geq1/t}(B_u-bu)\leq a\right\}.
$$

Since $B$ and $W$ have the same law by [time inversion of Brownian motion](../../../../../../time-inversion-of-brownian-motion.md),

$$
\boxed{
\mathbb P\!\left(\sup_{0\leq s\leq t}(W_s-as)\leq b\right)
=\mathbb P\!\left(\sup_{u\geq1/t}(W_u-bu)\leq a\right).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
