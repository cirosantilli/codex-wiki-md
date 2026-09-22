<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Under the usual reversible-circuit interpretation, there is a genuine [obstruction to uniform probability lowering by a unitary](../../../../../../obstruction-to-uniform-probability-lowering-by-a-unitary.md) in the printed premise. The universal assertion cannot hold for arbitrary $p$: it fails already at the search density $p=k/N$.

An explicit counterexample uses $N=4$, one good basis state $|0\rangle$, $p=1/4$ and $p'=1/8$. The six pure states

$$
|\psi_{j,\pm}\rangle=\frac12|0\rangle\pm\frac{\sqrt3}{2}|j\rangle,\qquad j=1,2,3,
$$

all have good probability $1/4$. Their equally weighted [density operator](../../../../../../density-matrix.md) is $I_4/4$, a [maximally mixed state](../../../../../../maximally-mixed-state.md). Every [unitary operator](../../../../../../unitary-operator.md) $C$ leaves this mixture unchanged, so its average output good probability remains $1/4$. The printed assertion would instead make all six output probabilities $1/8$, a contradiction. More generally, averaging states $\sqrt{k/N}|g\rangle+e^{i\alpha}\sqrt{1-k/N}|b\rangle$ uniformly over good and bad basis vectors and two opposite phases gives $I_N/N$, proving the same obstruction at the actual search density $p=k/N$.

The intended conditional construction needs only a supplied reversible preparation that lowers the success probability of the particular starting state, not of every state. Here is the complete argument under that weaker resource assumption. Count $C$ and $C^\dagger$ as supplied, query-free operations, as required for the claimed input-oracle bound. Let $\theta=\arcsin\sqrt{k/N}$ and choose

$$
j=\left\lceil\frac\pi{4\theta}-\frac12\right\rceil,\qquad\theta_* =\frac\pi{4j+2},\qquad p_* =\sin^2\theta_*\le\frac kN.
$$

If equality holds, use the original preparation. Otherwise use the stipulated preparation on $|\psi_0\rangle$ to obtain $|\psi_*\rangle=C|\psi_0\rangle$ with good probability $p_*$. Its [reflection operator](../../../../../../reflection-operator.md) is implementable by

$$
I_{\psi_*}=C I_{\psi_0}C^\dagger.
$$

The good and bad components may be nonuniform, but [amplitude amplification](../../../../../../amplitude-amplification.md) applies to this same two-dimensional decomposition. After $j$ iterations of $-I_{\psi_*}I_f$, its good probability is

$$
\boxed{\sin^2((2j+1)\theta_*)=1,\qquad j=O\!\left(\sqrt{N/k}\right).}
$$

Thus **the stated exact-query conclusion follows from accessible preparation of one known-overlap state and its inverse.** If the supplied preparation uses oracle queries, those costs cannot be omitted.

A physically realizable [known-state success dilution for exact amplitude amplification](../../../../../../known-state-success-dilution-for-exact-amplitude-amplification.md) is available in the standard enlarged marking-oracle model. Append a flag in $\sqrt{1-q}|0\rangle+\sqrt q|1\rangle$, where $q=p_*/p$, and call a joint state good only when $f(x)=1$ and the flag is one. This prepared state's success probability is exactly $pq=p_*$. Reflect about this known product preparation and mark the joint good subspace; $j$ ordinary iterations then succeed with certainty. A supplied controlled phase oracle gives one marking query per iteration, or a Boolean bit oracle computes $f$, applies the joint phase and uncomputes $f$ in two queries. Measuring the data therefore returns a good $x$ with certainty in $O(\sqrt{N/k})$ queries. This changes the state space and marking test, and does not assert the impossible universal $n$-qubit circuit. Controlled access is an additional resource in a bare phase-oracle model, so it is made explicit rather than silently assumed.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
