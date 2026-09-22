<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use target signature $(-,+,\ldots,+)$ and a closed-string spatial coordinate $0\le\sigma\le2\pi$. Write $Y$ for the compact coordinate and $X^A$ for the noncompact coordinates. In [conformal gauge](../../../../../conformal-gauge.md), the [wave equation](../../../../../wave-equation-split.md) factorizes, so every coordinate is a sum of a function of $\tau+\sigma$ and a function of $\tau-\sigma$. The closed-string boundary conditions are

$$
X^A(\tau,\sigma+2\pi)=X^A(\tau,\sigma),\qquad Y(\tau,\sigma+2\pi)=Y(\tau,\sigma)+2\pi wR,\quad w\in\mathbb Z.
$$

Thus the [derivatives](../../../../../derivative.md) of each chiral part are periodic and have [integer](../../../../../integer.md) [Fourier modes](../../../../../fourier-mode.md); only their [worldsheet zero modes](../../../../../worldsheet-zero-mode.md) can produce the winding displacement. Integrating these [Fourier series](../../../../../fourier-series-split.md) gives the [closed-string mode expansion](../../../../../closed-string-mode-expansion.md)

$$
X^A=x^A+\alpha'p^A\tau+i\sqrt{\frac{\alpha'}2}\sum_{m\ne0}\frac{\alpha_m^Ae^{-im(\tau-\sigma)}+\widetilde\alpha_m^Ae^{-im(\tau+\sigma)}}m,
$$



$$
Y=y+\alpha'\frac nR\tau+wR\sigma+i\sqrt{\frac{\alpha'}2}\sum_{m\ne0}\frac{\alpha_m^Ye^{-im(\tau-\sigma)}+\widetilde\alpha_m^Ye^{-im(\tau+\sigma)}}m.
$$

The oscillator reality conditions are $\alpha_m^\dagger=\alpha_{-m}$ and similarly for the tilded modes. The coefficient of $\tau$ follows by integrating the [canonical momentum](../../../../../canonical-momentum.md) density $\dot Y/(2\pi\alpha')$. Single-valued wavefunctions of the center coordinate $y\sim y+2\pi R$ have [momentum](../../../../../momentum.md) $n/R$, with $n\in\mathbb Z$. Equivalently, the compact chiral [worldsheet zero modes](../../../../../worldsheet-zero-mode.md) are $\alpha'p_L(\tau+\sigma)/2$ and $\alpha'p_R(\tau-\sigma)/2$, where

$$
\boxed{p_L=\frac nR+\frac{wR}{\alpha'},\qquad p_R=\frac nR-\frac{wR}{\alpha'}.}
$$

Here tildes denote the left-moving sector. This convention will also fix the sign in [compact-circle closed-string level matching](../../../../../compact-circle-closed-string-level-matching.md).

Choose a noncompact light-cone pair and impose [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md) $X^+=x^++\alpha'p^+\tau$, with $p^+\ne0$. The [Virasoro constraints](../../../../../virasoro-constraint.md) $(\partial_\pm X)^2=0$ then solve for $\partial_\pm X^-$ in terms of the transverse coordinates. For example, with $\partial_\pm=\partial_\tau\pm\partial_\sigma$, one has $\partial_\pm X^-=(\partial_\pm X^i)^2/(2\alpha'p^+)$. Thus there are two independent transverse oscillator [Fock spaces](../../../../../fock-space.md), including $Y$ among the transverse coordinates. Quantization gives $[\alpha_m^i,\alpha_k^j]=m\delta^{ij}\delta_{m+k,0}$, and the same relation for the tilded oscillators, with the two sectors commuting. Lorentz consistency gives the [critical dimension of the bosonic string](../../../../../critical-dimension-of-string-theory.md) $D=26$ and [string intercept](../../../../../normal-ordering-constant-of-a-string.md) one in each sector. Accordingly

