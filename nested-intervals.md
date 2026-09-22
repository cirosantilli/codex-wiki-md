# Nested intervals

↑ **Parent:** [Interval (mathematics)](interval-mathematics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nested_intervals)

A sequence of [nested intervals](nested-intervals.md) keeps every new enclosure inside the previous one:

$$
I_1\supseteq I_2\supseteq I_3\supseteq\cdots.
$$

Each step adds a restriction without discarding an earlier restriction. This is useful when an exact [real number](real-number.md) is described by increasingly precise bounds rather than by a finite decimal expansion. The [bisection method](bisection-method.md), for instance, produces [nested intervals](nested-intervals.md) that keep enclosing a [zero of a function](zero-of-a-function.md).

For a simple example, the [closed intervals](closed-real-interval.md) $I_n=[1-1/n,1+1/n]$ are nested and all contain $1$. Their lengths $2/n$ tend to zero, so the [nested interval theorem](nested-interval-theorem.md) leaves exactly that point. The family $J_n=[1-1/n,2+1/n]$ is also nested, but its intersection is the whole [closed interval](closed-real-interval.md) $[1,2]$. Nesting alone does not force uniqueness.

The [open intervals](open-interval.md) $K_n=(0,1/n)$ illustrate a different possibility. Every finite collection has a nonempty intersection, but the intersection of all of them is empty: any positive candidate eventually exceeds $1/n$, and zero is excluded from every member. Each finite row in the diagram contains points; the full infinite family need not.

**Table of contents**

- [Nested interval theorem](nested-interval-theorem.md)

## ↑ Ancestors (7)

1. [Interval (mathematics)](interval-mathematics.md)
2. [Real line](real-line.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Nested-bracket proof of the intermediate value theorem](nested-bracket-proof-of-the-intermediate-value-theorem.md)
- [Nested intervals](nested-intervals.md)
