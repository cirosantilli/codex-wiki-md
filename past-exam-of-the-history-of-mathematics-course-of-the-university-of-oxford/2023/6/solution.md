<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

[Heinrich Weber](../../../heinrich-martin-weber.md)'s 1882 paper concerns [prime numbers](../../../prime-number-split.md) represented by [quadratic forms](../../../quadratic-form-split.md). Its [definition](../../../definition-mathematics.md) abstracts a [finite group](../../../finite-group.md) from the nature of its elements: what matters is a closed [binary operation](../../../binary-operation.md), [associativity](../../../associative-property.md), and left and right [cancellation laws](../../../cancellation-law.md). Here degree $h$ means the number of elements, now called the [group order](../../../order-of-a-finite-group.md); it is not the number of letters acted on by a [permutation group](../../../permutation-group.md). This matters when relating the passage to earlier work on substitutions. The [definition](../../../definition-mathematics.md) fits the use of [groups](../../../group-split.md) of classes of [quadratic forms](../../../quadratic-form-split.md), where the elements are already mathematical objects more elaborate than individual permutations.[Mathematische Annalen 20 (1882), 301–329; opening group definition as reproduced in the exam](../../../beweis-des-satzes-dass-jede-eigentlich-primitive-quadratische-form-unendlich-viele-primzahlen-darzustellen-fahig-ist-by-heinrich-weber.md)[Discussion of Weber's 1882 definition and its class-group setting](../../../the-abstract-group-concept-by-the-mactutor-history-of-mathematics-archive.md)

The apparent omission of an [identity element](../../../identity-element.md) and [inverse elements](../../../inverse-element.md) is not fatal. **Every nonempty [finite cancellative semigroup](../../../finite-cancellative-semigroup.md) is a [group](../../../group-split.md).** Here is a proof identifying exactly where the assumption of a [finite set](../../../finite-set.md) enters. For fixed $a\in G$, the [maps](../../../function-class.md) $L_a(x)=ax$ and $R_a(x)=xa$ are [injective](../../../injective-function.md) by cancellation. An [injective function](../../../injective-function.md) from a [finite set](../../../finite-set.md) to itself is [surjective](../../../surjective-function.md), so choose $e$ with $ae=a$. For every $x$,

$$
a(ex)=(ae)x=ax,
$$

and left cancellation gives $ex=x$. To show $e$ is also a right [identity element](../../../identity-element.md), use

$$
(xe)x=x(ex)=xx.
$$

Right cancellation gives $xe=x$. Thus the same $e$ works on both sides for every $x$; it has not merely been chosen as an element fixing $a$.

[Surjectivity](../../../surjective-function.md) now gives $b,c$ with $ab=e$ and $ca=e$. By [associativity](../../../associative-property.md),

$$
c=ce=c(ab)=(ca)b=eb=b.
$$

So $b$ is a two-sided [inverse element](../../../inverse-element.md) of $a$. Since $a$ was arbitrary, the usual [group axioms](../../../group-axioms.md) follow. The nonempty hypothesis is tacit in a system of $h$ elements intended to have positive $h$: the empty system would satisfy the displayed universal conditions vacuously but would have no [identity element](../../../identity-element.md).

The infinite case exposes the force of the qualification. The positive [integers](../../../integer-split.md) under [addition](../../../addition.md) are closed, associative and cancellative, but have no additive [identity element](../../../identity-element.md). Even the nonnegative [integers](../../../integer-split.md) have an [identity element](../../../identity-element.md) without additive [inverse elements](../../../inverse-element.md) for positive elements. The failure is precisely that [injective functions](../../../injective-function.md) of an infinite [set](../../../set-split.md) to itself need not be [surjective](../../../surjective-function.md). [Heinrich Weber](../../../heinrich-martin-weber.md)'s conditions are therefore not an unrestricted replacement for the modern [group axioms](../../../group-axioms.md).

Historically the abstraction is important because it allows arguments to be applied across different kinds of elements. An assumption of [commutativity](../../../commutativity.md) is absent: class-group applications do not make commutativity part of the general [definition](../../../definition-mathematics.md). For example, the [symmetric group](../../../symmetric-group.md) $S_3$ meets the conditions but is [noncommutative](../../../noncommutativity.md). The [definition](../../../definition-mathematics.md) also does not require a prior presentation as permutations, although [Cayley's theorem](../../../cayley-s-theorem.md) provides such a representation. The passage documents **the separation of an algebraic structure from any one representation of it**, with [finiteness](../../../finiteness.md) carrying logical work that later axiom systems usually assign to explicit [identity element](../../../identity-element.md) and [inverse element](../../../inverse-element.md) axioms.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2023](../../2023-split.md)
3. [Past exam of the history of mathematics course of the University of Oxford](../../split.md)
4. [History of mathematics course of the University of Oxford](../../../history-of-mathematics-course-of-the-university-of-oxford.md)
5. [Year 3 of the mathematics course of the University of Oxford](../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
