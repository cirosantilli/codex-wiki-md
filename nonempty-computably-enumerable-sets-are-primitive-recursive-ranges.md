# Nonempty computably enumerable sets are primitive recursive ranges

↑ **Parent:** [Recursively enumerable set](recursively-enumerable-set.md)

Every nonempty [computably enumerable set](recursively-enumerable-set.md) $X\subseteq\mathbb N$ is the range of a [primitive recursive function](primitive-recursive-function.md) $f:\mathbb N\to\mathbb N$. Choose $x_0\in X$, decode $n=\langle x,t\rangle$ using a [primitive recursive pairing function](primitive-recursive-pairing-function.md), and output $x$ if the recognizing machine halts within $t$ steps, or $x_0$ otherwise. The [bounded halting predicate](bounded-halting-predicate.md) makes this function [primitive recursive](primitive-recursive-function.md), and every member of $X$ occurs for a sufficiently large bound. The [empty set](empty-set.md) is excluded because such a function is total.

## ↑ Ancestors (6)

1. [Recursively enumerable set](recursively-enumerable-set.md)
2. [Computability theory](computability-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
