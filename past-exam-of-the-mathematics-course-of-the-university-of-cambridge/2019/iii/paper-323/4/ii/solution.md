<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose an [orthonormal basis](../../../../../../orthonormal-basis.md) $\{|j\rangle\}_{j=1}^d$ of the input space and define operators from the input to the $k$-dimensional outcome register by

$$
K_{a,j}=|a\rangle\langle j|\sqrt{E_a}.
$$

These give a [Kraus representation](../../../../../../kraus-representation.md):

$$
\sum_{a,j}K_{a,j}XK_{a,j}^\dagger
=\sum_a\operatorname{Tr}(E_aX)|a\rangle\langle a|=\Phi(X).
$$

The [POVM](../../../../../../positive-operator-valued-measure.md) completeness relation gives

$$
\sum_{a,j}K_{a,j}^\dagger K_{a,j}
=\sum_a\sqrt{E_a}\left(\sum_j|j\rangle\langle j|\right)\sqrt{E_a}
=\sum_aE_a=I.
$$

Therefore $\Phi$ is a [completely positive map](../../../../../../completely-positive-map.md) and is trace preserving: it is a [quantum channel](../../../../../../quantum-channel.md) representing a deterministic [measurement channel](../../../../../../measurement-channel.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
