<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Include all fixed resource states and all measurement records in an environment, so the entire physical protocol has an [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md) $U$ from the unknown input to a larger pure output. If every recipient receives a perfect copy, its [reduced density matrix](../../../../../../reduced-density-matrix.md) is the pure projector $|\psi\rangle\langle\psi|$. A pure marginal forces factorization: write a joint [vector](../../../../../../vector.md) in a [basis](../../../../../../basis.md) beginning with $|\psi\rangle$; its squared components along every [orthogonal](../../../../../../orthogonal-vectors.md) [basis](../../../../../../basis.md) [vector](../../../../../../vector.md) vanish because their marginal [probabilities](../../../../../../probability.md) are zero. Applying this successively to all recipients gives

$$
U(|\psi\rangle|R\rangle)=|\psi\rangle^{\otimes N}|E_\psi\rangle,
$$

where $|R\rangle$ is the fixed initial resource and $|E_\psi\rangle$ may depend on the input. This includes Alice's discarded systems and every possible outcome record.

Choose two distinct nonorthogonal [pure states](../../../../../../pure-state.md), for example $|0\rangle$ and $|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$, and write their overlap as $s$. Preservation of the [inner product](../../../../../../inner-product.md) by the [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md) requires

$$
s=s^N\langle E_\psi|E_\varphi\rangle.
$$

Normalized environment [vectors](../../../../../../vector.md) have overlap of absolute value at most one. Thus $0<|s|<1$ would imply $|s|\leq|s|^N$, impossible for $N>1$. Hence **perfect transmission of a copy to every recipient is impossible for $N>1$**. This proves the [no-cloning theorem](../../../../../../no-cloning-theorem.md) obstruction even though Alice keeps no copy herself.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
