<h1 id="b/6/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume a nonempty set $a$ has no membership-minimal element, so for every $x\in a$ there is $y\in x\cap a$. Consider the formula $\varphi(x)\equiv x\notin a$.

It is progressive: if every element of $x$ is outside $a$ but $x\in a$, the assumed absence of a minimal element supplies $y\in x\cap a$, contradicting that hypothesis. The [membership induction theorem](../../../../../../membership-induction-theorem.md) therefore implies $x\notin a$ for every set $x$. This contradicts $a\ne\varnothing$.

Thus every nonempty set $a$ contains an element $x$ with $x\cap a=\varnothing$, exactly the [Axiom of foundation](../../../../../../axiom-of-regularity.md):

$$
\boxed{a\ne\varnothing\ \Longrightarrow\ \exists x\in a\ (x\cap a=\varnothing).}
$$

Only the induction schema and elementary set reasoning were needed; no prior use of [Axiom of foundation](../../../../../../axiom-of-regularity.md) occurs in the proof.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [6](../../../6.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../../split.md)
7. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
