<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the [compact set](../../../../../../compact-space.md) $K\subseteq B\subseteq U$ chosen in the preceding step, the [Urysohn lemma](../../../../../../urysohn-s-lemma.md) gives a [continuous function](../../../../../../continuous-function.md) $0\leq\varphi\leq1$ equal to one on $K$ and zero on $X\setminus U$. In a [metric space](../../../../../../metric-space.md) this cutoff can also be written explicitly, when $K$ and $X\setminus U$ are both nonempty:

$$
\varphi(x)=\frac{d(x,X\setminus U)}{d(x,K)+d(x,X\setminus U)}.
$$

The two sets are disjoint and closed, so the denominator never vanishes, and their distance functions are [continuous](../../../../../../continuous-function.md). If $K$ is empty, take $\varphi=0$; if $U=X$ and $K$ is nonempty, take $\varphi=1$. These choices satisfy the required boundary conditions in the exceptional cases.

The difference $\varphi-\mathbf1_B$ vanishes on $K$ and outside $U$, and its [absolute value](../../../../../../absolute-value.md) is at most one everywhere. Therefore

$$
\boxed{\|\varphi-\mathbf1_B\|_{L^1(\mu)}\leq\mu(U\setminus K)<\epsilon.}
$$

This is the precise continuous approximation required by both proofs of [ergodicity](../../../../../../ergodicity.md), and also gives $|\int\varphi\,d\mu-\mu(B)|<\epsilon$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
