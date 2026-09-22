<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $q_1=\bar Q^{\dot1}$ and $q_2=\bar Q^{\dot2}$. In the Jacobi-consistent convention just fixed,

$$
[J_i,q_a]=-\frac12(\sigma_i)_{ab}q_b.
$$

Applying the [commutator](../../../../../commutator.md) product rule twice gives

$$
[J^2,q_a]=\sum_i\bigl(J_i[J_i,q_a]+[J_i,q_a]J_i\bigr)
=\frac34q_a-\sum_i(\sigma_i)_{ab}q_bJ_i.
$$

Here $\sum_i\sigma_i^2=3I$ produces the constant term; moving the $J_i$ to the right accounts for it. Consequently

$$
\begin{aligned}
[J^2,q_1]&=\tfrac34q_1-q_2(J_1-iJ_2)-q_1J_3,\\
[J^2,q_2]&=\tfrac34q_2-q_1(J_1+iJ_2)+q_2J_3.
\end{aligned}
$$

Thus the physically consistent numerical coefficients are

$$
\boxed{(a_1,\ldots,a_9)=
(-\tfrac12,\tfrac34,-1,i,-1,\tfrac34,-1,-i,1).}
$$

If one mechanically retains the literal positive-sign column transformation instead, the coefficient tuple would be $(\tfrac12,\tfrac34,1,-i,1,\tfrac34,1,i,-1)$. It cannot describe a unitary multiplet with the supplied rotation algebra, by the explicit Jacobi counterexample in part (a).

Take the spin-zero [Clifford vacuum](../../../../../clifford-vacuum.md) $|\Omega\rangle$, normalized to one and annihilated by the two annihilation charges. This is a lowest Fock state of a positive-mass representation, not a zero-energy vacuum annihilated by every charge. For the first one-charge state,

$$
J^2q_1|\Omega\rangle=\tfrac34q_1|\Omega\rangle,
\qquad J_3q_1|\Omega\rangle=-\tfrac12q_1|\Omega\rangle.
$$

The ladder [commutators](../../../../../commutator.md) are $[J_+,q_1]=-q_2$, $[J_-,q_1]=0$, $[J_+,q_2]=0$, $[J_-,q_2]=-q_1$. Therefore these two states are the $j=1/2$ pair. A phase choice $|\tfrac12,+\tfrac12\rangle=-Nq_2|\Omega\rangle$ makes the usual positive ladder coefficient hold.

Raising the dotted index only changes the oscillator basis by the unitary antisymmetric epsilon matrix, so $\{q_a,q_b^\dagger\}=2m\delta_{ab}$. Since $q_a^\dagger|\Omega\rangle=0$,

$$
\|q_a|\Omega\rangle\|^2=2m,
\qquad\boxed{N=\frac1{\sqrt{2m}},\quad Nq_1|\Omega\rangle:
(j,j_3)=(\tfrac12,-\tfrac12).}
$$

The positive convention would formally label this state with $j_3=+1/2$ while $J_+$ acts nontrivially on it, contradicting the highest-weight ladder rule. This supplies an independent state-level check of the needed sign correction.

The two-charge state is a [rotation singlet](../../../../../singlet-state.md). Indeed, using $q_1^2=q_2^2=0$ and $q_2q_1=-q_1q_2$, the product rule gives $[J_i,q_1q_2]=0$ for every $i$: only the sum of the two diagonal spinor coefficients survives, and their trace is zero. Hence the requested [commutators](../../../../../commutator.md) and quantum numbers are

$$
\boxed{[J^2,q_1q_2]=[J_3,q_1q_2]=0,
\qquad N^2q_1q_2|\Omega\rangle:(j,j_3)=(0,0).}
$$

Its squared norm is $(2m)^2$ before multiplication by $N^4$, by the two oscillator [anticommutators](../../../../../anticommutator.md).

The [spin-zero massive N=1 supermultiplet](../../../../../spin-zero-massive-n-1-supermultiplet.md) therefore consists of $|\Omega\rangle$, $Nq_1|\Omega\rangle$, $Nq_2|\Omega\rangle$ and $N^2q_1q_2|\Omega\rangle$. Their [spins](../../../../../spin.md) are $0,1/2,1/2,0$, all with the same mass $m$. Starting with an even vacuum, the two spin-zero states are bosonic and the two one-charge states fermionic. They are the two real scalar degrees of freedom and the two on-shell [fermion](../../../../../fermion.md) polarizations of a massive chiral multiplet. Any product of three creation charges repeats an index and vanishes; annihilation charges reduce to these four states by the [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md). **There are exactly four independent states.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
