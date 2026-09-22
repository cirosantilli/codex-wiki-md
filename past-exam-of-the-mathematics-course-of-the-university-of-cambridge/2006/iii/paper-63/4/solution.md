<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use a free real [scalar field](../../../../../scalar-field.md) obeying a linear [Klein-Gordon equation](../../../../../klein-gordon-equation.md), for example $(\Box-\mu^2-\xi R)\phi=0$. This linearity is the assumption that permits mode evolution by a [Bogoliubov transformation](../../../../../bogoliubov-transformation.md). Work with a complete set of normalized modes, or normalizable wave packets when the spectrum is continuous. The stationary asymptotic regions supply time translations relative to which [positive-frequency solutions](../../../../../positive-frequency-solution.md) and their complex conjugates can be distinguished.

For solutions define the conserved [Klein-Gordon inner product](../../../../../klein-gordon-inner-product.md)

$$
(u,v)=i\int_\Sigma d\Sigma^a\left(u^*\nabla_av-v\nabla_au^*\right).
$$

Here $\Sigma$ is a [Cauchy surface](../../../../../cauchy-surface.md) with future-directed normal. Its conservation follows by applying the wave equation to the divergence of its current, provided boundary flux is included or vanishes. Let $u_j$ be a positive-frequency basis in the past and $v_s$ one in the future, each propagated as a solution through the intermediate geometry. Normalize them by $(u_i,u_j)=\delta_{ij}$, $(u_i^*,u_j^*)=-\delta_{ij}$ and $(u_i,u_j^*)=0$, with the corresponding identities for the future basis. The two field expansions are

$$
\widehat\phi=\sum_j(a_ju_j+a_j^\dagger u_j^*)
=\sum_s(b_sv_s+b_s^\dagger v_s^*).
$$

The [canonical commutation relations](../../../../../canonical-commutation-relation.md) give $[a_i,a_j^\dagger]=\delta_{ij}$ and $[b_s,b_t^\dagger]=\delta_{st}$. The [in-vacuum](../../../../../in-vacuum.md) satisfies $a_j|0_-\rangle=0$, while the [out-vacuum](../../../../../out-vacuum.md) satisfies $b_s|0_+\rangle=0$. They are generally different vacua.

Fix the coefficient convention by expanding future modes in past modes:

$$
v_s=\sum_j(\alpha_{sj}u_j+\beta_{sj}u_j^*),\qquad
\alpha_{sj}=(u_j,v_s),\qquad \beta_{sj}=-(u_j^*,v_s).
$$

The minus sign is due to the negative norm of the conjugate modes. Taking the [Klein-Gordon inner product](../../../../../klein-gordon-inner-product.md) with the field, which is antilinear in its first entry, gives

$$
\boxed{b_s=\sum_j(\alpha_{sj}^*a_j-\beta_{sj}^*a_j^\dagger).}
$$

Both frequency sectors are needed: if $\beta\ne0$, a future annihilation operator contains a past creation operator. This is the mechanism of [particle number from Bogoliubov coefficients](../../../../../particle-number-from-bogoliubov-coefficients.md), not a classical nonzero mean field.

Computing $[b_s,b_t^\dagger]$ and $[b_s,b_t]$ explicitly gives the [canonical identities for a bosonic Bogoliubov transformation](../../../../../canonical-identities-for-a-bosonic-bogoliubov-transformation.md):

$$
\sum_j(\alpha_{sj}\alpha_{tj}^*-\beta_{sj}\beta_{tj}^*)=\delta_{st},
\qquad
\sum_j(\alpha_{sj}\beta_{tj}-\beta_{sj}\alpha_{tj})=0.
$$

Completeness also gives the inverse $a_j=\sum_s(\alpha_{sj}b_s+\beta_{sj}^*b_s^\dagger)$. Thus the evolved past vacuum, viewed in the future [Fock space](../../../../../fock-space.md), obeys

$$
\left[\alpha^Tb+\beta^\dagger b^\dagger\right]|\Psi\rangle=0.
$$

For a finite-mode treatment with invertible $\alpha$, solve this condition by a [multimode squeezed vacuum](../../../../../multimode-squeezed-vacuum.md):

$$
|\Psi\rangle=C\exp\left(\frac12\sum_{s,t}Z_{st}b_s^\dagger b_t^\dagger\right)|0_+\rangle,
\qquad Z=-(\alpha^T)^{-1}\beta^\dagger.
$$

The canonical identities make $Z$ symmetric. Commuting $b_s$ through the exponential gives $b_s|\Psi\rangle=\sum_tZ_{st}b_t^\dagger|\Psi\rangle$, which directly verifies the vacuum condition. Its normalization is $|C|=\det(I-ZZ^\dagger)^{1/4}$. A general initial state is obtained by applying its initial creation-operator polynomial and expressing those operators in the future basis. In infinitely many modes, a common unitary Fock representation requires the creation-mixing coefficients to be Hilbert-Schmidt; finite wave-packet counts avoid treating delta-normalized modes as individual normalizable states. These are the [bosonic mode mixing implementability](../../../../../bosonic-mode-mixing-implementability.md) conditions, rather than an assumption of arbitrary finite total creation over an infinite time interval.

For the requested [number operator](../../../../../number-operator.md) of one future mode, set $N_s=b_s^\dagger b_s$. Expectations below are in the evolved past vacuum $|\Psi\rangle$, equivalently in $|0_-\rangle$ using the Heisenberg-mode operators above. Acting on the past vacuum gives $b_s|0_-\rangle=-\sum_j\beta_{sj}^*a_j^\dagger|0_-\rangle$, whose squared norm is

