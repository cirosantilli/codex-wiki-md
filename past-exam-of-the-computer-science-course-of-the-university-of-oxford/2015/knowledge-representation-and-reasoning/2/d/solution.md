<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For [EL with bottom](../../../../../el-with-bottom.md), the eligible axioms are $\boxed{(2),(4),(5)}$. Axioms (1) and (3) contain universal restrictions, and (3) also contains a disjunction, so they are outside its syntax. For plain [EL](../../../../../el.md), whose constructors are $\top$, atomic names, conjunction and existential restriction, the eligible axioms are $\boxed{(2),(5)}$; (4) is excluded because it uses $\bot$. These conventions should not be conflated.

Here is a normalized [TBox](../../../../../tbox.md) for the bottom-inclusive version. Introduce one fresh [description logic concept](../../../../../description-logic-concept.md) $X$ for $\exists R.A$, and use

$$
\boxed{\begin{aligned}
\exists R.A&\sqsubseteq X,\qquad X\sqsubseteq\exists R.A,\\
X&\sqsubseteq\exists R.X,\\
A\sqcap B&\sqsubseteq\bot,\\
C&\sqsubseteq\exists P.\top,\qquad \exists P.\top\sqsubseteq C.
\end{aligned}}
$$

These are the usual normalized forms: an existential restriction on the left with an atomic right-hand side, an atomic left-hand side with an existential restriction on the right, or a conjunction of atomic names implying $\bot$. Here $\top$ is permitted as a filler.

The first two [general concept inclusions](../../../../../general-concept-inclusion.md) force $X\equiv\exists R.A$. The third then says $\exists R.A\sqsubseteq\exists R.\exists R.A$, exactly (2). Conversely, any model of (2) extends by $X=(\exists R.A)^{\mathcal I}$ to satisfy all three normalized [general concept inclusions](../../../../../general-concept-inclusion.md). The last two are the two directions of (5). For plain [EL](../../../../../el.md), delete just $A\sqcap B\sqsubseteq\bot$ from this normalized [TBox](../../../../../tbox.md).

## ↑ Ancestors (11)

1. [D](../d.md)
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
