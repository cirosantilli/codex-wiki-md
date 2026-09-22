<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In a point-particle description of [quantum gravity](../../../../../../quantum-gravity.md), interactions of a massless spin-two field occur at localized vertices of [Feynman diagrams](../../../../../../feynman-diagram.md). The gravitational coupling has negative mass dimension for spacetime dimension greater than two, so short-distance loop integrations generate higher-derivative counterterms that cannot all be absorbed into the Einstein action. A [string worldsheet](../../../../../../worldsheet.md) instead joins incoming and outgoing strings by a smooth surface. In particular, a closed string splits or joins through a smooth pair-of-pants surface. There is no invariantly distinguished point at which every part of an extended string interacts. The choice of a time slicing can draw a joining point, but it is not a physical pointlike vertex. This removes the point-interaction geometry responsible for arbitrarily localized interactions and introduces the [string length](../../../../../../string-length.md) $\ell_s=\sqrt{\alpha'}$.

This geometric explanation is supported by the organization of the [Polyakov path integral](../../../../../../polyakov-path-integral.md). Introducing a [worldsheet](../../../../../../worldsheet.md) metric makes the [Nambu–Goto action](../../../../../../nambu-goto-action.md) amenable to [gauge fixing](../../../../../../gauge-fixing.md). In the Euclidean integral, metrics on a fixed oriented surface are divided by [worldsheet diffeomorphisms](../../../../../../worldsheet-diffeomorphism.md) and [Weyl transformations](../../../../../../weyl-transformation.md). What remains is a [Riemann surface](../../../../../../riemann-surfaces.md) with a conformal structure, together with finitely many [worldsheet moduli](../../../../../../worldsheet-moduli.md) and the positions of external [string vertex operators](../../../../../../string-vertex-operator.md). The determinants from fixing the metric are represented by [Faddeev-Popov ghosts](../../../../../../faddeev-popov-ghost.md). Schematically, for $n$ closed-string external states,

$$
\mathcal A_n=\sum_{g\geq0}g_s^{2g-2+n}\int_{\mathcal M_{g,n}}d\mu\,
\left\langle\prod_{i=1}^nV_i\;\text{(ghost insertions)}\right\rangle_g.
$$

Here $\mathcal M_{g,n}$ is the moduli space of genus-$g$ punctured surfaces. The dilaton weights a surface by its [Euler characteristic](../../../../../../euler-characteristic.md) $\chi=2-2g$, giving $g_s^{-\chi}$ before the normalization of external states. Every additional handle multiplies the contribution by $g_s^2$. The [string genus expansion](../../../../../../string-genus-expansion.md) therefore plays the role of the ordinary loop expansion, with the sphere giving tree level and the torus giving one loop. The critical dimension cancels the [worldsheet Weyl anomaly](../../../../../../worldsheet-weyl-anomaly.md), making this reduction to conformal geometry consistent.

The massless symmetric traceless closed-string state is a [graviton](../../../../../../graviton.md), and its long-wavelength interactions reproduce gravity. At distances comparable with $\ell_s$, however, an infinite tower of excited states contributes. This is more than a single particle form factor: the same amplitude contains graviton exchange, massive higher-spin exchange and string-scale softness.

The dimensionless variables in the given [Virasoro–Shapiro amplitude](../../../../../../virasoro-shapiro-amplitude.md) correspond to $s=\alpha'S/4$, $t=\alpha'T/4$, $u=\alpha'U/4$, where capital letters denote the usual dimensionful [Mandelstam invariants](../../../../../../mandelstam-variables.md). Its [constraint](../../../../../../constraint-mechanics.md) $s+t+u=-4$ identifies the external particles as the closed bosonic [tachyons](../../../../../../tachyon.md), not four gravitons. Nevertheless its intermediate massless pole directly exhibits graviton exchange. The overall normalization will be suppressed below; no additional copy of the amplitude formula is needed.

First, the amplitude is symmetric under permutations of $s,t,u$, expressing [crossing symmetry](../../../../../../crossing-symmetry.md). The poles in any channel are

$$
\boxed{s=n-1,\quad n=0,1,2,\ldots,\qquad M_n^2=\frac{4(n-1)}{\alpha'}.}
$$

For generic $t$, the residue can be calculated with the [Gamma function](../../../../../../gamma-function.md) pole at $-n$ and its recurrence:

$$
\boxed{\mathop{\rm Res}_{s=n-1}A=-\frac1{(n!)^2}\left[\prod_{j=2}^{n+1}(t+j)\right]^2.}
$$

The product is $1$ when $n=0$. Indeed, the pole factor contributes $(-1)^{n+1}/n!$, while the two remaining Gamma ratios contribute $(-1)^n(t+2)_n^2/n!$. A residue polynomial of degree $2n$ shows exchange of spins up to $2n$, with leading [Regge trajectory](../../../../../../regge-trajectory.md) $J=2+2s$. At $n=1$, the massless residue is $-(t+2)^2$, containing the spin-two exchange. By crossing, the massless $t$-channel pole is

$$
\boxed{A(s,t)=-\frac{(s+2)^2}{t}+O(1)\quad(t\longrightarrow0),}
$$

for generic $s$. Thus at large $s$ the pole behaves as $s^2/t$, the characteristic [energy](../../../../../../energy.md) dependence of [graviton](../../../../../../graviton.md) exchange. Its massless propagator produces the long-range gravitational interaction. At low energies the massive poles can instead be expanded into local higher-derivative corrections to the effective gravitational action.

At the string scale one must retain the whole tower. The [Gamma reflection formula](../../../../../../gamma-reflection-formula.md) rewrites the amplitude exactly as

$$
A=-\frac{\Gamma(-1-t)}{\Gamma(t+2)}\left[\frac{\Gamma(s+t+3)}{\Gamma(s+2)}\right]^2\frac{\sin\pi(s+t)}{\sin\pi s}.
$$

At large $s$ and fixed $t$, away from the resonance poles or with a specified complex continuation, the Gamma ratio scales as $s^{t+1}$. Hence the [Regge limit](../../../../../../regge-limit.md) scales as $s^{2+2t}$, up to the signature factor and the displayed $t$-dependent coefficient. In particular, a fixed nonzero [momentum](../../../../../../momentum.md) transfer changes the point-graviton power law by a factor $s^{2t}$: the graviton belongs to an entire trajectory rather than remaining an isolated spin-two exchange at arbitrarily high [energy](../../../../../../energy.md).

There is stronger suppression when the scattering angle is fixed. Put $t\simeq-as$, $u\simeq-(1-a)s$ with $0<a<1$. Applying [Stirling formula](../../../../../../stirling-formula.md) to the Gamma functions, after the same treatment of real-axis poles, gives the leading smooth envelope

$$
\boxed{\log|A|=-2s\,f(a)+O(\log s),\qquad f(a)=-a\log a-(1-a)\log(1-a)>0.}
$$

The leading $s\log s$ terms cancel and the remaining entropy-like combination is negative. In physical units the exponent is $-\alpha'Sf(a)/2$. This [fixed-angle softness of the closed-string amplitude](../../../../../../fixed-angle-softness-of-the-closed-string-amplitude.md) is absent for an elementary pointlike gravitational vertex. Equivalently, short-distance gravitational scattering probes additional string degrees of freedom. In a four-dimensional long-distance effective setting, a massive exchanged mode contributes a Yukawa-type correction proportional to $e^{-M_nr}/r$, with couplings and tensor factors depending on the external states. Such terms are suppressed for $r\gg\ell_s$ and become relevant for $r\sim\ell_s$. The amplitude establishes the spectrum and short-distance change; it does not by itself give a universal static potential for arbitrary sources. Its bosonic [tachyon](../../../../../../tachyon.md) also signals an unstable vacuum, so it must not be treated as a complete stable model of a gravitational force.

Finally, the [modular group](../../../../../../modular-group.md) prevents overcounting equivalent surfaces and reorganizes the loop ultraviolet region. A torus is $\mathbb C/(\mathbb Z+\tau\mathbb Z)$ with $\operatorname{Im}\tau>0$. A change of lattice basis identifies

$$
\tau\sim\frac{a\tau+b}{c\tau+d},\qquad a,b,c,d\in\mathbb Z,\quad ad-bc=1.
$$

Thus the one-loop integral uses a fundamental domain for $\operatorname{PSL}(2,\mathbb Z)$, for example

$$
\boxed{\mathcal F=\{\tau:|\operatorname{Re}\tau|\leq\tfrac12,\ |\tau|\geq1,\ \operatorname{Im}\tau>0\}.}
$$

The measure $d^2\tau/(\operatorname{Im}\tau)^2$ is invariant, and the physical integrand, including matter, ghosts and external insertions, must respect [torus modular invariance](../../../../../../torus-modular-invariance.md). In this domain $\operatorname{Im}\tau\geq\sqrt3/2$. The region of arbitrarily small proper time that causes [ultraviolet divergences](../../../../../../ultraviolet-divergence.md) in a particle loop is therefore not an independent part of the string integral; a modular transformation relates it to another description already represented in the domain.

This does not remove every possible divergence. The cusp $\operatorname{Im}\tau\to\infty$ is a long tube, and factorization through it can produce [infrared divergences](../../../../../../infrared-divergence.md), massless tadpoles or the bosonic [tachyon](../../../../../../tachyon.md) divergence. At higher genus, degenerating cycles similarly factorize into propagating intermediate string states. The essential improvement is the relation between [worldsheet](../../../../../../worldsheet.md) geometry, the full spectrum and the quotient by large diffeomorphisms; infrared and unstable-background problems remain separate questions. A short-distance expansion that keeps only the graviton discards precisely this structure.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
