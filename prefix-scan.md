# Prefix scan

↑ **Parent:** [Prefix sum](prefix-sum.md)

A prefix scan computes successive accumulated results for an [associative operation](associative-property.md) $\oplus$ while keeping input order fixed. A scan based on [addition](addition.md) produces [prefix sums](prefix-sum.md); one based on [matrix multiplication](matrix-multiplication.md) produces successive ordered matrix products. [Associativity](associative-property.md) allows regrouping, while [commutativity](commutativity.md) is unnecessary because the order stays fixed. If an initial empty prefix is included, its value is the [identity element](identity-element.md) for the chosen operation.

The ability to compute accumulated results does not by itself allow subtraction of two prefixes. For example, two accumulated minima cannot reveal a block minimum: the lists $(1,7,8)$ and $(1,2,3)$ both have successive minima $(1,1,1)$, but the minimum of positions two through three is seven for one and two for the other. Prefix sums support block recovery because [addition](addition.md) has [additive inverses](additive-inverse.md); an arbitrary [associative operation](associative-property.md) need not have that property.

## ↑ Ancestors (8)

1. [Prefix sum](prefix-sum.md)
2. [Sum](sum.md)
3. [Summation](summation.md)
4. [Addition](addition.md)
5. [Arithmetic](arithmetic-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Prefix sum](prefix-sum.md)
