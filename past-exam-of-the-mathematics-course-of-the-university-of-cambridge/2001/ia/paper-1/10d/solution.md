<h1 id="10d/solution">Solution</h1>

↑ **Parent:** [10D](../10d.md)

To prove the [intermediate value theorem](../../../../../intermediate-value-theorem.md) in this setting, let $A=\{t\in[a,b]:f(t)<v\}$ and $c=\sup A$. The endpoint inequalities and [continuity](../../../../../continuous-function.md) give an interval immediately to the right of $a$ contained in $A$ and an interval immediately to the left of $b$ disjoint from $A$. Thus $a<c<b$. Choose points of $A$ tending to $c$; [continuity](../../../../../continuous-function.md) gives $f(c)\le v$. If $f(c)<v$, [continuity](../../../../../continuous-function.md) would place some point larger than $c$ in $A$, contradicting the supremum. Hence **$\boxed{f(c)=v}$** at an interior point.

For a continuous self-map of $[a,b]$, define $g(t)=f(t)-t$. The range condition implies $g(a)\ge0$ and $g(b)\le0$. If either is zero, its endpoint is a [fixed point](../../../../../fixed-point.md). Otherwise apply the just-proved [intermediate value theorem](../../../../../intermediate-value-theorem.md) to $-g$ with target zero to obtain $d\in(a,b)$ and $g(d)=0$. Therefore

$$
\boxed{\text{Every continuous self-map of }[a,b]\text{ has a fixed point.}}
$$

This proves the [fixed-point property of a closed interval](../../../../../fixed-point-property-of-a-closed-interval.md) without requiring $f$ itself to be monotone.

## ↑ Ancestors (10)

1. [10D](../10d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
