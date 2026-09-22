# Henkin semantics

↑ **Parent:** [Second-order logic](second-order-logic.md)

In [Henkin semantics](henkin-semantics.md), a domain $D$ is accompanied by designated ranges $\mathcal H_k\subseteq\mathcal P(D^k)$ for [second-order relation variables](second-order-relation-variable.md) of each arity $k$. A formula $\exists R\,\varphi(R)$ searches only $\mathcal H_k$, and $\forall R\,\varphi(R)$ checks only $\mathcal H_k$. These ranges can be proper subcollections of the external [power set](power-set.md). Keeping $D$ and its input relations fixed therefore need not fix the truth of a [second-order logic](second-order-logic.md) sentence.

As a toy illustration of restricted quantification, take $D=\{a,b\}$ and unary range $\mathcal H_1=\{\varnothing,D\}$. The sentence

$$
\forall a\,\exists P\,\forall x\,(P(x)\leftrightarrow x=a)
$$

is true under [full semantics for second-order logic](full-semantics-for-second-order-logic.md), but false with this selected range, because neither singleton is available. Likewise, on the [complete graph](complete-graph.md) $K_3$, the unary range $\{\varnothing,D\}$ admits no witness for the [second-order encoding of three-colorability](second-order-encoding-of-three-colorability.md), even though a usual [proper vertex coloring](proper-vertex-coloring.md) exists. This toy range illustrates the truth definition only: it fails [second-order comprehension](second-order-comprehension.md) for the formula $x=a$, and is not a model of a system requiring that comprehension instance.

Admissible [Henkin semantics](henkin-semantics.md) for a specified deductive system must satisfy its [axioms](axiom.md), including its chosen [second-order comprehension](second-order-comprehension.md) requirements or analogous closure conditions for predicate abstraction. Closure is relative to the permitted formulas and parameters, rather than a blanket property of every selected family. In particular, on a finite domain, allowing [logical equality](logical-equality.md), individual parameters, all finite [logical disjunctions](logical-disjunction.md), and comprehension for those formulas forces every finite-arity relation to be available: enumerate its [tuples](finite-tuple.md) and disjoin the formulas naming them. Thus a proper restricted finite range cannot satisfy that entire scheme.

Treating each $\mathcal H_k$ as an additional sort, with an application relation between its members and $k$ individuals, translates this relational presentation into [first-order logic](first-order-logic.md) with several sorts. Include [axioms](axiom.md) saying that predicates with the same members are equal, together with whatever [second-order comprehension](second-order-comprehension.md) the system requires. This makes [Henkin semantics](henkin-semantics.md) useful for bringing [first-order logic](first-order-logic.md) methods to reasoning about predicates; it does not license conclusions about all external relations.

Leon Henkin's [Completeness in the Theory of Types, Journal of Symbolic Logic 15 (1950), pp. 81–91](https://www.cambridge.org/core/journals/journal-of-symbolic-logic/article/abs/completeness-in-the-theory-of-types1/551D2896D3C6F197030D3D8EEA911F1E) develops general models and proves completeness for his typed deductive system. Its opening footnote 5 explicitly discusses closure under operations associated with formula formation. Henkin later described the discovery process in his [1996 author retrospective, The Discovery of My Completeness Proofs](https://www.cambridge.org/core/journals/bulletin-of-symbolic-logic/article/abs/discovery-of-my-completeness-proofs/D414E205C8FE0F4F1DCABA9EDAD72B36); that later account is a historical recollection, distinct from the original publication.

## ↑ Ancestors (6)

1. [Second-order logic](second-order-logic.md)
2. [Mathematical logic](mathematical-logic-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Full semantics for second-order logic](full-semantics-for-second-order-logic.md)
- [Henkin semantics](henkin-semantics.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-25/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-20/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19/1/iii/solution.md)
- [Second-order comprehension](second-order-comprehension.md)
- [Second-order logic](second-order-logic.md)
- [Simple typed set theory with atoms](simple-typed-set-theory-with-atoms.md)
