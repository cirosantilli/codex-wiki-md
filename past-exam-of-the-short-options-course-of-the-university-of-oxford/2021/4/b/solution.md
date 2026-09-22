<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $x\in U$. Since $U$ is open, choose an open [ball](../../../../ball-mathematics.md) $B(x,\varepsilon)\subset U$. For any $y$ in this ball the segment $x+t(y-x)$ remains in it. For each coordinate $G_j$, the [chain rule](../../../../chain-rule.md) gives

$$
\frac d{dt}G_j(x+t(y-x))=DG_j{}_{x+t(y-x)}(y-x)=0.
$$

The ordinary [mean value theorem](../../../../mean-value-theorem.md) therefore gives $G_j(y)=G_j(x)$ for every coordinate, hence $G(y)=G(x)$. Thus $G$ is a [locally constant function](../../../../locally-constant-function.md).

For each $z\in\mathbb R^m$, its [preimage](../../../../preimage.md) is a union of such open balls, so $G^{-1}(\{z\})$ is open in $\mathbb R^n$. Its complement in $U$ is the union of the other fibers and is also open. If $U$ is nonempty and [connected](../../../../connected-space.md), the nonempty fiber through any chosen point is both open and closed in $U$, and must be all of $U$. Therefore

$$
\boxed{DG\equiv0\quad\Longrightarrow\quad G\text{ locally constant, and constant on connected }U.}
$$

The empty-domain case is vacuous. Notice that continuity of $DG$ was never needed.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