$$
\boxed{n_s\equiv\langle N_s\rangle=\sum_j|\beta_{sj}|^2.}
$$

The mean particle number vanishes exactly when that mode has no negative-frequency mixing.

The second moment needs the anomalous contraction

$$
c_s\equiv\langle b_sb_s\rangle=-\sum_j\alpha_{sj}^*\beta_{sj}^*.
$$

The [canonical commutation relations](../../../../../canonical-commutation-relation.md) give $N_s^2=b_s^{\dagger2}b_s^2+N_s$. Moreover,

$$
b_s^2|0_-\rangle=c_s|0_-\rangle
+\sum_{j,k}\beta_{sj}^*\beta_{sk}^*a_j^\dagger a_k^\dagger|0_-\rangle.
$$

Its vacuum and two-particle pieces are orthogonal. Applying the commutation relations twice shows

$$
\langle0_-|a_k a_j a_l^\dagger a_m^\dagger|0_-\rangle
=\delta_{jl}\delta_{km}+\delta_{jm}\delta_{kl}.
$$

The two pairings each contribute $n_s^2$ to the squared norm. Hence the full answer is

$$
\boxed{\langle N_s^2\rangle=2n_s^2+n_s+|c_s|^2
=2\left(\sum_j|\beta_{sj}|^2\right)^2+\sum_j|\beta_{sj}|^2
+\left|\sum_j\alpha_{sj}\beta_{sj}\right|^2.}
$$

Thus $\operatorname{Var}(N_s)=n_s(n_s+1)+|c_s|^2$. These are the [out-mode number fluctuations in the in-vacuum](../../../../../out-mode-number-fluctuations-in-the-in-vacuum.md). Omitting $c_s$ would assume a property not given in the general question. A thermal single mode has $c_s=0$, giving $\langle N_s^2\rangle=2n_s^2+n_s$. A single-mode [squeezed vacuum state](../../../../../squeezed-vacuum-state.md) instead has $|c_s|^2=n_s(n_s+1)$, giving $\langle N_s^2\rangle=3n_s^2+2n_s$.

If the counted observable is the total number over a finite set of future modes, its moments follow by retaining cross-mode correlations as well. Define $C_{st}=\langle b_s^\dagger b_t\rangle$ and $M_{st}=\langle b_sb_t\rangle$. The same vacuum pairings give $\langle N_sN_t\rangle=C_{ss}C_{tt}+|C_{st}|^2+|M_{st}|^2+\delta_{st}C_{ss}$. Thus $\langle N_{\rm tot}\rangle=\operatorname{tr}C$ and $\langle N_{\rm tot}^2\rangle=(\operatorname{tr}C)^2+\operatorname{tr}(C^2)+\operatorname{tr}(M^\dagger M)+\operatorname{tr}C$, with $C_{st}=\sum_j\beta_{sj}\beta_{tj}^*$ and $M_{st}=-\sum_j\alpha_{sj}^*\beta_{tj}^*$. Independent thermal counts cannot be assumed for a general correlated squeezed state.

For [Hawking radiation](../../../../../hawking-radiation.md), choose the incoming vacuum at [past null infinity](../../../../../past-null-infinity.md) of a collapse spacetime and propagate late outgoing modes backwards. Near a nonextremal forming [event horizon](../../../../../event-horizon.md), the logarithmic tortoise-coordinate divergence leads to the [Hawking exponential ray map](../../../../../hawking-exponential-ray-map.md)

$$
U_H-U=Ae^{-\kappa u},
$$

where $u$ is late retarded time, $U$ is an early regular affine null coordinate and $\kappa>0$ is the final [surface gravity](../../../../../surface-gravity.md). A late positive-frequency mode $e^{-i\omega u}$ therefore becomes proportional to $(U_H-U)^{i\omega/\kappa}$ on rays escaping just before horizon formation. This is not positive-frequency with respect to $U$: it has both frequency signs and hence nonzero $\beta$.

The thermal factor can be seen directly. With $x=U_H-U>0$, $a=\omega/\kappa$ and a regulator $\varepsilon>0$, the relevant Fourier integrals are

$$
\int_0^\infty x^{ia}e^{-(\varepsilon\pm i\omega')x}\,dx
=\Gamma(1+ia)(\varepsilon\pm i\omega')^{-1-ia}.
$$

As $\varepsilon\downarrow0$, the arguments of the two complex factors approach $\pm\pi/2$. Their squared-modulus ratio for the suppressed and enhanced frequency branches is $e^{-2\pi a}$. Thus the [thermal ratio of Hawking Bogoliubov coefficients](../../../../../thermal-ratio-of-hawking-bogoliubov-coefficients.md), combined with the canonical normalization, yields the bosonic occupation

$$
\boxed{n_\omega=\frac1{e^{2\pi\omega/\kappa}-1},\qquad
T_H=\frac\kappa{2\pi}}
$$

in units $\hbar=c=k_B=1$. Scattering through the exterior potential multiplies the asymptotic occupation by the appropriate [greybody factor](../../../../../greybody-factor.md).

A complete future mode description includes modes crossing the horizon as well as modes reaching [future null infinity](../../../../../future-null-infinity.md). The global incoming vacuum develops correlations between these sectors; restricting to the exterior gives approximately thermal outgoing occupation rather than a claim that the complete pure state became a thermal mixed state. This is the particle-production picture of a collapsing [black hole](../../../../../black-hole.md), not an incoming thermal bath on an eternal geometry. Including backreaction turns the emitted positive energy into black-hole mass loss. The renormalized quantum stress tensor is not subject to the pointwise classical positivity used in the [black-hole area theorem](../../../../../hawking-s-area-theorem.md), so this does not contradict its classical proof.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
