<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use units $k_B=\hbar=c=1$. In critical [light-cone gauge in string theory](../../../../../../light-cone-gauge-in-string-theory.md), each chiral sector of the [closed bosonic string](../../../../../../closed-string.md) has 24 transverse [string oscillator](../../../../../../string-oscillator.md) species. Their [generating function](../../../../../../generating-function.md) is

$$
F(q)=\prod_{m\geq1}(1-q^m)^{-24}=\sum_{N\geq0}d_Nq^N.
$$

Each factor sums the independent occupation numbers of the [string oscillators](../../../../../../string-oscillator.md) at level $m$. For $q=e^{-t}$ with $t\downarrow0$, the modular transformation of the [Dedekind eta function](../../../../../../dedekind-eta-function.md) gives

$$
F(e^{-t})\sim\left(\frac{t}{2\pi}\right)^{12}\exp\left(\frac{4\pi^2}{t}-t\right).
$$

Extract the coefficient by a contour integral and apply the [saddle-point approximation](../../../../../../saddle-point-approximation.md) to the exponent $(N-1)t+4\pi^2/t$. The saddle is $t_*=2\pi/\sqrt{N-1}$, with exponent $4\pi\sqrt{N-1}$ and second derivative $(N-1)^{3/2}/\pi$. The factor $t^{12}$ gives $(N-1)^{-6}$, and the Gaussian width gives $(N-1)^{-3/4}/\sqrt2$. Hence

$$
d_N\sim\frac1{\sqrt2}(N-1)^{-27/4}e^{4\pi\sqrt{N-1}}.
$$

For a noncompact [closed string](../../../../../../closed-string.md), [closed-string level matching](../../../../../../closed-string-level-matching.md) imposes equal left and right levels, but does not correlate their transverse polarizations. Therefore the [large-level degeneracy of a closed bosonic string](../../../../../../large-level-degeneracy-of-a-closed-bosonic-string.md) is

$$
\boxed{g_N=d_N^2\sim\frac12(N-1)^{-27/2}e^{8\pi\sqrt{N-1}}.}
$$

The mass relation is $\alpha'M^2=4(N-1)$. Thus $8\pi\sqrt{N-1}=\beta_HM$ with

$$
\boxed{\beta_H=4\pi\sqrt{\alpha'},\qquad T_H=\frac1{4\pi\sqrt{\alpha'}}.}
$$

Distinguish degeneracy per discrete level from a smoothed density per unit rest mass. Since $dN/dM=\alpha'M/2$, the latter is

$$
\rho(M)\sim C M^{-26}e^{\beta_HM}.
$$

The exponential growth comes from the many ways of distributing [string oscillator](../../../../../../string-oscillator.md) energy along a string; it is much faster than a fixed finite collection of particle species. The corresponding high-energy [entropy](../../../../../../entropy.md) is $S(E)=\beta_HE+O(\log E)$, so its microcanonical [temperature](../../../../../../temperature.md) tends to $T_H$. Additional energy can go into very long strings rather than raising the [temperature](../../../../../../temperature.md) substantially.

The Boltzmann suppression competes with this exponential density. For the [string oscillator](../../../../../../string-oscillator.md) rest-mass sum alone the large-$M$ tail is $\int dM\,M^{-26}e^{-(\beta-\beta_H)M}$. It converges for $\beta>\beta_H$ and fails for $\beta<\beta_H$. To include translational states in 25 noncompact spatial dimensions, take the one-string [partition function](../../../../../../canonical-partition-function.md) per unit spatial volume. At large $M$,

$$
\int d^{25}p\,e^{-\beta\sqrt{M^2+p^2}}\sim\left(\frac{2\pi M}{\beta}\right)^{25/2}e^{-\beta M}.
$$

This follows by expanding the energy as $M+p^2/(2M)+\cdots$ and doing a Gaussian [momentum](../../../../../../momentum.md) integral. Its high-mass contribution is consequently proportional to

$$
\int_{M_0}^\infty dM\,M^{-27/2}e^{-(\beta-\beta_H)M}.
$$

This integral is finite at $\beta=\beta_H$, although nonanalytic there: its first twelve derivatives in $\beta$ are finite, while the thirteenth diverges. The endpoint expansion contains a term proportional to $(\beta-\beta_H)^{25/2}$. Thus one must not assert that the [canonical partition function](../../../../../../canonical-partition-function.md) necessarily diverges exactly at $T_H$; the polynomial prefactor and the spatial spectrum matter. This is the [finite canonical partition function at the bosonic Hagedorn threshold](../../../../../../finite-canonical-partition-function-at-the-bosonic-hagedorn-threshold.md) distinction. The multi-string ideal gas has the same leading Hagedorn threshold, since the higher occupation-cycle terms probe $\ell\beta$, $\ell\geq2$, and are nonsingular at $\beta_H$.

There is also a [spacetime](../../../../../../spacetime.md) diagnosis. Euclidean [temperature](../../../../../../temperature.md) makes time a circle of radius $R_\beta=\beta/(2\pi)$. A [string oscillator](../../../../../../string-oscillator.md) ground state winding once around that circle, with zero [momentum](../../../../../../momentum.md) number, has

$$
m_{\rm th}^2=\frac{R_\beta^2}{\alpha'^2}-\frac4{\alpha'}=\frac{\beta^2}{4\pi^2\alpha'^2}-\frac4{\alpha'}.
$$

It becomes massless at $\beta_H$ and tachyonic for $T>T_H$. This [thermal winding instability of a closed bosonic string](../../../../../../thermal-winding-instability-of-a-closed-bosonic-string.md) signals failure of the perturbative low-temperature gas and motivates a transition to a different high-energy phase, often described in terms of long-string or winding-mode condensation. Free state counting fixes the threshold and its singular behavior, not the interacting phase's endpoint or the order of a transition.

Finally, the ordinary bosonic [tachyon](../../../../../../tachyon.md) is already an infrared instability at zero [temperature](../../../../../../temperature.md). The above canonical discussion is a formal analysis of the high-level spectrum with that separate infrared problem regulated. It does not establish a stable thermal vacuum of the unmodified bosonic theory; an actual equilibrium transition requires an appropriate stable setting and control of interactions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
