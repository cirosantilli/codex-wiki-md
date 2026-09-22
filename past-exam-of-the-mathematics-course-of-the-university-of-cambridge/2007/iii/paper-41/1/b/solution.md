<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose $A_0\in\operatorname{ri}K$. We first justify the finite-dimensional fact $\operatorname{ri}K\subseteq D$, since $D$ itself need not be closed. Around any relative-interior point $z$, choose a small [simplex](../../../../../../simplex.md) in $L$ whose vertices lie in $K$ and which contains $z$ strictly inside. Approximate its vertices by points of $D$, possible because $\overline D=K$. For close enough approximations, the barycentric coordinates of $z$ remain strictly positive; hence $z$ is a convex combination of points of $D$ and belongs to $D$. If $L=\{0\}$, the assertion is immediate.

Let $m=\mathbb E[wA_1]\in L$. Relative openness lets us choose $\varepsilon>0$ such that $A_0-\varepsilon m\in\operatorname{ri}K\subseteq D$. There is therefore a bounded nonnegative measurable $f$ satisfying $A_0-\varepsilon m=\mathbb E[w fA_1]$. Set

$$
\boxed{\nu=w(f+\varepsilon)>0.}
$$

Then $\mathbb E[\nu A_1]=A_0$ and $\mathbb E\|\nu A_1\|\leq\|f\|_\infty+\varepsilon<\infty$. This proves existence with strict positivity even when the unweighted asset vector is not integrable.

It also proves the [strictly positive barycentre cone lemma](../../../../../../strictly-positive-barycentre-cone-lemma.md). Every strictly positive weighted barycentre must lie in $\operatorname{ri}K$: otherwise the supporting vector constructed for the relative boundary would have zero value at that barycentre while its strictly positive weighted payoff had positive expectation. Thus the [relative interior](../../../../../../relative-interior.md) is exactly the set of such barycentres.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
