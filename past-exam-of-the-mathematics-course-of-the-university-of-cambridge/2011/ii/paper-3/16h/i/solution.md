<h1 id="16h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [compactness theorem](../../../../../../compactness-theorem.md) states that a set of first-order sentences has a model if every finite subset has a model. The [Upward Lowenheim-Skolem theorem](../../../../../../upward-lowenheim-skolem-theorem.md) says that an infinite structure $M$ in a language $L$ has an [elementary extension](../../../../../../elementary-extension.md) of every prescribed infinite cardinality $\kappa\geq\max(|M|,|L|,\aleph_0)$.

Add constants $c_a$ for all $a\in M$ and the [elementary diagram of a structure](../../../../../../elementary-diagram-of-a-structure.md) of $M$: every sentence with these constants true in $M$. Add $\kappa$ further constants $d_i$ and sentences $d_i\ne d_j$ for $i\ne j$. Any finite subset is satisfiable in $M$, by choosing the finitely many new constants distinctly, since $M$ is infinite. Compactness gives a model containing an elementary copy of $M$ and at least $\kappa$ elements.

For the exact cardinality, start with that copy and all the $d_i$, a set of cardinality $\kappa$. For every existential formula with parameters from this set that holds in the large model, choose one witness. Also close under the language's functions. Repeat countably many times. At each stage there are at most $\kappa$ formulas and finite parameter tuples, so the union still has cardinality $\kappa$. Every existential formula true in the large model with parameters in the union has a witness in the union; an induction on formulas proves that this substructure is elementary. This establishes the exact-size statement without assuming an unproved downward theorem.

A [dense total order](../../../../../../dense-order.md) with $a<b$ is not a [well-order](../../../../../../well-order.md): the nonempty set $\{x:a<x\}$ has no least element, since density supplies a point strictly between $a$ and any proposed least element.

In the strict-order language, the required axioms are

$$
\forall x\ \neg(x<x),\quad \forall x,y,z\ ((x<y\land y<z)\Rightarrow x<z),
$$



$$
\forall x,y\ (x=y\lor x<y\lor y<x),\quad \forall x,y\ (x<y\Rightarrow\exists z\ (x<z\land z<y)).
$$

These axiomatize dense total orders, allowing endpoints. If more than one point is required, add $\exists x\exists y\ (x<y)$. For a non-strict poset language replace $x<y$ by $x\leq y\land x\ne y$.

$$
\boxed{\text{Dense total orders are first-order axiomatizable.}}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [16H](../../16h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
