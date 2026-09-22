<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Distinguish target-space light-cone coordinates from the worldsheet $\pm$ labels. In target space take $X^\pm=(X^0\pm X^{25})/\sqrt2$, so the [Minkowski metric](../../../../../minkowski-metric.md) is $ds^2=-2dX^+dX^-+\sum_i(dX^i)^2$. After [conformal gauge](../../../../../conformal-gauge.md) has been chosen, the residual transformations of $\tau+\sigma$ and $\tau-\sigma$ may be used, on a patch with $p^+\ne0$, to make

$$
X^+=x^++\kappa\tau.
$$

For an open string on $0\le\sigma\le\pi$, the conventional normalization is $\kappa=2\alpha'p^+$. For the closed-string convention of the preceding solution, $\kappa=\alpha'p^+$. In either case, the two [Virasoro constraints](../../../../../virasoro-constraint.md) read

$$
-2\partial_\pm X^+\partial_\pm X^-+\sum_i(\partial_\pm X^i)^2=0.
$$

Since $\partial_\pm X^+=\kappa/2$, they determine the longitudinal coordinate:

$$
\boxed{\partial_\pm X^-=\frac1\kappa\sum_i(\partial_\pm X^i)^2.}
$$

Its oscillator content is fixed by the transverse coordinates, leaving $d-2$ independent fields. This is the [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md); it solves the constraints rather than imposing them afresh on each transverse state.

For [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) at both endpoints, the open-string expansion is

$$
X^\mu=x^\mu+2\alpha'p^\mu\tau+i\sqrt{2\alpha'}\sum_{n\ne0}\frac{\alpha_n^\mu}{n}e^{-in\tau}\cos(n\sigma).
$$

The transverse [string oscillators](../../../../../string-oscillator.md) satisfy $[\alpha_m^i,\alpha_n^j]=m\delta^{ij}\delta_{m+n,0}$, $i,j=1,\ldots,24$, and $\alpha_{n>0}^i|0,p\rangle=0$. Define $L_n^\perp=\tfrac12\sum_m:\!\alpha_{n-m}^i\alpha_m^i\!:$ and $\alpha_0^+=\sqrt{2\alpha'}p^+$. The solved longitudinal modes, including the zero-mode constraint, are

$$
\alpha_n^-=\frac{L_n^\perp-a\delta_{n0}}{\alpha_0^+}.
$$

The critical [bosonic string theory](../../../../../bosonic-string-theory.md) has 24 transverse bosons. Their regulated oscillator vacuum energy is $24\cdot\tfrac12\sum_{n\ge1}n=-1$, since the finite term of $\sum_{n\ge1}ne^{-\varepsilon n}=\varepsilon^{-2}-1/12+O(\varepsilon^2)$ is $-1/12$. Thus the [normal-ordering constant of a string](../../../../../normal-ordering-constant-of-a-string.md) is $a=1$. A normalized transverse [Fock space](../../../../../fock-space.md) basis for general excited [physical string states](../../../../../physical-string-state.md) is

$$
\boxed{|\{k_{ni}\};p\rangle=\prod_{n\ge1}\prod_{i=1}^{24}\frac{(\alpha_{-n}^i/\sqrt n)^{k_{ni}}}{\sqrt{k_{ni}!}}|0,p\rangle,
\qquad k_{ni}\in\{0,1,2,\ldots\},}
$$

with finitely many nonzero occupation numbers. Arbitrary physical states are superpositions of this basis, with each momentum on its corresponding [mass shell](../../../../../mass-shell.md). The [string level operator](../../../../../string-level-operator.md) and [open bosonic string mass spectrum](../../../../../open-bosonic-string-mass-spectrum.md) give

$$
N=\sum_{n,i}n k_{ni},\qquad
\boxed{M^2=\frac{N-1}{\alpha'},\qquad p^-=\frac{p_i p_i+(N-1)/\alpha'}{2p^+}.}
$$

All spatial directions have free endpoints, so **this string ends on a space-filling D25-brane**. More generally, a [D-brane](../../../../../d-brane.md) has [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) along its worldvolume and [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) in its transverse directions; a D$p$-brane has $p$ spatial worldvolume directions. A stack may additionally supply [Chan-Paton factors](../../../../../chan-paton-factor.md), without changing the oscillator construction above.

To see [T-duality of D-brane boundary conditions](../../../../../t-duality-of-d-brane-boundary-conditions.md) directly, decompose the compact coordinate as $X= X_L(\tau+\sigma)+X_R(\tau-\sigma)$ and define its dual by $\widetilde X=X_L-X_R$. Differentiation gives

$$
\partial_\tau\widetilde X=\partial_\sigma X,\qquad
\partial_\sigma\widetilde X=\partial_\tau X.
$$

Therefore the original [Neumann boundary condition](../../../../../neumann-boundary-condition.md) $\partial_\sigma X=0$ becomes $\partial_\tau\widetilde X=0$ at each endpoint. The dual endpoint coordinate is time-independent: **the dual condition is Dirichlet**. Conversely a fixed endpoint in $X$ becomes Neumann in the dual coordinate. For a circle, the [T-duality](../../../../../t-duality.md) radius is $\widetilde R=\alpha'/R$. A wrapped Neumann brane loses one spatial dimension in the dual picture, for example D25 becomes D24. The two dual endpoint constants need not be identical; their positions encode the original Wilson-line data.

For the separated-brane problem, use two static parallel D$p$-branes and no relative angle or background field. Let their displacement in transverse directions be $d^I$, with $\sum_I(d^I)^2=d^2$. A Dirichlet coordinate contains the classical term

$$
X^I(\sigma,\tau)=y_1^I+\frac{d^I}{\pi}\sigma+\text{integer-moded sine oscillators}.
$$

The spatial gradient contributes to the worldsheet Hamiltonian

$$
\frac1{4\pi\alpha'}\int_0^\pi d\sigma\sum_I(X'^I)^2=\frac{d^2}{4\pi^2\alpha'}.
$$

Parallel branes have integer modes in their NN and DD directions, so their oscillator vacuum energy is still $-1$. The zero-mode [Virasoro constraint](../../../../../virasoro-constraint.md) is consequently

$$
\alpha'(-E^2+k_\parallel^2)+\frac{d^2}{4\pi^2\alpha'}+N-1=0.
$$

With [string tension](../../../../../string-tension.md) $T=1/(2\pi\alpha')$, the [Open string stretched between D-branes](../../../../../open-string-stretched-between-d-branes.md) has

$$
\boxed{M_N^2=(Td)^2+\frac{N-1}{\alpha'}.}
$$

The classical stretching energy is $Td$, while the quantum ground-state energy, when real, is

$$
\boxed{E_0(k_\parallel)=\sqrt{k_\parallel^2+\frac{d^2}{4\pi^2\alpha'^2}-\frac1{\alpha'}},\qquad
E_0(0)=\sqrt{(Td)^2-\frac1{\alpha'}}.}
$$

The vacuum correction is an additive term in energy squared, not a constant subtraction from the classical stretching energy. It follows that the [bosonic stretched-string tachyon threshold](../../../../../bosonic-stretched-string-tachyon-threshold.md) is

$$
\boxed{d_0=2\pi\sqrt{\alpha'},\qquad M_0^2<0\ \Longleftrightarrow\ d<d_0.}
$$

Below this threshold the lowest state is a [tachyon](../../../../../tachyon.md): small-momentum modes have imaginary frequency and the background is unstable, rather than having an ordinary real negative ground-state energy. It is massless at the threshold. The assumption of parallel branes is needed for the integer moding used here; relative angles change the vacuum contribution.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
