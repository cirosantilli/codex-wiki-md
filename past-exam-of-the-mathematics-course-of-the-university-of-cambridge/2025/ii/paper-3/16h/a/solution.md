<h1 id="16h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By [choice-function well-ordering construction](../../../../../../choice-function-well-ordering-construction.md), use [transfinite recursion](../../../../../../transfinite-recursion.md) to choose

$$
x_\beta=f\left(x\setminus\{x_\gamma:\gamma<\beta\}\right)
$$

whenever the set on the right is nonempty. The chosen elements are distinct, so if this construction continued through the [Hartogs theorem](../../../../../../hartogs-theorem.md) ordinal $h(x)$, the map $\beta\mapsto x_\beta$ would inject $h(x)$ into $x$, a contradiction. It therefore stops at some ordinal $\alpha<h(x)$. At the stopping stage every element of $x$ has been selected, and hence

$$
\beta\longmapsto x_\beta
$$

is a bijection $\alpha\to x$.

Assuming the [axiom of choice](../../../../../../axiom-of-choice.md), every set $x$ has such a choice function on its nonempty subsets. Transporting the membership order on $\alpha$ across the bijection well-orders $x$. Thus the axiom of choice implies the [well-ordering theorem](../../../../../../well-ordering-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16H](../../16h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