$$
N=\sum_{m>0}\alpha_{-m}^i\alpha_m^i,\qquad \widetilde N=\sum_{m>0}\widetilde\alpha_{-m}^i\widetilde\alpha_m^i
$$

count 24 transverse oscillator species. The two zero-mode constraints give the lower-dimensional [bosonic string mass spectrum](../../../../../bosonic-string-mass-spectrum.md)

$$
M^2=p_R^2+\frac4{\alpha'}(N-1)=p_L^2+\frac4{\alpha'}(\widetilde N-1).
$$

Taking their difference and average yields

$$
\boxed{\widetilde N-N+nw=0,\qquad M^2=\frac{n^2}{R^2}+\frac{w^2R^2}{\alpha'^2}+\frac2{\alpha'}(N+\widetilde N-2).}
$$

Every choice of transverse [string oscillators](../../../../../string-oscillator.md) and [integer](../../../../../integer.md) charges satisfying this [closed-string level matching](../../../../../closed-string-level-matching.md) is a [physical string state](../../../../../physical-string-state.md) in light-cone gauge. The eliminated longitudinal oscillators do not supply additional polarizations.

To classify all massless states, positivity of the two compact terms implies $N+\widetilde N\le2$. When the sum is two, masslessness forces $n=w=0$, and [closed-string level matching](../../../../../closed-string-level-matching.md) then forces $N=\widetilde N=1$. The states $\alpha_{-1}^i\widetilde\alpha_{-1}^j|0\rangle$ have $24^2=576$ polarizations. In 25 noncompact dimensions, their decomposition gives a [graviton](../../../../../graviton.md), a [Kalb–Ramond field](../../../../../kalb-ramond-field.md), a [dilaton](../../../../../dilaton.md), two Abelian gauge vectors from the metric and two-form with one compact index, and the radius [scalar field](../../../../../scalar-field.md). Their physical polarization counts are

$$
275+253+2\cdot23+1+1=576.
$$

The first two numbers are the symmetric [traceless second-rank tensor](../../../../../traceless-second-rank-tensor.md) and [antisymmetric second-rank tensor](../../../../../antisymmetric-second-rank-tensor.md) of the massless [little group](../../../../../little-group.md) $SO(23)$.

When $N+\widetilde N=1$, [closed-string level matching](../../../../../closed-string-level-matching.md) requires $|nw|=1$. The compact contribution obeys

