<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use base-two [logarithms](../../../../../../logarithm.md), so [entanglement entropy](../../../../../../entanglement-entropy.md) is measured in bits. Write $h_2(p)=-p\log_2p-(1-p)\log_2(1-p)$ for the [binary entropy](../../../../../../binary-entropy.md), with $0\log_20=0$. Taking a [partial trace](../../../../../../partial-trace.md) over any two parties removes the off-diagonal terms: the two traced strings are orthogonal. Consequently all three one-party [reduced density matrices](../../../../../../reduced-density-matrix.md) of the first [pure state](../../../../../../pure-state.md) are

$$
\rho_A=\rho_B=\rho_C=p|0\rangle\langle0|+(1-p)|1\rangle\langle1|.
$$

Each division into two groups is one party versus the other two. The [Schmidt coefficients](../../../../../../schmidt-coefficient.md) are $\sqrt p$ and $\sqrt{1-p}$, so **the entanglement entropy across each of $A:BC$, $B:AC$ and $C:AB$ is $h_2(p)$**. For the second [pure state](../../../../../../pure-state.md), set $p=1/2$: every one-party [reduced density matrix](../../../../../../reduced-density-matrix.md) is $I/2$, and **all three entanglement entropies are one bit**.

For every pair $XY$, the first [pure state](../../../../../../pure-state.md) instead gives the [reduced density matrix](../../../../../../reduced-density-matrix.md)

$$
\rho_{XY}=p|00\rangle\langle00|+(1-p)|11\rangle\langle11|.
$$

This is a [separable quantum state](../../../../../../separable-quantum-state.md), explicitly a [convex combination](../../../../../../convex-combination.md) of two [product states](../../../../../../product-state.md). Its [relative entropy of entanglement](../../../../../../relative-entropy-of-entanglement.md) is therefore zero: in $E_R(\rho)=\inf_{\sigma\in\mathrm{Sep}}D(\rho\|\sigma)$, choose $\sigma=\rho$ to attain zero, while [nonnegativity of quantum relative entropy](../../../../../../nonnegativity-of-quantum-relative-entropy.md) excludes a negative value. The same argument with equal weights applies to the second [pure state](../../../../../../pure-state.md). Thus

$$
\boxed{E_R(\rho_{AB})=E_R(\rho_{AC})=E_R(\rho_{BC})=0\quad\text{for both states}.}
$$

The pairwise [density matrices](../../../../../../density-matrix.md) contain classical correlations, despite the [entanglement](../../../../../../entangled-state.md) of the global [pure state](../../../../../../pure-state.md); discarding a party loses the coherence between its two branches.

The [entanglement entropy](../../../../../../entanglement-entropy.md) of $n$ independent source copies across any cut is $nh_2(p)$, whereas $f(n)$ copies of the target [GHZ state](../../../../../../greenberger-horne-zeilinger-state.md) have [entanglement entropy](../../../../../../entanglement-entropy.md) $f(n)$. [Average monotonicity of pure-state entanglement entropy](../../../../../../average-monotonicity-of-pure-state-entanglement-entropy.md) under [LOCC](../../../../../../local-operations-and-classical-communication.md) gives $P(n)f(n)\leq nh_2(p)$ for exact successful forward branches. In a reversible asymptotic conversion the reverse direction similarly prevents a first-order deficit, since $n'/n\to1$. For asymptotically faithful outputs, a [continuity bound for quantum conditional entropy](../../../../../../continuity-bound-for-quantum-conditional-entropy.md) with trivial conditioning changes these inequalities only by $o(n)$. Hence **the reversible leading-order rate is**

$$
\boxed{f(n)=nh_2(p)+o(n),\qquad \lim_{n\to\infty}\frac{f(n)}n=h_2(p).}
$$

The zero pairwise [relative entropies of entanglement](../../../../../../relative-entropy-of-entanglement.md) are consistent with this conversion: no independent pairwise resource has to be supplied or removed.

There is a qualification to the literal finite-block formulation in the source. For $0<p<1$, the [Schmidt rank](../../../../../../schmidt-rank.md) of the exact state of $n'$ source copies is $2^{n'}$, whereas $f$ target [GHZ states](../../../../../../greenberger-horne-zeilinger-state.md) have [Schmidt rank](../../../../../../schmidt-rank.md) $2^f$. Every refined [LOCC](../../../../../../local-operations-and-classical-communication.md) branch acts by a product of local [linear operators](../../../../../../linear-operator.md) and cannot increase this [Schmidt rank](../../../../../../schmidt-rank.md). For $p\ne1/2$, the displayed rate has $f<n'$ for sufficiently large blocks when $n'/n\to1$, so an exact successful reverse conversion is impossible, irrespective of its claimed probability. The [exact dilution obstruction from Schmidt rank](../../../../../../exact-dilution-obstruction-from-schmidt-rank.md) is avoided in the usual asymptotic formulation by allowing outputs approaching the desired [pure state](../../../../../../pure-state.md). The leading-order rate above and the exact forward protocol below remain valid; neither establishes the source's stronger exact round-trip claim. At $p=1/2$ the two states are identical. At $p=0$ or $1$, the source is a known [product state](../../../../../../product-state.md), the rate is zero, and local preparation supplies any desired number of source copies.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
