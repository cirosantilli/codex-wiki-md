<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take $0\le\sigma\le\pi$ and split the coordinates into $a=0,\ldots,p$ along the branes and $I=p+1,\ldots,25$ transverse to them. In [conformal gauge](../../../../../conformal-gauge.md) the [wave equation](../../../../../wave-equation-split.md) permits a separated mode $e^{-i\omega\tau}f(\sigma)$ with $f''+\omega^2f=0$. For [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) at both ends, $f'(0)=f'(\pi)=0$ selects $\cos m\sigma$ and [integer](../../../../../integer.md) $m$. The zero-frequency solution is independent of $\sigma$, with a constant position and a term linear in time. Therefore the [open-string mode expansion](../../../../../open-string-mode-expansion.md) is

$$
X^a=x^a+2\alpha'k^a\tau+i\sqrt{2\alpha'}\sum_{m\ne0}\frac{\alpha_m^a}{m}e^{-im\tau}\cos m\sigma.
$$

The [canonical momentum](../../../../../canonical-momentum.md) density integrated over this interval is $k^a$.

For [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), subtract the static interpolation between fixed endpoint positions $y_0^I$ and $y_\pi^I$. The remaining field vanishes at both ends, selecting $\sin m\sigma$ with [integer](../../../../../integer.md) $m$ and excluding a [momentum](../../../../../momentum.md) [worldsheet zero mode](../../../../../worldsheet-zero-mode.md). The expansion is

