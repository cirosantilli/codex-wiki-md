# Function collision

↑ **Parent:** [Function](function-split.md)

A function collision is a pair of distinct inputs $x\neq x'$ with $f(x)=f(x')$. An [injective function](injective-function.md) has no collisions. For a two-to-one function every nonempty [fiber](fiber-of-a-function.md) has two elements and hence one unordered collision pair. Finding such a pair through an oracle is the task of [quantum collision finding](quantum-collision-finding.md).

In the finite example under [image and preimage of a function](image-and-preimage-of-a-function.md), the pair $\{a,b\}$ is a [function collision](function-collision.md): both inputs give zero. The [function](function-split.md) retains their shared output but loses the distinction between them. If a [finite set](finite-set.md) has more inputs than the number of available outputs, the [pigeonhole principle](pigeonhole-principle.md) forces a [function collision](function-collision.md). Equal source and target [cardinalities](cardinality.md) alone do not prevent one.

For a finite [function](function-split.md), let $m_y$ be the [cardinality](cardinality.md) of its [fiber of a function](fiber-of-a-function.md) over $y$. The number of unordered [function collisions](function-collision.md) is $\sum_y\binom{m_y}{2}$, because each pair must lie in one common [fiber](fiber-of-a-function.md). The example's nonempty fiber sizes are $2,1,1$, giving exactly one collision pair.

## ↑ Ancestors (6)

1. [Function](function-split.md)
2. [Set theory](set-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Brassard–Høyer–Tapp collision algorithm](brassard-hoyer-tapp-collision-algorithm.md)
- [Function collision](function-collision.md)
- [Hash collision](hash-collision.md)
- [Image of a function](image-of-a-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/2/b/solution.md)
