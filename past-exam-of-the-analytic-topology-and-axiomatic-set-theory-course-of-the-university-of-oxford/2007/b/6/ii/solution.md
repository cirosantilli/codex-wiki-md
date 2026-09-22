<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The membership induction principle is the schema

$$
\boxed{\bigl[\forall x\bigl((\forall y\in x\ \varphi(y))\Rightarrow\varphi(x)\bigr)\bigr]\Longrightarrow\forall x\ \varphi(x),}
$$

allowing fixed parameters in $\varphi$.

Suppose the progressiveness hypothesis holds but $\neg\varphi(a)$. The [transitive set](../../../../../transitive-set.md) $T=\operatorname{TC}(\{a\})$ contains $a$. [Separation](../../../../../axiom-schema-of-specification.md) gives the nonempty set $B=\{x\in T:\neg\varphi(x)\}$. By [Foundation](../../../../../axiom-of-regularity.md) choose $b\in B$ with $b\cap B=\varnothing$. Every $y\in b$ belongs to $T$ because it is a [transitive set](../../../../../transitive-set.md) and cannot belong to $B$, so every such $y$ satisfies $\varphi$. Progressiveness now gives $\varphi(b)$, a contradiction. Thus the principle holds. The [transitive closure](../../../../../transitive-closure.md) is needed to turn a possibly proper class of counterexamples into a set to which [Foundation](../../../../../axiom-of-regularity.md) applies.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
