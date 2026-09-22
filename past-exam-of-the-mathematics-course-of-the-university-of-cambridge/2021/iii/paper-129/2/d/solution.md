<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Bourgain bound for three-term-progression-free sets](../../../../../../bourgain-bound-for-three-term-progression-free-sets.md) states that, if $N=|G|$ is odd and $A\subseteq G$ contains no nonconstant three-term [arithmetic progression](../../../../../../arithmetic-progression.md), then

$$
|A|\ll N\left(\frac{\log\log N}{\log N}\right)^{1/2}.
$$

Here is how it follows from the standard [Bohr-set density increment lemma](../../../../../../bohr-set-density-increment-lemma.md). Begin with $B_0=G$ and relative density $\alpha_0=\alpha=|A|/N$. Whenever the lemma gives its second alternative, replace the current set by the denser translate inside the smaller regular Bohr set. The density changes by

$$
\alpha_{i+1}\geq(1+c\alpha_i)\alpha_i,
$$

so this can happen only $O(\alpha^{-1})$ times. Throughout the iteration the rank is $O(\alpha^{-1})$, the width is at least $\alpha^{O(\alpha^{-1})}$, and the elementary lower bound for the size of a Bohr set gives

$$
|B_i|\geq\alpha^{O(\alpha^{-2})}N.
$$

At the terminal stage the first alternative of the density-increment lemma holds. Combining it with the last display yields

$$
\alpha^{-2}\log(1/\alpha)\ll\log N.
$$

If $\alpha<1/\log N$, Bourgain's bound is already true. Otherwise $\log(1/\alpha)\ll\log\log N$, and rearranging proves

$$
\boxed{\alpha\ll\left(\frac{\log\log N}{\log N}\right)^{1/2}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
