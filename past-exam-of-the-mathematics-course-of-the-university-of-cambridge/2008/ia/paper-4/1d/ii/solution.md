<h1 id="1d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**True.** The [function composition](../../../../../../function-composition.md) $j=g\circ f$ is an [injection](../../../../../../injective-function.md): $j(a)=j(a')$ first implies $f(a)=f(a')$ by the [injectivity](../../../../../../injective-function.md) of $g$, then $a=a'$ by the [injectivity](../../../../../../injective-function.md) of $f$. Fix one $a_0\in A$, using the given nonemptiness, and define

$$
h(c)=\begin{cases}a,&c=j(a)\text{ for some }a\in A,\\a_0,&c\notin j(A).\end{cases}
$$

The first case is well defined because $j$ is an [injection](../../../../../../injective-function.md). For every $a\in A$, $h(j(a))=a$. Thus this [left inverse](../../../../../../left-inverse.md) satisfies $\boxed{h\circ g\circ f=\operatorname{id}_A}$, the [identity function](../../../../../../identity-function.md) on $A$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1D](../../1d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
