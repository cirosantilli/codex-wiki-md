<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [Kronecker quiver](../../../../../../kronecker-quiver.md) representation with arrows $I$ and $N=\left(\begin{smallmatrix}0&1\\0&0\end{smallmatrix}\right)$, an endomorphism $(P,Q)$ satisfies $Q=P$ and $PN=NP$. Solving the second equation gives

$$
\operatorname{End}_Q(X)=\left\{\begin{pmatrix}a&b\\0&a\end{pmatrix}:a,b\in k\right\}\cong k[t]/(t^2).
$$

Thus **this representation is indecomposable but is not a brick**: its endomorphism ring is a [local endomorphism ring](../../../../../../local-endomorphism-ring.md), while the nonzero endomorphism $N$ is nilpotent.

For a general indecomposable non-brick, the [proof of Ringel lemma on bricks](../../../../../../proof-of-ringel-lemma-on-bricks.md) finds a proper indecomposable submodule with nonzero self-extensions. Repetition in strictly decreasing dimension reaches a [brick module](../../../../../../brick-module.md) $Y\subset X$ with $\operatorname{Ext}^1_Q(Y,Y)\ne0$. The linked proof supplies the minimal-rank, retraction and hereditary-extension steps.

Now assume the [Tits form of a quiver](../../../../../../tits-form-of-a-quiver.md) is positive definite. If an indecomposable $X$ were not a brick, this $Y$ would give the contradiction

$$
0<q(\dim Y)=1-\dim\operatorname{Ext}^1_Q(Y,Y)\le0.
$$

Hence $X$ is a brick. For its nonzero dimension vector $\mathbf n$, positivity and integrality then imply

$$
0<q(\mathbf n)=1-\dim\operatorname{Ext}^1_Q(X,X)\le1,\qquad \boxed{q(\mathbf n)=1,\quad\operatorname{Ext}^1_Q(X,X)=0}.
$$

Thus every indecomposable in this case is a rigid brick. This deduction uses the [Ringel lemma on bricks](../../../../../../ringel-lemma-on-bricks.md) and the [Ringel form](../../../../../../ringel-form.md), without requiring the full [Gabriel theorem](../../../../../../gabriel-s-theorem.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
