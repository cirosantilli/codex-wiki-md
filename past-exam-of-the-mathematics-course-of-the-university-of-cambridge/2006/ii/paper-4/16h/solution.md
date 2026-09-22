<h1 id="16h/solution">Solution</h1>

↑ **Parent:** [16H](../16h.md)

A relation $r$ on a set $a$ is a [well-founded relation](../../../../../well-founded-relation.md) when every nonempty subset $b\subseteq a$ contains an element $y$ with no $x\in b$ satisfying $x\,r\,y$. The [well-founded recursion](../../../../../well-founded-recursion.md) theorem states that a rule assigning a value at $y$ from the already assigned values at its predecessors determines a unique function on $a$; the rule must give a unique set-valued output for every possible predecessor assignment. No choice or transitivity of $r$ is needed.

Apply recursion with

$$
f(y)=\sup\{f(x)+1:x\,r\,y\}.
$$

The empty supremum is zero. [Well-founded induction](../../../../../well-founded-induction.md) makes every value an [ordinal](../../../../../ordinal.md); the [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) collects the values into a set. Choose an [ordinal](../../../../../ordinal.md) $\alpha$ larger than every value. Then $f:a\to\alpha$, and $x\,r\,y$ implies $f(x)+1\le f(y)$, hence $f(x)<f(y)$.

Conversely, suppose such an ordinal-valued function exists. In any nonempty $b\subseteq a$, choose $y\in b$ whose value is the least [ordinal](../../../../../ordinal.md) in $f[b]$. There can be no $x\in b$ with $x\,r\,y$, because it would have smaller value. Thus $r$ is well-founded, proving the equivalence.

Using the [axiom of choice](../../../../../axiom-of-choice.md), fix a [well-order](../../../../../well-order.md) $\prec$ of $a$. Order its elements lexicographically by $(f(x),x)$: first compare the [ordinal](../../../../../ordinal.md) rank, and for equal ranks use $\prec$. Every nonempty subset has a smallest rank and then a least element in that rank fibre, so this is a [well-order](../../../../../well-order.md). Since $x\,r\,y$ strictly increases rank, it respects every original relation pair. Hence **every [well-founded relation](../../../../../well-founded-relation.md) extends to a [well-order](../../../../../well-order.md) under choice**.

## ↑ Ancestors (10)

1. [16H](../16h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
