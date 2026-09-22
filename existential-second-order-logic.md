# Existential second-order logic

↑ **Parent:** [Second-order logic](second-order-logic.md)

An [existential second-order logic](existential-second-order-logic.md) sentence has the form

$$
\exists R_1\cdots\exists R_m\,\varphi,
$$

where each $R_i$ is a [second-order relation variable](second-order-relation-variable.md) of fixed finite arity $k_i$ and $\varphi$ is a [first-order sentence](first-order-sentence.md) over the input [first-order signature](first-order-signature.md) expanded by the $R_i$. The [first-order sentence](first-order-sentence.md) may contain both [universal quantification](universal-quantification.md) and [existential quantification](existential-quantification.md) over individuals; only the outer quantification over [second-order relation variables](second-order-relation-variable.md) is required to be existential. Under [full semantics for second-order logic](full-semantics-for-second-order-logic.md), truth means that some expansion by witness relations satisfies $\varphi$.

For a fixed [existential second-order logic](existential-second-order-logic.md) sentence on a domain of [cardinality](cardinality.md) $n$, the witnesses need $\sum_{i=1}^m n^{k_i}$ membership bits. The arities and the number of witnesses are constants because the sentence is fixed. After guessing those bits, a verifier evaluates the fixed [first-order sentence](first-order-sentence.md) by enumerating assignments to its finitely many individual variables, taking [polynomial time](polynomial-time.md). In the [second-order encoding of three-colorability](second-order-encoding-of-three-colorability.md), the three witnesses require $3n$ bits, and the edge constraints can be checked over at most $n^2$ ordered [vertex](vertex-graph-theory.md) pairs. This is the logical form of the [NP](np-complexity.md) principle that a positive answer has a short [complexity certificate](certificate-complexity.md).

The fixed-sentence qualification matters: it is the input [first-order structure](first-order-structure.md) that varies, rather than an arbitrarily large formula supplied with each input. [Fagin's theorem](fagin-s-theorem.md) states the converse as well: every [isomorphism](isomorphism.md)-invariant [NP](np-complexity.md) property of finite relational [first-order structures](first-order-structure.md) has such a description. The coloring example uses only unary [second-order relation variables](second-order-relation-variable.md); the general theorem allows any fixed finite arities.

**Table of contents**

- [Second-order encoding of three-colorability](second-order-encoding-of-three-colorability.md)
- [Fagin's theorem](fagin-s-theorem.md)

## ↑ Ancestors (6)

1. [Second-order logic](second-order-logic.md)
2. [Mathematical logic](mathematical-logic-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Existential second-order logic](existential-second-order-logic.md)
- [Fagin's theorem](fagin-s-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-23/7/a/solution.md)
- [Second-order encoding of three-colorability](second-order-encoding-of-three-colorability.md)
