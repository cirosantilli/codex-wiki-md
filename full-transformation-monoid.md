# Full transformation monoid

↑ **Parent:** [Transformation monoid](transformation-monoid.md)

The [full transformation monoid](full-transformation-monoid.md) consists of every [self-map](self-map.md) of $X$, with [function composition](function-composition.md) as its [binary operation](binary-operation.md). For $X=\{0,1\}$, there are four [functions](function-split.md): the [identity function](identity-function.md) $i$, the swap $s(0)=1,s(1)=0$, and the [constant functions](constant-function.md) $c_0(x)=0,c_1(x)=1$. Their composition order matters: $c_0\circ s=c_0$, whereas $s\circ c_0=c_1$. Thus [associativity](associative-property.md) does not imply [commutativity](commutativity.md).

<a id="image-four-self-maps-of-0-1-form-a-full-transformation-monoid"></a>
![](two-point-transformation-monoid.png)

**[Figure 2](#image-four-self-maps-of-0-1-form-a-full-transformation-monoid). Four self-maps of $\{0,1\}$ form a full transformation monoid**. The arrow diagrams show each [function](function-split.md). The [Cayley table](cayley-table.md) reads row $f$, column $g$ as $f\circ g$, applying $g$ first. Only $i$ and $s$ have [inverse elements](inverse-element.md). The [constant functions](constant-function.md) lose information and satisfy [idempotence](idempotence.md).

Only $i$ and $s$ are [bijections](bijection.md), and their [inverse elements](inverse-element.md) are themselves. They form a two-element [group](group-split.md) within this [monoid](monoid.md). The [constant functions](constant-function.md) instead satisfy $c_0\circ c_0=c_0$ and $c_1\circ c_1=c_1$, so they are [idempotent elements of a semigroup](idempotent-element-of-a-semigroup.md). Such irreversible transformations explain why the [monoid](monoid.md) setting is useful even when a [group](group-split.md) would be too restrictive.

## ↑ Ancestors (10)

1. [Transformation monoid](transformation-monoid.md)
2. [Monoid](monoid.md)
3. [Semigroup](semigroup.md)
4. [Associative property](associative-property.md)
5. [Binary operation](binary-operation.md)
6. [Algebraic operation](algebraic-operation-split.md)
7. [Algebra](algebra-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Full transformation monoid](full-transformation-monoid.md)
- [Inverse element](inverse-element.md)
- [Monoid](monoid.md)
- [Self-map](self-map.md)
