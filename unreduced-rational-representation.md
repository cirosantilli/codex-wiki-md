# Unreduced rational representation

↑ **Parent:** [Abstraction function](abstraction-function.md)

Consider an original [abstract data type](abstract-data-type.md) whose values are [rational numbers](rational-number.md). Store an [ordered pair](ordered-pair.md) $(n,d)$ of [integers](integer-split.md), interpreted as a [numerator](numerator.md) and a [denominator](denominator.md). Use exact, unbounded [integer](integer-split.md) [arithmetic](arithmetic-split.md) in this model. The storage space, [representation invariant](representation-invariant.md) and [abstraction function](abstraction-function.md) are

$$
R=\mathbb Z\times\mathbb Z,\qquad I(n,d)\iff d\ne0,\qquad R_{\mathrm{valid}}=\{(n,d)\in R:d\ne0\},\qquad \alpha:R_{\mathrm{valid}}\to\mathbb Q,\quad \alpha(n,d)=\frac nd.
$$

The [representation invariant](representation-invariant.md) does not require a positive [denominator](denominator.md) or a [reduced fraction](reduced-fraction.md). Consequently $(1,2)$, $(2,4)$ and $(-1,-2)$ are three different concrete states with the same abstract [rational number](rational-number.md) $1/2$. Similarly, $(0,1)$ and $(0,-3)$ both represent zero. The [abstraction function](abstraction-function.md) is a [surjection](surjective-function.md): every [rational number](rational-number.md) has an [integer](integer-split.md) [numerator](numerator.md) and a nonzero [integer](integer-split.md) [denominator](denominator.md), so every abstract value has a representation.

<a id="image-several-valid-integer-pairs-represent-one-rational-value-zero-denominators-have-no-abstract-value"></a>
![](rational-abstraction-concrete-state-map.png)

**[Figure 13](#image-several-valid-integer-pairs-represent-one-rational-value-zero-denominators-have-no-abstract-value). Several valid integer pairs represent one rational value; zero denominators have no abstract value**.

Both $(1,0)$ and $(0,0)$ violate the [representation invariant](representation-invariant.md); neither has a value under this [abstraction function](abstraction-function.md). By contrast, $(2,4)$ is completely valid. Simplifying it to the [reduced fraction](reduced-fraction.md) $1/2$ may be a useful implementation choice, but is not a requirement of this representation. Strengthening the [representation invariant](representation-invariant.md) to require a positive [denominator](denominator.md) and a [greatest common divisor](greatest-common-divisor.md) of one would choose a unique stored representative for each [rational number](rational-number.md); every constructor and operation would then need to establish that stronger condition.

Equality of abstract values is therefore different from equality of stored [ordered pairs](ordered-pair.md). For valid $(a,b)$ and $(c,d)$,

$$
\alpha(a,b)=\alpha(c,d)\iff ad=bc.
$$

This defines an [equivalence relation](equivalence-relation.md) on $R_{\mathrm{valid}}$: each [equivalence class](equivalence-class.md) contains all representations of one [rational number](rational-number.md). An [API](application-programming-interface.md) equality operation can compare these cross-products using exact [integer](integer-split.md) arithmetic. Comparing the two fields individually would incorrectly declare $(1,2)$ and $(2,4)$ unequal as [rational numbers](rational-number.md). The general reason is that an [abstraction function](abstraction-function.md) may map several concrete values to one abstract value.[Section 8.3.1, Abstraction Functions: several concrete values mapping to one abstract value; Section 8.3.4, Representation Invariants: valid domain of AF](ocaml-programming-correct-plus-efficient-plus-beautiful-by-michael-r-clarkson-and-others/8-3-module-documentation.md)

## ↑ Ancestors (5)

1. [Abstraction function](abstraction-function.md)
2. [Abstract data type](abstract-data-type.md)
3. [Encapsulation (computer programming)](encapsulation-computer-programming.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Abstraction function](abstraction-function.md)
- [Correct operations through an abstraction function](correct-operations-through-an-abstraction-function.md)
