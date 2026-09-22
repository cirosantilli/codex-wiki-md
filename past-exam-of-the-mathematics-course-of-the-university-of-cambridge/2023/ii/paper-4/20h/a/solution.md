<h1 id="20h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Minkowski's lemma](../../../../../../minkowski-s-theorem.md) states that if $\Lambda$ is a full lattice in $\mathbb R^n$ and $C\subset\mathbb R^n$ is measurable, [convex](../../../../../../convex-set.md), and centrally symmetric, then

$$
\operatorname{vol}(C)>2^n\operatorname{covol}(\Lambda)
$$

implies that $C$ contains a nonzero point of $\Lambda$.

Let $\sigma_1,\sigma_2:K\to\mathbb R$ be the two real embeddings. The [Minkowski embedding of a real quadratic field](../../../../../../minkowski-embedding-of-a-real-quadratic-field.md) identifies $\mathcal O_K$ with a lattice

$$
\Lambda=\{(\sigma_1(\alpha),\sigma_2(\alpha)):\alpha\in\mathcal O_K\}
$$

of covolume $\sqrt{|D_K|}$. Choose a constant $c$ satisfying

$$
2\sqrt{|D_K|}<c<4\sqrt{|D_K|}.
$$

For $R>0$, consider the closed diamond

$$
C_R=
\left\{(x,y):\frac{|x|}{R}+\frac{|y|}{c/R}\leq1\right\}.
$$

It is convex and centrally symmetric, and its area is

$$
\operatorname{vol}(C_R)=2R\frac cR=2c>4\sqrt{|D_K|}.
$$

Minkowski's lemma supplies a nonzero $\alpha_R\in\mathcal O_K$ whose two embeddings lie in $C_R$.

For $(x,y)\in C_R$, the [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md) gives

$$
|xy|leq\frac14R\frac cR=\frac c4<\sqrt{|D_K|}.
$$

Since the coordinate product is the [field norm](../../../../../../field-norm.md),

$$
|N_{K/\mathbb Q}(\alpha_R)|<\sqrt{|D_K|}.
$$

Finally, $|\sigma_2(\alpha_R)|\leq c/R\to0$ as $R\to\infty$. No fixed nonzero [algebraic integer](../../../../../../algebraic-integer.md) can occur for arbitrarily large $R$, because its second embedding is nonzero. Consequently the elements $\alpha_R$ obtained along an unbounded sequence of $R$ contain infinitely many distinct values. Here $N(\alpha)$ denotes the absolute norm, as usual in this inequality.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20H](../../20h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
