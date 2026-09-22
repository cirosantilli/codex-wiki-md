<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

A fragment has the [finite model property](../../../../../finite-model-property.md) if $\boxed{\text{every satisfiable sentence in the fragment has a finite model}}$. This does not mean that every model is finite, nor that there is one uniform bound on model size for the entire fragment.

[ALC](../../../../../alc.md) has the [finite model property](../../../../../finite-model-property.md), including satisfiability with respect to finite [TBoxes](../../../../../tbox.md). A [tableau algorithm for ALC](../../../../../tableau-algorithm-for-alc.md) uses finitely many possible labels and [direct blocking in description logic](../../../../../direct-blocking-in-description-logic.md) to obtain a finite representation of a model. The resulting finite-model claim is a property of the logic; termination alone, for an arbitrary procedure, would not establish it.

Full [first-order logic](../../../../../first-order-logic.md) does not have the [finite model property](../../../../../finite-model-property.md). For example, the [first-order sentence](../../../../../first-order-sentence.md)

$$
\bigl(\forall x\,\neg R(x,x)\bigr)\land
\bigl(\forall x\forall y\forall z\,((R(x,y)\land R(y,z))\to R(x,z))\bigr)\land
\bigl(\forall x\exists y\,R(x,y)\bigr)
$$

requires an irreflexive transitive relation with a successor for every element. It is satisfied by the usual strict order on the [natural numbers](../../../../../natural-number.md). In a nonempty finite domain, repeatedly taking successors eventually repeats an element; transitivity would then force $R(x,x)$, contradicting irreflexivity. Hence this satisfiable [first-order sentence](../../../../../first-order-sentence.md) has no finite model.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Knowledge representation and reasoning](../../../knowledge-representation-and-reasoning-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
