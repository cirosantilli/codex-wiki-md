<h1 id="b/6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

To prove that [power-set equality is not upward absolute](../../../../../power-set-equality-is-not-upward-absolute.md), use the standard [constructible universe theorem](../../../../../constructible-universe-theorem.md): $L$ is a transitive [inner model](../../../../../inner-model.md) of [ZF](../../../../../zermelo-fraenkel-set-theory.md) containing every [ordinal](../../../../../ordinal-split.md), and [set](../../../../../set-split.md) rank is absolute between $L$ and $V$. Since $V\ne L$, some rank stage contains a nonconstructible [set](../../../../../set-split.md). Let $\alpha$ be the least [ordinal](../../../../../ordinal-split.md) with $V_\alpha\nsubseteq L$. It is not zero; it cannot be a limit, since a [union](../../../../../set-union.md) of earlier stages contained in $L$ is still contained in $L$. Thus $\alpha=\beta+1$ and $V_\beta\subseteq L$.

We need not merely this inclusion, but that $y=V_\beta$ itself belongs to $L$. Inside $L$, [ZF](../../../../../zermelo-fraenkel-set-theory.md) constructs its own rank stage $(V_\beta)^L$, which is a [set](../../../../../set-split.md) of $L$. By transitivity and [rank absoluteness](../../../../../set-theoretic-absoluteness.md),

$$
(V_\beta)^L=V_\beta\cap L=V_\beta.
$$

Consequently $y\in L$. Let $x=(\mathcal P(y))^L$, the [power set](../../../../../power-set.md) computed in $L$. Then $x\in L$ and $L\models x=\mathcal P(y)$.

By minimality there is $z\in V_{\beta+1}\setminus L$. Externally $z\subseteq V_\beta=y$, but $z\notin x$, because every member of the [set](../../../../../set-split.md) $x\in L$ is in the [transitive class](../../../../../transitive-class.md) $L$. Hence $V\not\models x=\mathcal P(y)$. Taking $U_1=L$ and $U_2=V$ proves **[power-set equality is not upward absolute](../../../../../power-set-equality-is-not-upward-absolute.md), even between transitive models of [ZF](../../../../../zermelo-fraenkel-set-theory.md)**.

There is no contradiction with absoluteness of $z\subseteq y$: that bounded relation agrees whenever both parameters are present in the smaller class. [Power-set equality](../../../../../power-set-equality-is-not-upward-absolute.md) quantifies over all [subsets](../../../../../subset.md), including a new $z$ absent from the smaller class. The step proving $V_\beta\in L$ is essential; inclusion in a class alone would not imply membership in it.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
