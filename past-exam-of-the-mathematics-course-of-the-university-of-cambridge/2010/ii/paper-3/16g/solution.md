<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

The [cumulative hierarchy](../../../../../cumulative-hierarchy.md) is defined by [transfinite recursion](../../../../../transfinite-recursion.md):

$$
V_0=\varnothing,\qquad V_{\alpha+1}=\mathcal P(V_\alpha),\qquad
V_\lambda=\bigcup_{\beta<\lambda}V_\beta\quad(\lambda\text{ a limit ordinal}).
$$

The [rank of a set](../../../../../rank-of-a-set.md) is $\operatorname{rk}(x)=\sup_{y\in x}(\operatorname{rk}(y)+1)$, equivalently the least $\alpha$ such that $x\subseteq V_\alpha$. The standard hierarchy properties give $\operatorname{rk}(V_\alpha)=\alpha$, so **every [ordinal](../../../../../ordinal.md) occurs as a set rank**; the [ordinal](../../../../../ordinal.md) $\alpha$ itself is another example of rank $\alpha$.

Let $x$ be transitive of rank $\alpha$, and fix $\beta<\alpha$. The supremum formula gives an element of $x$ whose rank is at least $\beta$. Choose such an element $y$ of least possible rank. If $\operatorname{rk}(y)>\beta$, the same supremum formula gives $z\in y$ with rank at least $\beta$. Transitivity gives $z\in x$, and membership strictly decreases rank, contradicting the choice of $y$. Thus **$x$ contains an element of every rank below $\alpha$**.

A nonempty finite set has rank the maximum of finitely many [successor ordinals](../../../../../successor-ordinal.md), hence a [successor ordinal](../../../../../successor-ordinal.md); the empty set has rank zero. Conversely, for any $\beta$, the singleton $\{V_\beta\}$ has rank $\beta+1$. Thus

$$
\boxed{\text{finite-set ranks are exactly }0\text{ and all successor ordinals}.}
$$

A finite [transitive set](../../../../../transitive-set.md) of rank $\alpha$ contains, by the proved property, distinct elements of every rank $\beta<\alpha$. Finiteness therefore forces $\alpha<\omega$. Every finite [ordinal](../../../../../ordinal.md) is itself a finite [transitive set](../../../../../transitive-set.md) of that rank. Consequently

$$
\boxed{\text{finite-transitive-set ranks are exactly the finite ordinals}.}
$$

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
