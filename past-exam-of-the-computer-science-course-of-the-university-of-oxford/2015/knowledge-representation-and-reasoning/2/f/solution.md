<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For plain [EL](../../../../../el.md), $\boxed{\text{every concept is satisfiable with respect to every EL TBox}}$. On a one-element domain, interpret every atomic [description logic concept](../../../../../description-logic-concept.md) as the whole domain and every [description logic role](../../../../../description-logic-role.md) as the full binary relation. A structural induction makes every [EL](../../../../../el.md) [description logic concept](../../../../../description-logic-concept.md) denote that element. Every [general concept inclusion](../../../../../general-concept-inclusion.md) is consequently true, including cyclic ones. The decision procedure can therefore always answer `yes` on well-formed inputs.

For [EL with bottom](../../../../../el-with-bottom.md), [concept satisfiability](../../../../../concept-satisfiability.md) with respect to general [TBoxes](../../../../../tbox.md) is $\boxed{\text{P-complete}}$ under the usual logarithmic-space reductions. Polynomial-time completion propagates atomic inclusions, conjunction consequences and existential requirements; deriving $\bot$ for the queried [description logic concept](../../../../../description-logic-concept.md) detects unsatisfiability. There are polynomially many such labels and normalized relationships to propagate.

For the lower bound, encode a monotone [Boolean circuit](../../../../../boolean-circuit.md) with a starting [description logic concept](../../../../../description-logic-concept.md) $S$. Give each input gate labelled one an inclusion $S\sqsubseteq G_i$. Encode an AND gate by $G_i\sqcap G_j\sqsubseteq G_k$, and an OR gate by $G_i\sqsubseteq G_k$ and $G_j\sqsubseteq G_k$. Finally add $G_{\mathrm{out}}\sqsubseteq\bot$. Then $S$ is unsatisfiable exactly when the circuit output is one. The complement version is also [P-complete](../../../../../p-completeness.md), since [P](../../../../../p-complexity.md) is closed under complement. Thus allowing $\bot$ changes a trivial satisfiability problem into a nontrivial polynomial-time one. The bottom-inclusive convention is also reflected in the [Sections 2 and 5: allowed class expressions and the complexity table for OWL 2 EL](../../../../../owl-2-web-ontology-language-profiles-second-edition.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Knowledge representation and reasoning](../../../knowledge-representation-and-reasoning-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
