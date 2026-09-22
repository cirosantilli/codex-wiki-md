<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use binary [linear codes](../../../../../linear-code.md) $C\subseteq C'\subseteq\mathbb F_2^N$, with dimensions $k,k'$. For each coset $u+C$ in $C'/C$, define

$$
|u+C\rangle=\frac1{\sqrt{|C|}}\sum_{c\in C}|u+c\rangle.
$$

Representatives of one coset give the same vector, and distinct cosets have disjoint computational supports, so these vectors are orthonormal. Their span is the [CSS code](../../../../../css-code.md) $\mathcal X$, encoding **$\boxed{k'-k\text{ logical qubits in }N\text{ physical qubits}}$**.

For $a,b\in\mathbb F_2^N$, write $X^a=\bigotimes_jX_j^{a_j}$ and $Z^b=\bigotimes_jZ_j^{b_j}$. The code is stabilized by $X^c$ for $c\in C$, because it permutes the sum, and by $Z^z$ for $z\in(C')^\perp$, because $z\cdot(u+c)=0$. These [Pauli operators](../../../../../pauli-operator.md) commute: $c\cdot z=0$. There are $k+N-k'$ independent [stabilizer generators](../../../../../stabilizer-generator.md), so their common positive eigenspace has dimension $2^{N-(k+N-k')}=2^{k'-k}$; it is exactly the span above.

The commuting check measurements separate the two types of error. A bit error $X^a$ changes the signs of the $Z$ checks by $(-1)^{z\cdot a}$, giving the ordinary [syndrome](../../../../../syndrome.md) of $a$ for $C'$. A phase error $Z^b$ changes the $X$ checks by $(-1)^{c\cdot b}$, giving the syndrome of $b$ for the [dual code](../../../../../dual-code.md) $C^\perp$. If $C'$ corrects $t_X$ bit errors and $C^\perp$ corrects $t_Z$ bit errors, these checks identify the respective patterns, and inverse Pauli operations recover the state without revealing the logical coset. This is the [nested-code CSS syndrome recovery](../../../../../nested-code-css-syndrome-recovery.md) procedure.

The sharper distances account for harmless stabilizer errors. A Pauli $X^aZ^b$ commutes with every check precisely when $a\in C'$ and $b\in C^\perp$. Among these, it acts as a stabilizer, up to a phase, precisely when $a\in C$ and $b\in(C')^\perp$. To justify the latter assertion, $X^a$ with $a\in C'\setminus C$ permutes distinct logical cosets, while $Z^b$ with $b\in C^\perp\setminus(C')^\perp$ has unequal signs on two such cosets. Neither can act as a scalar, and a combined operator has the same nontrivial permutation or phase distinction. For positive logical dimension set

$$
d_X=\min_{a\in C'\setminus C}\operatorname{wt}(a),\qquad
d_Z=\min_{b\in C^\perp\setminus(C')^\perp}\operatorname{wt}(b).
$$

The [quantum code distance](../../../../../distance-of-a-quantum-error-correcting-code.md) is **$\boxed{d=\min(d_X,d_Z)}$**: a nontrivial logical Pauli has at least one nonstabilizer component of weight at least the corresponding distance, while a pure $X$ or pure $Z$ logical operator attains the minimum. The weight of $X^aZ^b$ counts the union of its supports, so this argument also includes $Y$ errors.

Here is the correction proof for coherent errors, not only a classical decoding argument. Let $P$ be the code projector and let $E,F$ have bit-component weights at most $t_X$ and phase-component weights at most $t_Z$. If $2t_X<d_X$ and $2t_Z<d_Z$, the corresponding components of $E^\dagger F$ have weights below $d_X,d_Z$. If this product anticommutes with a stabilizer $S$, then $P(E^\dagger F)P=-P(E^\dagger F)P=0$, using $SP=P$. If it commutes with all stabilizers, the weight bounds force its two components into $C$ and $(C')^\perp$, so its code compression is a scalar multiple of $P$. Thus the [Knill--Laflamme condition](../../../../../knill-laflamme-condition.md) holds for the entire error family.

To see directly why this gives a common recovery, diagonalize its positive Gram matrix $c_{EF}$ and form the corresponding error combinations $F_j$. Their restrictions obey $PF_j^\dagger F_lP=c_j\delta_{jl}P$. For $c_j>0$, $F_jP/\sqrt{c_j}$ is an isometry onto a syndrome subspace, and the different images are orthogonal. Measure these subspaces and apply the inverse isometry; zero-$c_j$ combinations annihilate the code. This recovers every [quantum channel](../../../../../quantum-channel.md) whose [Kraus operators](../../../../../kraus-operator.md) lie in the error span. Arbitrary operators supported on at most $t$ qubits expand in [Pauli operators](../../../../../pauli-operator.md) with the same support. Consequently the CSS code corrects **all errors on up to $\boxed{t=\lfloor(d-1)/2\rfloor}$ qubits**, and more generally the asymmetric family just described. The sufficient classical bound is obtained by replacing $d_X,d_Z$ by the minimum distances of $C'$ and $C^\perp$, respectively; degeneracy can improve it.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
