<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $x\in V_\delta$. Since $\delta$ is a [limit ordinal](../../../../limit-ordinal.md), choose $\beta<\delta$ with $x\in V_\beta$. Transitivity gives $x\subseteq V_\beta$. Every subset $u\subseteq x$ therefore belongs to $V_{\beta+1}=\mathcal P(V_\beta)$, and consequently

$$
\mathcal P(x)\subseteq V_{\beta+1},\qquad\mathcal P(x)\in V_{\beta+2}\subseteq V_\delta.
$$

The last inclusion uses $\beta+2<\delta$, since a finite number of successor steps remains below a [limit ordinal](../../../../limit-ordinal.md). In particular every subset of $x$ is also an element of the [transitive set](../../../../transitive-set.md) $V_\delta$.

Take $y=\mathcal P(x)$. For any $u\in V_\delta$, transitivity ensures that the internal statement $u\subseteq x$ agrees with the external one. Hence

$$
(V_\delta,\in)\models\forall u\,(u\in y\leftrightarrow u\subseteq x).
$$

Such a $y\in V_\delta$ exists for every $x\in V_\delta$, so **$(V_\delta,\in)$ satisfies the [Axiom of power set](../../../../axiom-of-power-set.md)**. This [power-set axiom at limit ranks](../../../../power-set-axiom-at-limit-ranks.md) actually holds for every nonzero [limit ordinal](../../../../limit-ordinal.md); the stated restriction $\delta>\omega$ is sufficient.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the axiomatic set theory course of the University of Oxford](../../../split.md)
5. [Axiomatic set theory course of the University of Oxford](../../../../axiomatic-set-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
