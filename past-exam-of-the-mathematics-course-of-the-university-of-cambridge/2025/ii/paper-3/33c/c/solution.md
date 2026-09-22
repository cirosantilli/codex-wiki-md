<h1 id="33c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $T_{ij}=a_i^\dagger a_j$, expand the commutator and commute one annihilation operator past one creation operator:

$$
\begin{aligned}
[T_{ij},T_{kl}]
&=a_i^\dagger a_j a_k^\dagger a_l
 -a_k^\dagger a_l a_i^\dagger a_j\\
&=\delta_{jk}a_i^\dagger a_l
 -\delta_{il}a_k^\dagger a_j.
\end{aligned}
$$

Hence the [oscillator bilinear commutator](../../../../../../oscillator-bilinear-commutator.md) is

$$
\boxed{[T_{ij},T_{kl}]=\delta_{jk}T_{il}-\delta_{il}T_{kj}}.
$$

Since

$$
H=T_{xx}+T_{yy}+1,
$$

we obtain

$$
[T_{ij},H]
=\sum_k(\delta_{jk}T_{ik}-\delta_{ik}T_{kj})=0.
$$

Every $T_{ij}$ therefore acts within a fixed energy eigenspace.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [33C](../../33c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
