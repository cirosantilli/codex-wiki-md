<h1 id="12f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\mathbf a,\mathbf b\in\mathbb R^{n+1}$, the [triangle inequality](../../../../../../triangle-inequality.md) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
\begin{aligned}
|S(\mathbf a)-S(\mathbf b)|
&\leq \lVert T(\mathbf a-\mathbf b)\rVert_\infty\\
&\leq \sum_{r=0}^n|a_r-b_r|
\leq \sqrt{n+1}\,\lVert\mathbf a-\mathbf b\rVert_2.
\end{aligned}
$$

Thus $S$ is a [continuous function](../../../../../../continuous-function.md). The [unit sphere](../../../../../../unit-sphere.md) in the finite-dimensional [Euclidean normed vector space](../../../../../../euclidean-norm.md) $\mathbb R^{n+1}$ is [compact](../../../../../../compact-space.md). Moreover, $S(\mathbf a)=0$ implies that the [polynomial](../../../../../../polynomial-split.md) $T\mathbf a$ vanishes identically, so every coefficient $a_r$ is zero. Hence $S$ is strictly positive on the unit sphere. By the [extreme value theorem](../../../../../../extreme-value-theorem.md), it has a positive minimum

$$
\delta=\min_{\lVert\mathbf a\rVert_2=1}S(\mathbf a)>0.
$$

The [supremum norm](../../../../../../supremum-norm.md) is homogeneous. For $\mathbf a\ne0$,

$$
\lVert T\mathbf a\rVert_\infty
=\lVert\mathbf a\rVert_2
 S\left(\frac{\mathbf a}{\lVert\mathbf a\rVert_2}\right)
\geq\delta\lVert\mathbf a\rVert_2.
$$

It follows directly that $\lVert T\mathbf a\rVert_\infty\to\infty$ whenever $\lVert\mathbf a\rVert_2\to\infty$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12F](../../12f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
