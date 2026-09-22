<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**No representation exists, even allowing arbitrary signed weights and [self-loops](../../../../../loop-graph-theory.md).** Every singleton [coalition](../../../../../coalition-game-theory.md) loses, so each loop weight must be $\ell_i=v(\{i\})=0$. Every two-player [coalition](../../../../../coalition-game-theory.md) wins, which then forces

$$
w_{12}=w_{13}=w_{23}=1.
$$

The represented grand-[coalition](../../../../../coalition-game-theory.md) value would consequently be

$$
v(\{1,2,3\})=\ell_1+\ell_2+\ell_3+w_{12}+w_{13}+w_{23}=3,
$$

contradicting its required value $1$. The obstruction is the additive [edge](../../../../../edge-of-a-graph.md) representation, not a restriction that weights be nonnegative: the singleton and pair values already determine every relevant weight.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
