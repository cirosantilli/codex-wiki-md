<h1 id="4g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A word $w$ is accepted by the [Epsilon-NFA](../../../../../../epsilon-nfa.md) precisely when

$$
\widehat\delta_E(q_0,w)\cap F_E\ne\varnothing.
$$

By part (b), this reached subset is exactly $\widehat\delta_D(q_D,w)$, and by the definition of $F_D$ the intersection condition is equivalent to $\widehat\delta_D(q_D,w)\in F_D$. Hence

$$
\boxed{\mathcal L(D)=\mathcal L(E).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4G](../../4g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
