<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Absorb (4) using the equivalence

$$
A\sqcap B\sqsubseteq\bot\quad\Longleftrightarrow\quad A\sqsubseteq\neg B.
$$

Thus we can take

$$
\boxed{\mathcal T_u=\{C\equiv\exists P.\top,\ A\sqsubseteq\neg B\},\qquad \mathcal T_g=\{(1),(2),(3)\}.}
$$

Here $A\sqsubseteq\neg B$ is a primitive inclusion, handled by adding $\neg B$ whenever $A$ labels a node. For literal substitution-based [TBox unfolding](../../../../../../tbox-unfolding.md), introduce a fresh [description logic concept](../../../../../../description-logic-concept.md) $A_0$ and replace the primitive inclusion by

$$
A\equiv A_0\sqcap\neg B.
$$

This preserves the original models after forgetting $A_0$: any model of the primitive inclusion extends by taking $A_0=A$, and any model of the new definition satisfies the primitive inclusion. The fresh name is important. Replacing $A$ by $\neg B$ alone would incorrectly assert that every non-$B$ element is an $A$ element.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Knowledge representation and reasoning](../../../../knowledge-representation-and-reasoning-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
