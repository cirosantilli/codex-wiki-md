<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In the state-picture convention, a [Stinespring representation of a completely positive map](../../../../../../stinespring-representation-of-a-completely-positive-map.md) $\mathcal N:\mathcal L(\mathcal H_Q)\to\mathcal L(\mathcal H_{Q'})$ consists of an auxiliary [Hilbert space](../../../../../../hilbert-space-split.md) $\mathcal H_E$ and a linear map $V:\mathcal H_Q\to\mathcal H_{Q'}\otimes\mathcal H_E$ such that

$$
\boxed{\mathcal N(X)=\operatorname{Tr}_E(VXV^\dagger)\quad\text{for all }X.}
$$

The [partial trace](../../../../../../partial-trace.md) discards the environment. For example, from a [Kraus representation](../../../../../../kraus-representation.md) $\mathcal N(X)=\sum_jK_jXK_j^\dagger$, take $V=\sum_jK_j\otimes|j\rangle_E$. The adjoint, or observable-picture, form is $\mathcal N^\dagger(Y)=V^\dagger(Y\otimes I_E)V$.

A general [completely positive map](../../../../../../completely-positive-map.md) does not require $V$ to be an [linear isometry of Hilbert spaces](../../../../../../linear-isometry-of-hilbert-spaces.md). If $\mathcal N$ is trace preserving, then $V^\dagger V=\sum_jK_j^\dagger K_j=I$, so $V$ is an [linear isometry of Hilbert spaces](../../../../../../linear-isometry-of-hilbert-spaces.md). This is the [Stinespring dilation](../../../../../../stinespring-dilation.md) of a [quantum channel](../../../../../../quantum-channel.md), which will be used in the data-processing proof.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
