<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We first justify the [submodularity of matroid rank](../../../../../../submodularity-of-matroid-rank.md), which will also support later arguments. Choose a maximal [matroid independent set](../../../../../../independent-set-of-a-matroid.md) $I_0$ in $A\cap B$, extend it to a maximal [matroid independent set](../../../../../../independent-set-of-a-matroid.md) $I_A$ in $A$, and then to one $I_U$ in $A\cup B$. These extensions exist by successive additions, and their sizes are the respective values of the [rank of a matroid](../../../../../../rank-of-a-matroid.md). No element of $I_U\setminus I_A$ lies in $A$: such an element could have been added to $I_A$, contradicting maximality in $A$. Therefore $I_0\cup(I_U\setminus I_A)$ is an independent [subset](../../../../../../subset.md) of $B$, giving

$$
r(A\cap B)+r(A\cup B)-r(A)\leq r(B).
$$

Now let $Y\subseteq Z$ and $x\in\sigma(Y)$. If $x\in Z$, then $x\in\sigma(Z)$ by (ii). Otherwise apply [submodularity of matroid rank](../../../../../../submodularity-of-matroid-rank.md) to $Y+x$ and $Z$, whose [intersection](../../../../../../set-intersection.md) is $Y$:

$$
r(Z+x)+r(Y)\leq r(Y+x)+r(Z)=r(Y)+r(Z).
$$

The monotonicity of the [rank of a matroid](../../../../../../rank-of-a-matroid.md) supplies the opposite bound $r(Z+x)\geq r(Z)$, so equality holds. Thus $x\in\sigma(Z)$, proving **$\sigma(Y)\subseteq\sigma(Z)$**.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Combinatorial optimisation](../../../../combinatorial-optimisation-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
