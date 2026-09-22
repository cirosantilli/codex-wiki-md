<h1 id="1/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The usual transformation to [clausal normal form](../../../../../../clausal-form.md) preserves $\boxed{\text{equisatisfiability, but not necessarily logical equivalence}}$. Removing implications and distributing [logical conjunction](../../../../../../logical-conjunction.md) and [logical disjunction](../../../../../../logical-disjunction.md) preserve [logical equivalence](../../../../../../logical-equivalence.md). [Skolemization](../../../../../../skolemization.md) introduces new symbols and chooses witnesses as functions of preceding universally quantified variables.

For example,

$$
\varphi=\forall x\exists y\,R(x,y)
\quad\longmapsto\quad
\psi=\forall x\,R(x,f(x)).
$$

On the domain $\{0,1\}$, let $R$ be equality. Then $\varphi$ is true. Expand this same [first-order structure](../../../../../../first-order-structure.md) by interpreting $f$ as the constant function with value $0$. The resulting [first-order structure](../../../../../../first-order-structure.md) falsifies $\psi$ at $x=1$. Interpreting $f$ as the identity instead satisfies $\psi$.

Thus every model of $\psi$ has a reduct satisfying $\varphi$, and a model of $\varphi$ can be expanded with suitable witnesses to satisfy $\psi$. That model-expansion property gives [equisatisfiability](../../../../../../equisatisfiability.md), not [logical equivalence](../../../../../../logical-equivalence.md) for every interpretation of the added function. If “CNF” means a conjunctive matrix with existential quantifiers retained, [Skolemization](../../../../../../skolemization.md) has not yet happened and an equivalent form is possible; this is why the convention must be specified.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Knowledge representation and reasoning](../../../../knowledge-representation-and-reasoning-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
