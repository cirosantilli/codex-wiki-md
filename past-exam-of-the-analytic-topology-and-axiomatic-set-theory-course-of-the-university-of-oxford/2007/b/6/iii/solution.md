<h1 id="b/6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

An $\in$-[isomorphism](../../../../../isomorphism.md) is a [bijection](../../../../../bijection.md) $f:X\to Y$ such that $x\in x'$ if and only if $f(x)\in f(x')$ for all $x,x'\in X$. When $Y$ is transitive, [surjectivity](../../../../../surjective-function.md) gives the stronger recursive description

$$
f(x)=\{f(u):u\in x\cap X\}\qquad(x\in X).
$$

Indeed every member of $f(x)$ belongs to $Y$ because it is a [transitive set](../../../../../transitive-set.md) and so has a preimage in $X$; the [isomorphism](../../../../../isomorphism.md) property identifies exactly which preimages occur.

If $f,g$ are two such maps, possibly to different [transitive sets](../../../../../transitive-set.md), form $B=\{x\in X:f(x)\ne g(x)\}$. If $B$ were nonempty, [Foundation](../../../../../axiom-of-regularity.md) would give $x\in B$ with $x\cap B=\varnothing$. All predecessors $u\in x\cap X$ then satisfy $f(u)=g(u)$, and the recursive descriptions force $f(x)=g(x)$, a contradiction. Therefore **the map and its transitive range are unique**.

The necessary and sufficient condition is that $\langle X,\in\rangle$ be **[well-founded](../../../../../well-founded-relation.md) and extensional as a relation on $X$**. Well-foundedness says every nonempty $A\subseteq X$ has a member with no $\in$-predecessor in $A$. The [extensional relation](../../../../../extensional-relation.md) condition says distinct elements $x,x'\in X$ have distinct predecessor sets $x\cap X$, $x'\cap X$. Sufficiency is the [Mostowski collapse theorem](../../../../../mostowski-collapse-theorem.md).

For necessity, an [isomorphism](../../../../../isomorphism.md) transfers well-foundedness from its transitive range, where [Foundation](../../../../../axiom-of-regularity.md) applies. For extensionality, if $x\cap X=x'\cap X$, the recursive descriptions give $f(x)=f(x')$, and [injectivity](../../../../../injective-function.md) gives $x=x'$. Notice that ambient [axiom of extensionality](../../../../../axiom-of-extensionality.md) alone does not establish this internal predecessor condition; for example $X=\{\{0\},\{2\}\}$ can have distinct elements with no predecessors in $X$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
