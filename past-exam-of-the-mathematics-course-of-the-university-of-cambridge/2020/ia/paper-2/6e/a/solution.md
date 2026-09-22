<h1 id="6e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The singleton orbits are exactly $X^G$. Every other orbit represented by $x$ has size $|G|/|G_x|$ by the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md). Partitioning $X$ into its [orbits of a group action](../../../../../../orbit-of-a-group-action.md) therefore gives

$$
|X|=|X^G|+\sum_x\frac{|G|}{|G_x|}.
$$

For the second identity, count

$$
Z=\{(g,x)\in G\times X:g\cdot x=x\}
$$

in two ways. Holding $g$ fixed gives

$$
|Z|=\sum_{g\in G}|X^g|.
$$

Holding $x$ fixed gives $|Z|=\sum_{x\in X}|G_x|$. Each orbit contributes $|G|/|G_x|$ points, each with stabilizer size $|G_x|$, and hence contributes $|G|$. Thus $|Z|=|G|\,|X/G|$, proving [Burnside lemma](../../../../../../burnside-s-lemma.md):

$$
\boxed{|X/G|=\frac1{|G|}\sum_{g\in G}|X^g|}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6E](../../6e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
