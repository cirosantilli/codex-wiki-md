<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [weak topology](../../../../../../weak-topology-split.md) $\sigma(X,X^*)$ is the coarsest topology on $X$ for which every bounded linear functional in $X^*$ is continuous. Thus every $f\in X^*$ is weakly continuous. Conversely, if a linear functional $f$ is weakly continuous at zero, some basic weak neighbourhood gives $f_1,\ldots,f_n\in X^*$ and $\varepsilon>0$ such that

$$
|f_j(x)|<\varepsilon\ (1\leq j\leq n)
\quad\Longrightarrow\quad |f(x)|<1.
$$

It follows that $\bigcap_j\ker f_j\subseteq\ker f$, and elementary linear algebra then gives $f\in\operatorname{span}\{f_1,\ldots,f_n\}\subseteq X^*$.

To prove [Mazur theorem](../../../../../../mazur-theorem.md), let $K$ be norm-closed and convex and let $x\notin K$. The [Hahn-Banach separation theorem](../../../../../../hahn-banach-separation-theorem.md) strictly separates $x$ from $K$ by some member of $X^*$. The corresponding open half-space is weakly open, contains $x$, and misses $K$. Thus $K$ is weakly closed.

If $X$ is reflexive, the [Banach-Alaoglu theorem](../../../../../../banach-alaoglu-theorem.md) makes $B_{X^{**}}$ weak-star compact, and the canonical identification transports this to weak compactness of $B_X$. Conversely, if $B_X$ is weakly compact, then $J(B_X)$ is weak-star compact and hence weak-star closed in $B_{X^{**}}$. [Goldstine theorem](../../../../../../goldstine-theorem.md) says it is weak-star dense there, so it equals $B_{X^{**}}$ and $X$ is reflexive.

When $X$ is reflexive, weak and weak-star topologies coincide on $X^*$, so Banach–Alaoglu makes $B_{X^*}$ weakly compact and $X^*$ is reflexive. If $Y\subseteq X$ is closed, then $B_Y$ is a weakly closed subset of $B_X$, hence weakly compact. The quotient map sends a suitable weakly compact ball of $X$ onto the unit ball of $X/Y$, which is therefore weakly compact. Thus $Y$ and $X/Y$ are reflexive as well.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
