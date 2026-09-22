<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $p(x)=\mathbb P(X_1^n=x)$, $a(x)=p(x)W(x)$, and

$$
A=\sum_xa(x)=\mathbb E[W(X_1^n)].
$$

On the support of $p$, define the [probability mass function](../../../../../../probability-mass-function.md)

$$
R^*(x)=\frac{a(x)}A=\frac{p(x)W(x)}{\mathbb E[W(X_1^n)]}.
$$

For any real length function satisfying the [Kraft inequality](../../../../../../kraft-mcmillan-inequality.md), put $K=\sum_x2^{-L(x)}\leq1$ and $R_L(x)=2^{-L(x)}/K$. The [Gibbs inequality](../../../../../../gibbs-inequality.md) gives

$$
\begin{aligned}
\sum_xa(x)L(x)
&=A\sum_xR^*(x)\{-\log_2R_L(x)-\log_2K\}\\
&=A\{H(R^*)+D(R^*\Vert R_L)-\log_2K\}\\
&\geq AH(R^*).
\end{aligned}
$$

Equality holds for the ideal weighted lengths

$$
L_n^*(x)=-\log_2R^*(x)
=\log_2\frac{\mathbb E[W(X_1^n)]}{p(x)W(x)}.
$$

Thus the smallest average weighted description length is

$$
\mathbb E[W(X_1^n)]
H\!\left(\frac{p(\mathord\cdot)W(\mathord\cdot)}{\mathbb E W(X_1^n)}\right).
$$

When $p$ has full support, the displayed $L_n^*$ attains this minimum. If some strings have zero probability, the same value is the infimum over finite lengths and is attained by the extended-real ideal assignment $L_n^*(x)=\infty$ there; finite codewords of arbitrarily large length approach it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