$$
\frac{n^2}{R^2}+\frac{w^2R^2}{\alpha'^2}\ge\frac{2|nw|}{\alpha'}=\frac2{\alpha'},
$$

and equality occurs precisely at $R=\sqrt{\alpha'}$. The charges $n=w=\pm1$ have $(N,\widetilde N)=(1,0)$; the charges $n=-w=\pm1$ have $(N,\widetilde N)=(0,1)$. Each charge has 24 polarizations supplied by its single excited sector. At a general radius these have

$$
M^2=\left(\frac R{\alpha'}-\frac1R\right)^2.
$$

Finally, $N=\widetilde N=0$ requires $nw=0$. The [exceptional massless ground states of a bosonic circle](../../../../../exceptional-massless-ground-states-of-a-bosonic-circle.md) occur at

$$
R=\frac{|n|\sqrt{\alpha'}}2\quad(w=0,n\ne0),\qquad R=\frac{2\sqrt{\alpha'}}{|w|}\quad(n=0,w\ne0).
$$

Each charge is a [scalar field](../../../../../scalar-field.md). These special radii must be included if “general radius” is to mean a complete classification, rather than only a generic radius. **At a generic radius the massless spectrum is the neutral 576-state spectrum above; at exceptional radii one adds exactly the states just listed.** The neutral [ground state](../../../../../ground-state.md) remains tachyonic.

The map

$$
R'=\frac{\alpha'}R,\qquad (n',w')=(w,n)
$$

sends $p_L$ to $p_L$ and $p_R$ to $-p_R$. Reversing all right-moving compact [string oscillators](../../../../../string-oscillator.md), $\alpha_m^Y\mapsto-\alpha_m^Y$, preserves their [commutators](../../../../../commutator.md) and oscillator number; the left-moving oscillators are unchanged. Both the mass formula and [compact-circle closed-string level matching](../../../../../compact-circle-closed-string-level-matching.md) are therefore unchanged, with a one-to-one map of the complete oscillator basis. **This proves [T-duality](../../../../../t-duality.md) of the full spectrum, including winding, massive and tachyonic states.**

At the [self-dual circle](../../../../../self-dual-circle-compactification.md) the four single-oscillator charge families give $4\cdot24=96$ new massless states. Each family decomposes into a 25-dimensional gauge vector with 23 polarizations and one [scalar field](../../../../../scalar-field.md). There are also four massless [ground states](../../../../../ground-state.md), with charges $(\pm2,0)$ and $(0,\pm2)$. Thus the [massless spectrum at the bosonic self-dual circle](../../../../../massless-spectrum-at-the-bosonic-self-dual-circle.md) has

$$
\boxed{576+96+4=676\ \text{polarizations}:\quad4\ \text{extra vectors and}\ 8\ \text{extra scalars}.}
$$

The gauge interpretation follows directly from the chiral compact-boson operators. With $\langle Y_L(z)Y_L(0)\rangle=-\alpha'\log z/2$, the exponential $e^{ikY_L}$ has [conformal weight](../../../../../conformal-weight.md) $\alpha'k^2/4$. At the self-dual radius,

$$
J_L^3=\frac{i}{\sqrt{\alpha'}}\partial Y_L,\qquad J_L^\pm=:e^{\pm2iY_L/\sqrt{\alpha'}}:
$$

have weight one and satisfy $J^3(z)J^3(0)\sim1/(2z^2)$, $J^3(z)J^\pm(0)\sim\pm J^\pm(0)/z$, and $J^+(z)J^-(0)\sim z^{-2}+2J^3(0)/z$. These are the level-one $SU(2)$ current relations; the right sector supplies another copy. Multiplying these currents by a noncompact oscillator produces six gauge vectors in total. The nine scalar [string vertex operators](../../../../../string-vertex-operator.md) $J_L^aJ_R^b$ form the $(3,3)$ representation, accounting for the radius [scalar field](../../../../../scalar-field.md) and eight new [scalar fields](../../../../../scalar-field.md). The remaining neutral fields are the [graviton](../../../../../graviton.md), two-form and [dilaton](../../../../../dilaton.md).

A [radius deformation as a Higgs mechanism](../../../../../radius-deformation-as-a-higgs-mechanism.md) is the [expectation value](../../../../../expectation-value.md) of the Cartan–Cartan scalar [string vertex operator](../../../../../string-vertex-operator.md) $J_L^3J_R^3\propto\partial Y_L\bar\partial Y_R$. Its stabilizer is $U(1)_L\times U(1)_R$, so

$$
\boxed{SU(2)_L\times SU(2)_R\longrightarrow U(1)_L\times U(1)_R,\qquad m_W=\left|\frac R{\alpha'}-\frac1R\right|.}
$$

The four compact single-oscillator [scalar field](../../../../../scalar-field.md) polarizations become [longitudinal polarizations](../../../../../longitudinal-polarization.md) of the four [massive vectors](../../../../../massive-vector-particle.md), exactly as in the [Higgs mechanism](../../../../../higgs-mechanism.md). The other four extra [scalar fields](../../../../../scalar-field.md) have masses $4/R^2-4/\alpha'$ or $4R^2/\alpha'^2-4/\alpha'$ and need not remain massless; one pair becomes tachyonic on either side of the self-dual point. Together with the original bosonic [tachyon](../../../../../tachyon.md), this means that the gauge-symmetry interpretation is formal and does not assert a stable bosonic-string vacuum.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
