# Sequential Bayesian photon counting

↑ **Parent:** [Haroche cavity photon nondemolition experiment](haroche-cavity-photon-nondemolition-experiment.md)

Consider an original balanced-readout model, rather than a fit to the experiment. Let $n\in\{0,\ldots,N_{\max}\}$, with a normalized [prior probability](prior-probability.md) $p_0(n)\geq0$ and $\sum_n p_0(n)=1$. A detected [chemical atom](atom-physics.md) has outcome $s\in\{e,g\}$. Define the [conditional probabilities](conditional-probability.md)

$$
L_e(n;\phi)=P(e\mid n,\phi)=\frac{1+C\cos(\phi+n\chi)}2,\qquad
L_g(n;\phi)=1-L_e(n;\phi),\qquad 0\leq C\leq1.
$$

Here $\chi$ is the accumulated [quantum phase](quantum-phase.md) per photon, $\phi$ the controlled analysis [quantum phase](quantum-phase.md), and $C$ the fringe contrast. The two [probabilities](probability.md) sum to one for every $n$. Actual calibration may also require an offset and asymmetric detection errors; $C$ alone does not specify a [quantum instrument](quantum-instrument.md).

Assume no [photon number](photon-number.md) change during the record and fresh independently prepared atomic meters. For observed outcomes $s_1,\ldots,s_k$ at recorded settings $\phi_1,\ldots,\phi_k$, the [Born rule](born-rule.md) and [Bayes' theorem](bayes-theorem.md) give

$$
Z_k=\sum_{m=0}^{N_{\max}}p_{k-1}(m)L_{s_k}(m;\phi_k),\qquad
p_k(n)=\frac{p_{k-1}(n)L_{s_k}(n;\phi_k)}{Z_k}
=\frac{p_0(n)\prod_{j=1}^k L_{s_j}(n;\phi_j)}{\sum_{m=0}^{N_{\max}}p_0(m)\prod_{j=1}^k L_{s_j}(m;\phi_j)}.
$$

The [posterior probability](posterior-probability.md) is defined only for $Z_k>0$. Summing its numerator over $n$ proves normalization. This is also the update of diagonal elements of a field [density operator](density-matrix-split.md) under a [measurement in quantum mechanics](quantum-measurement-split.md); it does not assume that an initial [quantum superposition](quantum-superposition.md) was an unknown pre-existing integer. The observed settings are part of the record, especially when selected adaptively.

For an exact finite example take $p_0=(1,1,1,1)/4$, $C=4/5$, and $\chi=\pi/2$. An $e$ outcome at $\phi=0$ has [likelihood](likelihood-function.md) $(9,5,1,5)/10$, giving $p_1=(9,5,1,5)/20$. Another $e$ at $\phi=-\pi/2$ gives $p_2=(9,9,1,1)/20$. A subsequent $g$ at $\phi=0$ gives

$$
p_3=\frac1{68}(9,45,9,5),\qquad P(s_1=e,s_2=e,s_3=g)=\frac{17}{200}.
$$

Thus three atomic records raise the [posterior probability](posterior-probability.md) of $n=1$ from $1/4$ to $45/68$, while leaving finite uncertainty. No one of these outcomes identifies $n$ with certainty.

<a id="image-synthetic-atomic-records-progressively-concentrate-a-photon-number-posterior"></a>
![](sequential-photon-number-posterior.png)

**[Figure 3](#image-synthetic-atomic-records-progressively-concentrate-a-photon-number-posterior). Synthetic atomic records progressively concentrate a photon-number posterior**. Original simulation, not laboratory data: $n=0,\ldots,7$, uniform prior, $C=0.8$, $\chi=\pi/4$, four cyclic analysis phases, and a fixed simulated $n=3$. Cavity loss is omitted. Individual updates can broaden the distribution even though this record eventually concentrates.

The periodic [likelihood function](likelihood-function.md) imposes an identifiability limit. If $\chi=2\pi/q$ for an integer $q>0$, then $L_s(n+q;\phi)=L_s(n;\phi)$ for every setting: the [posterior odds](posterior-odds.md) between $n$ and $n+q$ never change. Varying $\phi$ can resolve a cosine reflection ambiguity within a period, but cannot remove this exact period. Changing $\chi$ can supply additional information. A finite cutoff is therefore a physical assumption to justify, not evidence that excluded high [photon numbers](photon-number.md) were absent. At $C=0$ no outcome changes the [prior probability](prior-probability.md); at $0<C<1$ neither binary outcome has an exactly zero [likelihood](likelihood-function.md).

The no-loss assumption also has a time limit. In an original zero-temperature loss model, let $\kappa=1/T_c$. A [Fock state](fock-state.md) $|n\rangle$ loses its first photon at rate $n\kappa$, so its survival [probability](probability.md) is $\exp(-n\kappa t)$ and its mean lifetime is $T_c/n$ for $n>0$. Several records must be acquired within that lifetime to identify a plateau. When losses matter, first predict $p_k^-(n)=\sum_m T_{nm}(\Delta t)p_{k-1}(m)$ using a normalized transition [matrix](matrix.md), then apply the atomic [Bayesian inference](bayesian-statistics-split.md) update to $p_k^-$. Thermal excitation requires upward transitions too. A delayed or broadened inference after a jump need not indicate that an atom caused the jump.

## ↑ Ancestors (7)

1. [Haroche cavity photon nondemolition experiment](haroche-cavity-photon-nondemolition-experiment.md)
2. [Quantum nondemolition measurement](quantum-nondemolition-measurement.md)
3. [Measurement in quantum mechanics](quantum-measurement-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
