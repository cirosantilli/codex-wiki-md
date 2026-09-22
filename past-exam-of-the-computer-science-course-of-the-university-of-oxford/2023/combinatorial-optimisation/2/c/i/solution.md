<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [rank of a matroid](../../../../../../rank-of-a-matroid.md) on a [subset](../../../../../../subset.md) $A\subseteq X$ is

$$
\boxed{r(A)=\max\{|I|:I\subseteq A,\ I\in\mathcal I\}.}
$$

The [matroid independence axioms](../../../../../../matroid-independence-axioms.md) imply that every maximal [matroid independent set](../../../../../../independent-set-of-a-matroid.md) in $A$ has this [cardinality](../../../../../../cardinality.md). We write $A+x=A\cup\{x\}$, as in the source. Directly from the definition,

$$
A\subseteq B\Longrightarrow r(A)\leq r(B),\qquad
r(A)\leq r(A+x)\leq r(A)+1.
$$

For the last upper bound, deleting $x$ from any [matroid independent set](../../../../../../independent-set-of-a-matroid.md) in $A+x$ leaves an independent [subset](../../../../../../subset.md) of $A$.

## ↑ Ancestors (12)

1. [I](../i.md)
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
