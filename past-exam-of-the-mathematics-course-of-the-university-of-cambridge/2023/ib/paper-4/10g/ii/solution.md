<h1 id="10g/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $X$ be [compact](../../../../../../compact-space.md) and $q:X\to X/R$ the quotient map. If $(U_i)_{i\in I}$ is an open cover of $X/R$, then $(q^{-1}(U_i))_{i\in I}$ is an open cover of $X$. A finite subfamily covers $X$; because $q$ is surjective, the corresponding $U_i$ cover $X/R$. Thus every quotient of a compact space is compact.

The Hausdorff property need not survive. On the [real line](../../../../../../real-line.md), define

$$
xRy\quad\Longleftrightarrow\quad x-y\in\mathbb Q.
$$

The quotient $\mathbb R/\mathbb Q$ has more than one point. If two nonempty open subsets of the quotient were disjoint, their inverse images would be disjoint nonempty open subsets of $\mathbb R$ invariant under rational translation. But any two nonempty open intervals acquire an intersection after one is translated by a suitably chosen rational number, so two such saturated open sets cannot be disjoint. Distinct quotient points cannot be separated, and the quotient is not Hausdorff. This is the [non-Hausdorff quotient of the real line by rational translation](../../../../../../non-hausdorff-quotient-of-the-real-line-by-rational-translation.md).

Finally let $f:X\to Y$ be a continuous bijection, with $X$ compact and $Y$ Hausdorff. Every closed subset $C\subseteq X$ is compact. Its continuous image $f(C)$ is compact, and every compact subset of a Hausdorff space is closed. Hence $f$ is a [closed map](../../../../../../closed-map.md). For every closed $C\subseteq X$,

$$
(f^{-1})^{-1}(C)=f(C)
$$

is closed in $Y$, so $f^{-1}$ is continuous. Therefore $f$ is a homeomorphism. This is the [compact-to-Hausdorff continuous bijection theorem](../../../../../../compact-to-hausdorff-continuous-bijection-theorem.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10G](../../10g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