$$
\boxed{X^I=y_0^I+\frac{y_\pi^I-y_0^I}{\pi}\sigma+\sqrt{2\alpha'}\sum_{m\ne0}\frac{\alpha_m^I}{m}e^{-im\tau}\sin m\sigma.}
$$

Here $\alpha_m^{I\dagger}=\alpha_{-m}^I$. There is no factor $i$ in the [sine series](../../../../../fourier-sine-series.md) with this reality convention: changing $m$ to $-m$ reverses both the sine and the denominator. These are the [integer-mode expansion with parallel D-brane endpoints](../../../../../integer-mode-expansion-with-parallel-d-brane-endpoints.md); they are not the half-integer modes of a coordinate with a Neumann condition at one endpoint and a Dirichlet condition at the other.

The endpoints can move on $(p+1)$-dimensional [worldvolumes](../../../../../worldvolume.md) but are fixed in the transverse directions. Thus these are [open strings](../../../../../open-string.md) attached to [D-branes](../../../../../d-brane.md), or stretched between parallel [D-branes](../../../../../d-brane.md) at $y_0$ and $y_\pi$. The tangential [momenta](../../../../../momentum.md) describe propagation on the brane; the transverse positions describe its embedding. Let $L=|y_\pi-y_0|$. The linear spatial [worldsheet zero mode](../../../../../worldsheet-zero-mode.md) contributes $L^2/(4\pi^2\alpha')$ to $L_0$. Quantization with [string intercept](../../../../../normal-ordering-constant-of-a-string.md) one gives

$$
\boxed{M^2=\frac{L^2}{4\pi^2\alpha'^2}+\frac{N-1}{\alpha'}.}
$$

The first term is also the square of the classical stretched-string energy $TL$, since the [string tension](../../../../../string-tension.md) is $T=1/(2\pi\alpha')$.

For two coincident [D3-branes](../../../../../d3-brane.md), label the ends of an oriented [open string](../../../../../open-string.md) by $i,j\in\{1,2\}$. The four endpoint combinations give [Chan-Paton factors](../../../../../chan-paton-factor.md) $\lambda_{ij}$, which form the full algebra of $2\times2$ [matrices](../../../../../matrix.md). Under a change of brane basis these transform as $\lambda\mapsto U\lambda U^{-1}$, the [adjoint action](../../../../../adjoint-representation-of-a-lie-group.md) of $U(2)$. At $L=0$, the first oscillator level is massless. Its tangential polarization supplies a four-dimensional vector $A_a$, while the 22 [transverse polarizations](../../../../../transverse-polarization.md) supply real adjoint [scalar fields](../../../../../scalar-field.md) $\Phi^I$. This is the [bosonic D3-brane low-energy field content](../../../../../bosonic-d3-brane-low-energy-field-content.md).

The endpoint [matrices](../../../../../matrix.md) multiply in their boundary order in disk amplitudes. The difference between the two orders in the three-vector interaction gives the [matrix commutator](../../../../../commutator.md); the kinematic factor is the one-derivative [Yang-Mills theory](../../../../../yang-mills-theory.md) cubic vertex. Factorization and the vector [gauge redundancy](../../../../../gauge-redundancy.md) then supply the quartic interaction with the same [commutator](../../../../../commutator.md). Equivalently, the leading low-energy action is the [dimensional reduction](../../../../../dimensional-reduction.md) of 26-dimensional [Yang-Mills theory](../../../../../yang-mills-theory.md), with

$$
F_{ab}=\partial_aA_b-\partial_bA_a-i[A_a,A_b],\qquad D_a\Phi^I=\partial_a\Phi^I-i[A_a,\Phi^I],
$$



$$
S_{\mathrm{low}}=\frac1{g_{\mathrm{YM}}^2}\int d^4x\,\operatorname{Tr}\left(-\frac14F_{ab}F^{ab}-\frac12D_a\Phi^I D^a\Phi^I+\frac14[\Phi^I,\Phi^J][\Phi^I,\Phi^J]\right)+\cdots.
$$

For Hermitian [scalar fields](../../../../../scalar-field.md) the last displayed term corresponds to a nonnegative potential, because their [commutators](../../../../../commutator.md) are anti-Hermitian. Higher-derivative terms are suppressed at energies well below $1/\sqrt{\alpha'}$. **Ignoring the [tachyon](../../../../../tachyon.md), the gauge sector is four-dimensional $U(2)$ [Yang-Mills theory](../../../../../yang-mills-theory.md), accompanied by 22 adjoint [scalar fields](../../../../../scalar-field.md).** It is not pure [Yang-Mills theory](../../../../../yang-mills-theory.md), nor the supersymmetric six-scalar [D3-brane](../../../../../d3-brane.md) theory of a ten-dimensional superstring.

Separate the two branes and use the [D-brane scalar-position normalization](../../../../../d-brane-scalar-position-normalization.md)

$$
\langle\Phi^I\rangle=\frac1{2\pi\alpha'}\begin{pmatrix}y_1^I&0\\0&y_2^I\end{pmatrix}.
$$

A [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md) preserves this [expectation value](../../../../../expectation-value.md) only when it is diagonal if $y_1\ne y_2$. Thus the unbroken [group](../../../../../group-split.md) is $U(1)\times U(1)$. The [scalar field](../../../../../scalar-field.md) [kinetic term](../../../../../kinetic-term.md) supplies a mass for the off-diagonal vectors, since

$$
[A_a,\langle\Phi^I\rangle]_{12}=\frac{y_2^I-y_1^I}{2\pi\alpha'}(A_a)_{12}.
$$

Summing over $I$ gives $m_{12}^2=L^2/(4\pi^2\alpha'^2)$, exactly the mass of the stretched $N=1$ string. The two diagonal gauge vectors remain massless. This identifies brane separation with an adjoint [Higgs mechanism](../../../../../higgs-mechanism.md), rather than an explicit deletion of the off-diagonal strings.

For the [ground state](../../../../../ground-state.md) of an [open string](../../../../../open-string.md) joining the two different branes, $N=0$, so the [bosonic stretched-string tachyon threshold](../../../../../bosonic-stretched-string-tachyon-threshold.md) is

$$
\boxed{M_0^2<0\quad\Longleftrightarrow\quad L<2\pi\sqrt{\alpha'}.}
$$

At equality it is massless, and above it the stretched [ground state](../../../../../ground-state.md) has positive mass squared. The same-brane ground strings still have $M_0^2=-1/\alpha'$; this calculation removes only the stretched-string instability, not the original instability of the bosonic branes.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
