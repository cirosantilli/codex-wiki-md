# Second-order logic

↑ **Parent:** [Mathematical logic](mathematical-logic-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second-order_logic)

[Second-order logic](second-order-logic.md) extends [first-order logic](first-order-logic.md) by allowing [existential quantification](existential-quantification.md) and [universal quantification](universal-quantification.md) over [second-order relation variables](second-order-relation-variable.md), as well as over individual objects. In the relational presentation used here, an individual variable $x$ ranges over a domain $D$, while a [second-order relation variable](second-order-relation-variable.md) $R$ of arity $k$ denotes a [subset](subset.md) of $D^k$. Unary [second-order relation variables](second-order-relation-variable.md) denote [subsets](subset.md) of $D$; binary ones denote [binary relations](binary-relation.md). Presentations with [function](function-split.md) variables can instead describe their graphs by [second-order relation variables](second-order-relation-variable.md), with [first-order formulas](first-order-formula.md) requiring a unique output for every input.

For a [graph](graph-split.md) with [vertices](vertex-graph-theory.md) $D$ and fixed [graph adjacency](graph-adjacency.md) $E$, the [first-order sentence](first-order-sentence.md) $\forall x\,\exists y\,E(x,y)$ says that every [vertex](vertex-graph-theory.md) has a neighbour. It selects individual [vertices](vertex-graph-theory.md) while $E$ retains its given interpretation. By contrast,

$$
\exists P\,\bigl(\exists x\,P(x)\ \land\ \forall x\forall y\,((P(x)\land P(y))\to\neg E(x,y))\bigr)
$$

selects an entire [subset](subset.md) $P$ and says that it is a nonempty [independent set](independent-set-graph-theory.md). Here $P$ is a unary [second-order relation variable](second-order-relation-variable.md), rather than a symbol in the input [first-order signature](first-order-signature.md). This particular property also has a simple [first-order sentence](first-order-sentence.md) on [simple graphs](simple-graph.md); the example illustrates the change in what can be selected, rather than proving a separation in expressive power.

The usefulness of [second-order logic](second-order-logic.md) is that one can describe a whole proposed solution, such as a [graph coloring](graph-coloring.md), and then impose local constraints on it. Syntax alone does not specify which proposed relations are available: [full semantics for second-order logic](full-semantics-for-second-order-logic.md) permits all external [subsets](subset.md) of $D^k$, whereas [Henkin semantics](henkin-semantics.md) supplies designated ranges. The [second-order encoding of three-colorability](second-order-encoding-of-three-colorability.md) makes this distinction concrete.

**Table of contents**

- [Second-order relation variable](second-order-relation-variable.md)
- [Existential second-order logic](existential-second-order-logic.md)
  - [Second-order encoding of three-colorability](second-order-encoding-of-three-colorability.md)
  - [Fagin's theorem](fagin-s-theorem.md)
- [Henkin semantics](henkin-semantics.md)
- [Full semantics for second-order logic](full-semantics-for-second-order-logic.md)
- [Second-order comprehension](second-order-comprehension.md)

## ↑ Ancestors (5)

1. [Mathematical logic](mathematical-logic-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Fagin's theorem](fagin-s-theorem.md)
- [Full semantics for second-order logic](full-semantics-for-second-order-logic.md)
- [Henkin semantics](henkin-semantics.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-23/7/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-23/7/c/solution.md)
- [PSPACE](pspace.md)
- [Second-order logic](second-order-logic.md)
