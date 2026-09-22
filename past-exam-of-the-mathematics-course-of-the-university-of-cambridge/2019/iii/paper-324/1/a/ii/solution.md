<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the [finite abelian group](../../../../../../../finite-abelian-group.md) additively. Its [group shift operator](../../../../../../../group-shift-operator.md) is

$$
\boxed{U(h)|g\rangle=|g+h\rangle.}
$$

These [unitary operators](../../../../../../../unitary-operator.md) form the [regular representation](../../../../../../../regular-representation.md) and commute. The representation-theoretic facts we use are that every [irreducible representation of a finite abelian group](../../../../../../../irreducible-representation-of-a-finite-abelian-group.md) is one-dimensional, there are $|G|$ such [characters of a representation](../../../../../../../character-of-a-representation.md), and their [character orthogonality](../../../../../../../character-orthogonality.md) gives an [orthonormal basis](../../../../../../../orthonormal-basis.md) of functions on $G$. Each [linear character](../../../../../../../linear-character.md) here is a [group homomorphism](../../../../../../../group-homomorphism.md) $\chi:G\to U(1)$, with $|\chi(g)|=1$.

For $\chi\in\widehat G$, the [character group of a finite abelian group](../../../../../../../character-group-of-a-finite-abelian-group.md), put

$$
|v_\chi\rangle=\frac1{\sqrt{|G|}}\sum_{g\in G}\overline{\chi(g)}|g\rangle.
$$

Changing variables to $u=g+h$ gives

$$
U(h)|v_\chi\rangle
=\frac1{\sqrt{|G|}}\sum_u\overline{\chi(u-h)}|u\rangle
=\boxed{\chi(h)|v_\chi\rangle}.
$$

The $|G|$ vectors $|v_\chi\rangle$ are therefore a common [eigenbasis](../../../../../../../eigenbasis.md). Using $\chi(g)$ instead of its [complex conjugate](../../../../../../../complex-conjugate.md) in their definition reverses every [eigenphase](../../../../../../../eigenphase.md); this is merely the [quantum Fourier transform](../../../../../../../quantum-fourier-transform.md) sign convention.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
