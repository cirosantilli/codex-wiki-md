<h1 id="algebra/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Expanding gives $(I-E)^2-(I-E)=E^2-E$, so either operator is [idempotent](../../../../idempotent.md) exactly when the other is. For an [idempotent](../../../../idempotent.md) $E$,

$$
v=(v-Ev)+Ev,\qquad E(v-Ev)=0.
$$

If $w\in\ker E\cap\operatorname{Im}E$, write $w=Eu$; then $0=Ew=E^2u=Eu=w$. Hence $V=\ker E\oplus\operatorname{Im}E$.

Next,

$$
(E_1+E_2)^2-(E_1+E_2)=E_1E_2+E_2E_1.
$$

If the right side vanishes, left multiplication by $E_1$ gives $E_1E_2+E_1E_2E_1=0$, while right multiplication gives $E_1E_2E_1+E_2E_1=0$. Subtraction shows $E_1E_2=E_2E_1$, and their original sum now gives $2E_1E_2=0$. Over the real or complex numbers this implies **$E_1E_2=E_2E_1=0$**.

For three [idempotents](../../../../idempotent.md) summing to $I$, each pair sum equals the complementary [idempotent](../../../../idempotent.md) $I-E_k$. Thus every product of distinct operators vanishes. Every [vector](../../../../vector.md) equals $E_1v+E_2v+E_3v$. If $v_1+v_2+v_3=0$ with $v_i\in\operatorname{Im}E_i$, applying $E_j$ gives $v_j=0$. Therefore

$$
\boxed{V=\operatorname{Im}E_1\oplus\operatorname{Im}E_2\oplus\operatorname{Im}E_3.}
$$

Take a [basis](../../../../basis.md) of each summand and unite the three [bases](../../../../basis.md). A [vector](../../../../vector.md) in the $j$th [basis](../../../../basis.md) has [eigenvalue](../../../../eigenvalue.md) one for $E_j$ and [zero](../../../../zero-of-a-function.md) for the other two, so this is the requested common [eigenbasis](../../../../eigenbasis.md). [Zero](../../../../zero-of-a-function.md) summands simply contribute no [basis](../../../../basis.md) [vectors](../../../../vector.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Algebra](../../algebra.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
