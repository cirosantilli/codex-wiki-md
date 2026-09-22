<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an [idempotent](../../../../../idempotent.md) $e\in R$, define the [principal open subset](../../../../../principal-open-subscheme.md) $D(e)\subseteq\operatorname{Spec}R$. Since $e(1-e)=0$, a [prime ideal](../../../../../prime-ideal.md) contains at least one of $e,1-e$, and it cannot contain both. Therefore

$$
D(e)=V(1-e),\qquad \operatorname{Spec}R=D(e)\sqcup D(1-e).
$$

Thus $D(e)$ is a [clopen set](../../../../../clopen-set.md).

Conversely, let $C$ be a [clopen set](../../../../../clopen-set.md) in $T=\operatorname{Spec}R$. The [structure sheaf](../../../../../structure-sheaf-of-a-scheme.md) glues the section $1$ on $C$ and the section $0$ on its complement to a unique [global section](../../../../../global-section.md) $e\in\Gamma(T,\mathcal O_T)=R$. Checking on these two [open subsets](../../../../../open-set.md) gives $e^2=e$, and $D(e)=C$. Conversely, the restriction of an [idempotent](../../../../../idempotent.md) $e$ to $D(e)$ is $1$ because $e$ is a [unit](../../../../../unit-in-a-ring.md) there, and its restriction to $D(1-e)$ is $0$. Thus the two constructions are inverse, including for the zero [ring](../../../../../ring.md):

$$
\boxed{\{e\in R:e^2=e\}\ \longleftrightarrow\ \{C\subseteq\operatorname{Spec}R:C\text{ clopen}\},\qquad e\longmapsto D(e).}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the introduction to schemes course of the University of Oxford](../../../../split.md)
6. [Introduction to schemes course of the University of Oxford](../../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
