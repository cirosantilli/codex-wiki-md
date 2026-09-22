# Full semantics for second-order logic

↑ **Parent:** [Second-order logic](second-order-logic.md)

Under [full semantics for second-order logic](full-semantics-for-second-order-logic.md), a [second-order relation variable](second-order-relation-variable.md) of arity $k$ ranges over exactly $\mathcal P(D^k)$, the external [power set](power-set.md) of the appropriate [Cartesian product](cartesian-product.md). Thus

$$
\exists R\,\varphi(R)\quad\text{means}\quad
\text{some }S\subseteq D^k\text{ satisfies }\varphi(S),
$$

and [universal quantification](universal-quantification.md) over $R$ checks every such [subset](subset.md). Here the [power set](power-set.md) is taken in the ambient mathematical universe, not merely among relations definable by formulas or represented by objects inside $D$.

For $D=\{a,b,c\}$, a unary [second-order relation variable](second-order-relation-variable.md) has eight possible values, including the three singletons needed by the [second-order encoding of three-colorability](second-order-encoding-of-three-colorability.md). The three unary witnesses can range independently over those eight [subsets](subset.md), giving $8^3=512$ candidate triples before the [first-order sentence](first-order-sentence.md) is checked; only six triples pass for the [complete graph](complete-graph.md) $K_3$. For $K_4$, there are $16^3=4096$ candidate triples and none passes. Distinguishing the range of candidates from the constraints on valid witnesses clarifies both [full semantics for second-order logic](full-semantics-for-second-order-logic.md) and the verifier view of [NP](np-complexity.md).

The appeal of [full semantics for second-order logic](full-semantics-for-second-order-logic.md) is its literal reading of assertions about every [subset](subset.md) or every relation. A [first-order structure](first-order-structure.md) fixes the second-order ranges automatically, in contrast to [Henkin semantics](henkin-semantics.md). That expressive force comes with a limitation: there is no effective, sound deductive system complete for all valid [second-order logic](second-order-logic.md) sentences under [full semantics for second-order logic](full-semantics-for-second-order-logic.md). This limitation and the change of intended models motivating [Henkin semantics](henkin-semantics.md) are described at the start of [Henkin's 1950 paper](https://www.cambridge.org/core/journals/journal-of-symbolic-logic/article/abs/completeness-in-the-theory-of-types1/551D2896D3C6F197030D3D8EEA911F1E).

For a domain $V_\lambda$, an external functional graph with all its individual [ordered pairs](ordered-pair.md) in $V_\lambda$ is therefore available, even if the whole graph does not belong to $V_\lambda$. More generally, a binary [second-order relation variable](second-order-relation-variable.md) can denote any external [subset](subset.md) of $V_\lambda\times V_\lambda$; its [ordered pairs](ordered-pair.md) need not themselves be elements of the individual domain. Having endpoints in the domain is what matters. This distinction between internal objects and externally available relations is essential when applying [second-order logic](second-order-logic.md) to the [cumulative hierarchy](cumulative-hierarchy.md).

## ↑ Ancestors (6)

1. [Second-order logic](second-order-logic.md)
2. [Mathematical logic](mathematical-logic-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Existential second-order logic](existential-second-order-logic.md)
- [Fagin's theorem](fagin-s-theorem.md)
- [Full second-order replacement rank obstruction](full-second-order-replacement-rank-obstruction.md)
- [Full semantics for second-order logic](full-semantics-for-second-order-logic.md)
- [Henkin semantics](henkin-semantics.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19/1/iii/solution.md)
- [Second-order comprehension](second-order-comprehension.md)
- [Second-order logic](second-order-logic.md)
- [Second-order relation variable](second-order-relation-variable.md)
