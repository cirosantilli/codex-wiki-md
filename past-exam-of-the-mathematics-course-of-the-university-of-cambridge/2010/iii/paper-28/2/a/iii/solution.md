<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $G$ be the [cumulative distribution function](../../../../../../../cumulative-distribution-function.md) of the arbitrary Borel [probability measure](../../../../../../../probability-measure.md) $\mu$. It may have atoms or flat intervals. Use its [quantile function](../../../../../../../quantile-function.md)

$$
Q(u)=\inf\{x\in\mathbb R:G(x)\geq u\},\qquad0<u<1.
$$

The limits of $G$ at the two infinities make $Q(u)$ finite. Its monotonicity and right continuity imply the exact equivalence $Q(u)\leq x\iff u\leq G(x)$. For the nontrivial direction, if $Q(u)\leq x$, points with $G\geq u$ lie arbitrarily close above $Q(u)$; if the infimum itself is $x$, right continuity gives $G(x)\geq u$. The other direction follows directly from the defining infimum.

Take independent uniform variables $U_k$ and set $Y'_k=Q(U_k)$. Then

$$
\mathbb P(Y'_k\leq x)=\mathbb P(U_k\leq G(x))=G(x),
$$

so $(Y'_k)$ has the same entire sequence law as the original iid sample $(Y_k)$. On this construction, the [empirical distribution function](../../../../../../../empirical-distribution-function.md) satisfies

$$
G'_n(x)=\frac1n\sum_{k=1}^n\mathbf1_{\{U_k\leq G(x)\}}=F_n(G(x)).
$$

Thus part (ii) gives

$$
\sup_{x\in\mathbb R}|G'_n(x)-G(x)|
\leq\sup_{t\in[0,1]}|F_n(t)-t|\longrightarrow0\quad\text{almost surely}.
$$

The supremum is measurable: since both distribution functions are right-continuous, it equals the supremum over rational $x$. The convergence event consequently depends measurably on the coordinate sequence, and equality of the sequence laws transfers its probability one to $(Y_k)$. Hence

$$
\boxed{\sup_{x\in\mathbb R}|G_n(x)-G(x)|\longrightarrow0\quad\text{almost surely}.}
$$

This is the [Quantile proof of the Glivenko-Cantelli theorem](../../../../../../../quantile-proof-of-the-glivenko-cantelli-theorem.md), including arbitrary distributions with atoms. The original PDF supplies the full definition and absolute-value signs in this part, which the TeX conversion incompletely records.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
