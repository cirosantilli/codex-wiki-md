<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the [Kuratowski ordered pair](../../../../kuratowski-ordered-pair.md)

$$
\boxed{\langle x,y\rangle=\{\{x\},\{x,y\}\}.}
$$

The [axiom of pairing](../../../../axiom-of-pairing.md) first constructs $\{x\}$ and $\{x,y\}$, then constructs the displayed [pair](../../../../pair.md) of those [sets](../../../../set-split.md), proving that it is a [set](../../../../set-split.md).

For any $a,b$, the [intersection](../../../../set-intersection.md) of the members of this [pair](../../../../pair.md) is $\{a\}$, and their [union](../../../../set-union.md) is $\{a,b\}$. Thus equality of two [ordered pairs](../../../../ordered-pair.md) first gives $\{a\}=\{c\}$, hence $a=c$, and then $\{a,b\}=\{a,d\}$. If $b=a$, this latter [set](../../../../set-split.md) is a [singleton](../../../../singleton-mathematics.md) and forces $d=a$. If $b\ne a$, its unique member distinct from $a$ is $b$, forcing $d=b$. Hence equality of [ordered pairs](../../../../ordered-pair.md) gives equality of both coordinates.

For a [set](../../../../set-split.md) $R$ of [ordered pairs](../../../../ordered-pair.md), both coordinates of every [pair](../../../../pair.md) belong to

$$
U=\bigcup\bigcup R,
$$

which is a [set](../../../../set-split.md) by two applications of the [Axiom of union](../../../../axiom-of-union.md). [Axiom of separation](../../../../axiom-schema-of-specification.md) inside $U$ gives

$$
\operatorname{dom}R=\{x\in U:\exists y\,\langle x,y\rangle\in R\},\qquad
\operatorname{ran}R=\{y\in U:\exists x\,\langle x,y\rangle\in R\}.
$$

These are [sets](../../../../set-split.md), including when $R$ is empty.

The [Axiom of foundation](../../../../axiom-of-regularity.md) asserts that every nonempty [set](../../../../set-split.md) $A$ has an element $a$ with $a\cap A=\varnothing$. If a [descending membership sequence](../../../../descending-membership-sequence.md) $f:\omega\to V$ existed, [replacement](../../../../axiom-schema-of-replacement.md) would give the nonempty range [set](../../../../set-split.md) $S=\{f(n):n\in\omega\}$. [Foundation](../../../../axiom-of-regularity.md) would give some $f(n)$ disjoint from $S$. But $f(n^+)\in f(n)$ and $f(n^+)\in S$, contradicting that disjointness. Thus [foundation](../../../../axiom-of-regularity.md) rules out every such [sequence](../../../../sequence.md).

Conversely suppose there is no [descending membership sequence](../../../../descending-membership-sequence.md), but [foundation](../../../../axiom-of-regularity.md) fails. There is then a nonempty [set](../../../../set-split.md) $A$ such that $a\cap A\ne\varnothing$ for every $a\in A$. The [axiom of choice](../../../../axiom-of-choice.md) selects a [function](../../../../function-split.md) $h$ on $A$ with $h(a)\in a\cap A$. Choose $a_0\in A$ and use [recursion](../../../../recursion-computer-science.md) to define

$$
f(0)=a_0,\qquad f(n^+)=h(f(n)).
$$

Every value remains in $A$, and $f(n^+)\in f(n)$ for every $n$. This is the forbidden [sequence](../../../../sequence.md). Therefore, with the stated [choice](../../../../axiom-of-choice.md) assumption, **[foundation](../../../../axiom-of-regularity.md) is equivalent to the absence of [descending membership sequences](../../../../descending-membership-sequence.md)**. The selection step explains exactly where [choice](../../../../axiom-of-choice.md) is used; [dependent choice](../../../../axiom-of-dependent-choice.md) would suffice.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the logic and set theory course of the University of Oxford](../../../split.md)
5. [Logic and set theory course of the University of Oxford](../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
