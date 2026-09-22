<h1 id="b/8/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $a\in L$. In the ambient universe form the [set](../../../../../set-split.md)

$$
S=\{y\in\mathcal P(a):y\in L\}
$$

by [power set](../../../../../power-set.md) and [separation](../../../../../axiom-schema-of-specification.md), using definability of $L$. This is the collection which must serve as the [power set](../../../../../power-set.md) of $a$ inside $L$; it need not be the entire ambient [power set](../../../../../power-set.md).

For each $y\in S$, let $\alpha_y$ be the least [ordinal](../../../../../ordinal-split.md) with $y\in L_{\alpha_y}$. **Ambient [replacement](../../../../../axiom-schema-of-replacement.md) is used to collect the [ordinals](../../../../../ordinal-split.md) $\alpha_y$ into a [set](../../../../../set-split.md).** Their [supremum](../../../../../supremum.md), enlarged if necessary to include a stage containing $a$, gives an [ordinal](../../../../../ordinal-split.md) $\beta$ such that $a\in L_\beta$ and every $y\in S$ belongs to $L_\beta$.

Because $L_\beta$ is transitive and $a\in L_\beta$, the bounded property $y\subseteq a$ for $y\in L_\beta$ has its actual meaning when evaluated in that structure: every element of $y$ already lies in $L_\beta$, and membership is unchanged. It follows that

$$
S=\{y\in L_\beta:\langle L_\beta,\in\rangle\models y\subseteq a\}.
$$

This is a definable [subset](../../../../../subset.md) of $L_\beta$ using the parameter $a$, so $S\in\operatorname{Def}(L_\beta)=L_{\beta+1}\subseteq L$. Every member of $L$ which is a [subset](../../../../../subset.md) of $a$ is in $S$, and every member of $S$ is such a [subset](../../../../../subset.md). Therefore

$$
\boxed{\mathcal P^{L}(a)=\mathcal P^{V}(a)\cap L\in L,}
$$

which is exactly the power-set axiom in $\langle L,\in\rangle$. The [replacement](../../../../../axiom-schema-of-replacement.md) step is indispensable to this proof: definability over one stage requires first bounding all the constructible [subsets](../../../../../subset.md) by one common stage.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
