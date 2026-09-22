<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the [addition of angular momentum](../../../../../addition-of-angular-momentum.md), the uncoupled orthonormal [basis](../../../../../basis.md) is $|j_1m_1\rangle\otimes|j_2m_2\rangle$, whereas the coupled orthonormal [basis](../../../../../basis.md) diagonalizes $\mathbf J^2$ and $J_3$ for $\mathbf J=\mathbf J_1+\mathbf J_2$. Define the [Clebsch-Gordan coefficients](../../../../../clebsch-gordan-coefficients.md) by

$$
|JM\rangle=\sum_{m_1,m_2}C^{JM}_{m_1m_2}|j_1m_1\rangle|j_2m_2\rangle,\qquad
C^{JM}_{m_1m_2}=\langle j_1m_1,j_2m_2\mid JM\rangle.
$$

The [Clebsch-Gordan decomposition](../../../../../clebsch-gordan-decomposition.md) allows $|j_1-j_2|\leq J\leq j_1+j_2$ in unit steps, and a coefficient vanishes unless $m_1+m_2=M$. Taking the inner product of the expansion with itself proves

$$
\sum_{m_1,m_2}|C^{JM}_{m_1m_2}|^2=\langle JM|JM\rangle=1.
$$

With the customary real phase convention the modulus signs can be omitted, giving the sum of squares used in the question. In an arbitrary phase convention the modulus-square identity is the invariant statement.

Treat the [strong interaction](../../../../../strong-interaction.md) as exactly [isospin](../../../../../isospin.md)-invariant for this calculation. Its transition operator $T$ commutes with the three [isospin](../../../../../isospin.md) generators and hence with their [quadratic Casimir operator](../../../../../quadratic-casimir-operator.md). Acting on the initial state $|IM\rangle$, it can therefore produce only final states with the same $I$ and $M$. The [tensor product representation](../../../../../tensor-product-of-group-representations.md) of final multiplets $I_1,I_2$ contains one copy of each permitted total [isospin](../../../../../isospin.md), so $T|IM\rangle=a_M|(I_1I_2)IM\rangle$. Commuting $T$ with the lowering operator gives

$$
a_M\sqrt{(I+M)(I-M+1)}=a_{M-1}\sqrt{(I+M)(I-M+1)}.
$$

Every connecting ladder factor is nonzero, so all $a_M$ coincide with one reduced coefficient $a$. Expanding the final coupled state now gives the [isospin-invariant two-body decay amplitude](../../../../../isospin-invariant-two-body-decay-amplitude.md)

$$
\boxed{A_{M_1M_2;M}=a\,\langle I_1M_1,I_2M_2\mid IM\rangle.}
$$

The reduced coefficient may depend on the particle species, momenta and [spin](../../../../../spin.md) channel, but not on the three [isospin](../../../../../isospin.md) projections. Summing the squared amplitude over the orthogonal charge channels gives

$$
\boxed{\sum_{M_1,M_2}|A_{M_1M_2;M}|^2=|a|^2.}
$$

A physical [decay rate](../../../../../decay-width.md) also includes phase space, angular integration and any [spin](../../../../../spin.md) sums. In the [isospin](../../../../../isospin.md)-degenerate limit these factors are common to the charge channels; absorbing their square root into $a$ gives $\Gamma_{IM}=|a|^2$ for this specified two-body multiplet channel. If several distinct species or independent [spin](../../../../../spin.md) channels are included in “anything”, their reduced rates must additionally be summed. There is no extra factor $2I+1$ when the initial magnetic component is fixed.

The [Delta baryon](../../../../../delta-baryon.md) states have $I=3/2$ and projections $3/2,1/2,-1/2,-3/2$ for $\Delta^{++},\Delta^+,\Delta^0,\Delta^-$. The [proton](../../../../../proton.md) and [neutron](../../../../../neutron.md) form $I=1/2$, with projections $+1/2,-1/2$, and the [pion](../../../../../pion.md) triplet has $I=1$ with projections $+1,0,-1$. The highest coupled state is

$$
|3/2,3/2\rangle=|p\pi^+\rangle.
$$

Apply the total lowering operator $I_-=I_-^{(N)}+I_-^{(\pi)}$. Its coefficient on the left is $\sqrt3$, while on the right the nucleon and [pion](../../../../../pion.md) coefficients are $1$ and $\sqrt2$:

$$
\sqrt3\,|3/2,1/2\rangle=|n\pi^+\rangle+\sqrt2\,|p\pi^0\rangle.
$$

The squared [Clebsch-Gordan coefficients](../../../../../clebsch-gordan-coefficients.md) are consequently $1/3$ and $2/3$, compared with coefficient one for the $\Delta^{++}$ channel. Thus the [Delta baryon pion branching ratios](../../../../../delta-baryon-pion-branching-ratios.md) are

$$
\boxed{\frac{\Gamma(\Delta^+\to p\pi^0)}{\Gamma(\Delta^{++}\to p\pi^+)}=\frac23,\qquad
\frac{\Gamma(\Delta^+\to n\pi^+)}{\Gamma(\Delta^{++}\to p\pi^+)}=\frac13.}
$$

At the opposite end of the same [isospin multiplet](../../../../../isospin-multiplet.md), $|3/2,-3/2\rangle=|n\pi^-\rangle$, so **the strong decay is $\Delta^-\to n\pi^-$**, with the same reduced rate in this symmetry limit. Physical mass splittings and electromagnetic effects perturb these idealized equal-kinematics ratios.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
