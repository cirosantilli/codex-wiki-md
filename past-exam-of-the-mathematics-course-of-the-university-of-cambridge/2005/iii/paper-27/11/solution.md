<h1 id="11/solution">Solution</h1>

↑ **Parent:** [11](../11.md)

Interpret the assertion in the usual well-founded, class-theoretic version of [Zermelo set theory](../../../../../zermelo-set-theory.md), including [foundation](../../../../../axiom-of-regularity.md), class comprehension and separation with class parameters. Classes are not extra sets. The [axiom of limitation of size](../../../../../axiom-of-limitation-of-size.md), in the form used here, says that every proper class is in bijection with the universe $V$.

First derive [replacement](../../../../../axiom-schema-of-replacement.md). Let a functional class relation map a set $a$ onto its image class $B$. If $B$ were proper, the limitation axiom would give a bijection $h:B\to V$. Its composite with the original map would be a surjection $g:a\to V$. Class-parameter [separation](../../../../../axiom-schema-of-specification.md) forms

$$
D=\{x\in a:x\notin g(x)\}.
$$

Surjectivity gives $d\in a$ with $g(d)=D$, whence $d\in D$ iff $d\notin D$, a contradiction. Thus $B$ is a set, proving each instance of replacement. The argument also gives class replacement when the functional class is a parameter.

The class $\mathrm{On}$ of [ordinals](../../../../../ordinal.md) is proper: were it a set, its union and successor would be ordinals larger than every ordinal in it. Limitation gives a bijection $e:\mathrm{On}\to V$. Ordering $V$ by the ordinal indices of $e$ gives a global well-order; each nonempty set has a member with least index. Choosing that member defines [global choice](../../../../../axiom-of-global-choice.md).

Conversely assume replacement and global choice. Ordinary choice well-orders each rank segment, and global choice selects such a well-order uniformly, since the collection of well-orders of each fixed rank segment is a nonempty set. Order all sets first by their [rank of a set](../../../../../rank-of-a-set.md) and then by the selected order within that rank. The resulting global order is set-like: the predecessors of any element are contained in a rank segment and form a set. Restrict it to a proper class $A$. By [transfinite recursion](../../../../../transfinite-recursion.md), enumerate $A$ in this order. It cannot be exhausted at a set ordinal, since [replacement](../../../../../axiom-schema-of-replacement.md) would then make $A$ a set. Every member appears, because its predecessors form a set, whose well-order has an ordinal order type. Hence $A$ has order type $\mathrm{On}$. The same applies to $V$, and composing the two enumerations gives a bijection $A\cong V$. Thus **limitation of size is equivalent to replacement plus global choice** in this class-theoretic setting.

## ↑ Ancestors (10)

1. [11](../11.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
