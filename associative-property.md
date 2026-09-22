# Associative property

↑ **Parent:** [Binary operation](binary-operation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Associative_property)

The [associative property](associative-property.md) says that regrouping three [inputs](input-computer-science.md) does not change the result of a [binary operation](binary-operation.md): $(a\ast b)\ast c=a\ast(b\ast c)$ for every $a,b,c$ in its [domain of a function](domain-of-a-function.md). It changes parentheses while keeping the order of the [inputs](input-computer-science.md). [Commutativity](commutativity.md) instead exchanges two [inputs](input-computer-science.md); the two properties are different.

For [addition](addition.md) modulo three, $(2+1)+1\equiv2+(1+1)\equiv1\pmod3$. For [subtraction](subtraction.md) modulo three,

$$
(2-1)-1\equiv0,\qquad 2-(1-1)\equiv2\pmod3,
$$

so the second [binary operation](binary-operation.md) fails the [associative property](associative-property.md). One failed triple disproves [associativity](associative-property.md); checking a few successful triples does not establish it for all [inputs](input-computer-science.md).

The useful consequence is that a finite ordered sequence can be combined in chunks. For an [associative operation](associative-property.md), $(a\ast b)\ast(c\ast d)$ has the same value as $((a\ast b)\ast c)\ast d$. Intermediate results can therefore summarize parts of a computation without retaining their internal parentheses. The order must still be preserved when the [binary operation](binary-operation.md) is not [commutative](commutativity.md). [Function composition](function-composition.md) and [concatenation](concatenation.md) provide examples where grouping is harmless but exchanging entries changes the result.

**Table of contents**

- [Semigroup](semigroup.md)
  - [Numerical semigroup](numerical-semigroup.md)
  - [Rectangular band](rectangular-band.md)
    - [Cartesian closed category of rectangular bands](cartesian-closed-category-of-rectangular-bands.md)
  - [Idempotent element of a semigroup](idempotent-element-of-a-semigroup.md)
  - [Semigroup presentation](semigroup-presentation.md)
    - [Finite semigroup presentation](finite-semigroup-presentation.md)
      - [Semigroup simulation of a Turing machine](semigroup-simulation-of-a-turing-machine.md)
  - [Subsemigroup](subsemigroup.md)
  - [Monoid](monoid.md)
    - [Inverse element](inverse-element.md)
    - [Transformation monoid](transformation-monoid.md)
      - [Full transformation monoid](full-transformation-monoid.md)
    - [Monoid action](monoid-action.md)
      - [Right monoid action](right-monoid-action.md)
        - [Exponential of right monoid actions](exponential-of-right-monoid-actions.md)
          - [Exponential of right group actions](exponential-of-right-group-actions.md)
      - [Equivariant map of monoid sets](equivariant-map-of-monoid-sets.md)
      - [M-set](m-set.md)
    - [Monoid homomorphism](monoid-homomorphism.md)
    - [Monoid automorphism](monoid-automorphism.md)
    - [Free monoid](free-monoid.md)
    - [Commutative monoid](commutative-monoid.md)
      - [Free commutative monoid](free-commutative-monoid.md)
      - [Cancellative commutative monoid](cancellative-commutative-monoid.md)
        - [Congruence submonoid of the positive integers](congruence-submonoid-of-the-positive-integers.md)
          - [Nonunique factorization in a congruence submonoid](nonunique-factorization-in-a-congruence-submonoid.md)
        - [Irreducible element of a commutative monoid](irreducible-element-of-a-commutative-monoid.md)
        - [Torsion-free cancellative commutative monoid](torsion-free-cancellative-commutative-monoid.md)
      - [Category of commutative monoids](category-of-commutative-monoids.md)
  - [Additive semigroup](additive-semigroup.md)
    - [Face of an additive monoid](face-of-an-additive-monoid.md)
  - [Topological semigroup](topological-semigroup.md)
    - [Left-topological semigroup](left-topological-semigroup.md)
      - [Ellis–Numakura lemma](ellis-numakura-lemma.md)

## ↑ Ancestors (6)

1. [Binary operation](binary-operation.md)
2. [Algebraic operation](algebraic-operation-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Associative property](associative-property.md)
- [Cayley table](cayley-table.md)
- [Concatenation](concatenation.md)
- [Free monoid](free-monoid.md)
- [Function composition](function-composition.md)
- [Identity element](identity-element.md)
- [Magma (algebra)](magma-algebra.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/6/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/11/a/solution.md)
- [Semigroup](semigroup.md)
- [Transformation monoid](transformation-monoid.md)
