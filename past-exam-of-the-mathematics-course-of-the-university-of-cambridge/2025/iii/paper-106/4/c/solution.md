<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $X$ is a [reflexive Banach space](../../../../../../reflexive-banach-space.md), its closed unit ball is weakly compact. A bounded linear map is weak-to-weak continuous, so $T(B_X)$ is weakly compact in $Y$. Compact subsets of a Hausdorff space are closed, hence $T(B_X)$ is weakly closed and therefore norm closed.

Now suppose the two norms on $V$ have the same continuous dual as a set. Each $X_j^*$ is a [Banach space](../../../../../../banach-space-split.md) in its dual norm. The identity

$$
I:(X_1^*,\|\cdot\|_{1,*})\longrightarrow(X_2^*,\|\cdot\|_{2,*})
$$

has closed graph: if $f_n\to f$ in the first dual norm and $f_n\to g$ in the second, evaluating at each $x\in V$ gives $f(x)=g(x)$. The [closed graph theorem](../../../../../../closed-graph-theorem.md) makes $I$ bounded, and the same argument for $I^{-1}$ makes the dual norms equivalent. Thus there are $c,C>0$ with

$$
c\|f\|_{1,*}\leq\|f\|_{2,*}\leq C\|f\|_{1,*}.
$$

The dual formula

$$
\|x\|_j=\sup_{\|f\|_{j,*}\leq1}|f(x)|
$$

from the Hahn--Banach theorem transfers these inequalities to the original norms. Hence $\|\cdot\|_1$ and $\|\cdot\|_2$ are equivalent.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
