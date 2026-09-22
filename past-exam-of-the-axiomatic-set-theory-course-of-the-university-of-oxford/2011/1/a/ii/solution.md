<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Two facts about a [transitive set](../../../../../transitive-set.md) $A$ drive the [transfinite induction](../../../../../transfinite-induction.md). First, $A\subseteq\mathcal P(A)$: every $x\in A$ is a subset of $A$. Second, $\mathcal P(A)$ is a [transitive set](../../../../../transitive-set.md): if $x\in y\in\mathcal P(A)$, then $x\in A$, hence $x\subseteq A$, hence $x\in\mathcal P(A)$.

Starting with $V_0=\varnothing$, these facts prove the successor step. At a [limit ordinal](../../../../../limit-ordinal.md) $\lambda$, the union of the earlier increasing [transitive sets](../../../../../transitive-set.md) is transitive: if $x\in y\in V_\lambda$, some $\alpha<\lambda$ contains $y$ in $V_\alpha$, and transitivity puts $x$ there too. The union contains every earlier stage. Thus the induction gives both transitivity and $V_\beta\subseteq V_\alpha$ whenever $\beta\leq\alpha$.

Finally $V_\alpha\subseteq V_\alpha$, so $V_\alpha\in\mathcal P(V_\alpha)=V_{\alpha+1}$. The [Axiom of foundation](../../../../../axiom-of-regularity.md) gives $V_\alpha\notin V_\alpha$. This witnesses strictness:

$$
\boxed{V_\alpha\text{ is transitive},\qquad V_\alpha\subsetneq V_{\alpha+1}.}
$$

This is the [transitivity and strict growth of the cumulative hierarchy](../../../../../transitivity-and-strict-growth-of-the-cumulative-hierarchy.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Axiomatic set theory course of the University of Oxford](../../../../../axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
