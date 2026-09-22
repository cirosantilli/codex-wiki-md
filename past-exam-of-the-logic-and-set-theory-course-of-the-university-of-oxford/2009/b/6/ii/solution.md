<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply [Zorn's lemma](../../../../../zorn-s-lemma.md) using the chain upper bounds just proved, obtaining a maximal partial [group operation](../../../../../group-operation.md) $m$ on a nonempty carrier $A\subseteq X$. Suppose $|X\setminus A|\geq|A|$. Then choose a [subset](../../../../../subset.md) $B\subseteq X\setminus A$ and a [bijection](../../../../../bijection.md) $b:A\to B$. The [set](../../../../../set-split.md) $A\cup B$ can be identified with $A\times C_2$ by sending $(a,0)$ to $a$ and $(a,1)$ to $b(a)$.

Use [group extension by a duplicate carrier](../../../../../group-extension-by-a-duplicate-carrier.md) to transport the direct-product [group operation](../../../../../group-operation.md) along this [bijection](../../../../../bijection.md). Its restriction to $A\times A$ is exactly the original $m$, because $(a,0)(a',0)=(m(a,a'),0)$. It therefore gives a strictly larger member of $\mathcal G$, contradicting maximality. Thus $|A|\nleq|X\setminus A|$. Cardinal comparability, allowed as a consequence of [Zorn's lemma](../../../../../zorn-s-lemma.md), leaves the strict opposite inequality:

$$
\boxed{|X\setminus A|<|A|.}
$$

The argument uses choice through [Zorn's lemma](../../../../../zorn-s-lemma.md) and cardinal comparability; the extension itself is an explicit transported direct-product operation once the [bijection](../../../../../bijection.md) with $B$ is chosen.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
