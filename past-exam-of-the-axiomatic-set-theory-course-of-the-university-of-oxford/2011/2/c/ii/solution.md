<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the convention that the [transitive closure](../../../../../transitive-closure.md) $\operatorname{TC}(x)$ is the least [transitive set](../../../../../transitive-set.md) containing $x$ as a subset. In [ZF](../../../../../zermelo-fraenkel-set-theory.md), [transfinite recursion](../../../../../transfinite-recursion.md) and [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) construct

$$
x_0=x,\qquad x_{n+1}=\bigcup x_n,\qquad t=\bigcup_{n<\omega}x_n.
$$

Then $x\subseteq t$. If $a\in b\in t$, some $n$ has $b\in x_n$, whence $a\in x_{n+1}\subseteq t$. Thus $t$ is transitive. If another [transitive set](../../../../../transitive-set.md) $s$ contains $x$, induction gives $x_n\subseteq s$ for every $n$, and hence $t\subseteq s$. This proves existence and uniqueness of the [transitive closure](../../../../../transitive-closure.md).

Let $W(w)$ be the [bounded definition of omega](../../../../../bounded-definition-of-omega.md) above. The displayed construction can be expressed as

$$
\exists w\,\exists f\,\exists r\,\bigl[W(w)\land f:w\to r\land\operatorname{ran}(f)=r\land f(0)=x\land\forall n\in w\,(f(n+1)=\bigcup f(n))\land y=\bigcup r\bigr].
$$

Here the brackets abbreviate a [bounded formula in set theory](../../../../../bounded-formula-in-set-theory.md): use the permitted bounded function and union predicates, bound the values of $f$ by $r$, and bound each successor index by $w$. Ordered-pair graph access is bounded; $\operatorname{ran}(f)=r$ says every value in $r$ occurs at an index in $w$. Any auxiliary sets used for the graph coding may be put in the initial existential block. Thus this is a [Sigma-one formula in set theory](../../../../../sigma-one-formula-in-set-theory.md) defining $y=\operatorname{TC}(x)$.

Denote this formula by $T(x,y)$. Existence and uniqueness give the [ZF](../../../../../zermelo-fraenkel-set-theory.md) equivalence

$$
\neg T(x,y)\iff\exists z\,(T(x,z)\land z\ne y).
$$

The right side is again $\Sigma_1$, after combining existential blocks. Consequently $T$ is a [Delta-one formula modulo ZF](../../../../../delta-one-formula-modulo-zf.md), so [Delta-one absoluteness](../../../../../delta-one-absoluteness.md) applies. Therefore **[transitive closure is Delta-one definable](../../../../../transitive-closure-is-delta-one-definable.md) and is ZF-absolute**. If closure is instead required to contain $x$ as an element, apply exactly this construction to $\{x\}$; the absoluteness conclusion is unchanged.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
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
