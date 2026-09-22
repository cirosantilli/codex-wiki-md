<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

After replacing $X$ by a maximal $D$-linearly independent subset with the same span, write $X=\{x_1,\ldots,x_n\}$. The standard independence lemma, proved by induction using Schur's lemma, says

$$
\bigcap_{i<n}\operatorname{ann}_R(x_i)\,x_n\ne0.
$$

Otherwise $rx_n$ would depend only on $(rx_1,\ldots,rx_{n-1})$, defining an $R$-map whose coordinate maps lie in $\operatorname{End}_R(V)$ and forcing $x_n\in\sum_{i<n}x_iD$. Applying the same argument with $y$ shows that $\bigcap_i\operatorname{ann}_R(x_i)y=0$ implies $y\in XD$, proving the requested claim.

The [Jacobson density theorem](../../../../../../jacobson-density-theorem.md) states that if $x_1,\ldots,x_n$ are $D$-independent and $y_1,\ldots,y_n\in V$, there is $r\in R$ with $rx_i=y_i$ for every $i$. Induct on $n$. First match the first $n-1$ values. The independence lemma makes $I x_n$, for $I=\bigcap_{i<n}\operatorname{ann}_R(x_i)$, a nonzero submodule and hence all of $V$; an element of $I$ supplies the final correction.

If $R$ is primitive, choose a faithful simple module $V$. When $\dim_DV=n<\infty$, density makes $R\to\operatorname{End}_D(V)\cong\operatorname{Mat}_n(D)$ surjective and faithfulness makes it injective. If $\dim_DV$ is infinite, choose an $n$-dimensional $D$-subspace $W$ and let $R_n=\{r:rW\subseteq W\}$. Density makes restriction $R_n\to\operatorname{End}_D(W)\cong\operatorname{Mat}_n(D)$ surjective.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 139](../../../paper-139-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
