<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A family $(Y_i)_{i\in I}$ of integrable [random variables](../../../../../../random-variable-split.md) is [uniformly integrable](../../../../../../uniform-integrability.md) if

$$
\boxed{\lim_{K\to\infty}\sup_{i\in I}\mathbb E\bigl[|Y_i|\mathbf1_{\{|Y_i|>K\}}\bigr]=0.}
$$

This controls the contributions of large values uniformly over the family, rather than merely bounding its [L1 norms](../../../../../../l1-norm.md).

Put $X_n=\mathbb E[Z\mid\mathcal F_n]$ and $A_n(K)=\{|X_n|>K\}\in\mathcal F_n$. The [conditional Jensen inequality](../../../../../../conditional-jensen-inequality.md) gives $|X_n|\leq\mathbb E[|Z|\mid\mathcal F_n]$, hence $\mathbb E|X_n|\leq\mathbb E|Z|$. The [Markov inequality](../../../../../../markov-inequality.md) therefore gives

$$
\mathbb P(A_n(K))\leq\frac{\mathbb E|Z|}{K}.
$$

Using the measurability of $A_n(K)$ in the defining integral identity for [conditional expectation](../../../../../../conditional-expectation.md), for every $R>0$ we get

$$
\begin{aligned}
\mathbb E[|X_n|\mathbf1_{A_n(K)}]
&\leq\mathbb E[|Z|\mathbf1_{A_n(K)}]\\
&\leq\mathbb E[|Z|\mathbf1_{\{|Z|>R\}}]+R\mathbb P(A_n(K))\\
&\leq\mathbb E[|Z|\mathbf1_{\{|Z|>R\}}]+\frac{R\mathbb E|Z|}{K}.
\end{aligned}
$$

The first term tends to zero as $R\to\infty$ because $Z$ is integrable, by the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md). Given $\varepsilon>0$, first choose $R$ to make it less than $\varepsilon/2$, then choose $K$ to make the second term less than $\varepsilon/2$. These choices work for every $n$. This proves [uniform integrability of conditional expectations](../../../../../../uniform-integrability-of-conditional-expectations.md):

$$
\boxed{\{\mathbb E[Z\mid\mathcal F_n]:n\geq1\}\text{ is uniformly integrable}.}
$$

In fact the argument works for an arbitrary family of [sigma-algebras](../../../../../../sigma-algebra.md); nesting is not needed for this conclusion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
