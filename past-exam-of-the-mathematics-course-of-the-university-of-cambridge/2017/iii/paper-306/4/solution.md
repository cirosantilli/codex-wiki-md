<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [Majorana spinor](../../../../../majorana-spinor.md) equals its [charge conjugation](../../../../../charge-conjugation.md), $\psi^c=C\bar\psi^{\,T}=\psi$, with conventional phase choices absorbed into $C$. The two-component [worldsheet Majorana fermion](../../../../../worldsheet-majorana-fermion.md) therefore has no independent complex conjugate components; in a Majorana representation its components can be real [Grassmann variables](../../../../../grassmann-variable.md). The same condition applies to the constant supersymmetry parameter. Grassmann statistics matter in the variation: replacing the spinors by commuting numerical vectors would give the wrong bilinear interchange signs.

The displayed rigid transformation is understood in flat [conformal gauge](../../../../../conformal-gauge.md). Take $h_{\mu\nu}=\eta_{\mu\nu}=\operatorname{diag}(-1,1)$, $\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}$, and choose

$$
\gamma^0=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
\gamma^1=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad\bar\psi=\psi^T\gamma^0.
$$

Here $C=\gamma^0$ is a valid invariant charge-conjugation form: $C^T=-C$ and $(\gamma^\mu)^TC=-C\gamma^\mu$. These concrete matrices make all signs checkable; equivalent Majorana conventions give the same result with their consistently transformed bars.

Let $A=\sqrt{\alpha'/2}$ and $B=1/\sqrt{2\alpha'}$, so $\alpha'B=A$. Suppressing the common factor $-1/(4\pi\alpha')$ in the action, the flat kinetic density is

$$
\mathcal L_0=\partial_\mu X^a\partial^\mu X_a+i\alpha'\bar\psi^a\gamma^\mu\partial_\mu\psi_a.
$$

The rigid variations have $\delta X^a=iA\bar\epsilon\psi^a$ and $\delta\psi^a=B\gamma^\nu\partial_\nu X^a\epsilon$. The supersymmetry variation is even, so its product rule has no extra graded sign. From the [Majorana Grassmann bilinear interchange](../../../../../majorana-grassmann-bilinear-interchange.md) identities,

$$
\delta\bar\psi^a=-B\bar\epsilon\gamma^\nu\partial_\nu X^a,\qquad
\bar\psi^a\epsilon=\bar\epsilon\psi^a,\qquad
\bar\psi^a\gamma^\mu\gamma^\nu\epsilon=\bar\epsilon\gamma^\nu\gamma^\mu\psi^a.
$$

For example the last identity follows by moving the Grassmann-odd parameter through $\psi$, then using $C^T=-C$ and the transpose relations twice. No equation of motion has been used.

The two kinetic variations are

$$
\delta\mathcal L_B=2iA\partial^\mu X_a\bar\epsilon\partial_\mu\psi^a,
$$



$$
\delta\mathcal L_F=-iA\partial_\nu X_a\bar\epsilon\gamma^\nu\gamma^\mu\partial_\mu\psi^a+iA\bar\psi_a\gamma^\mu\gamma^\nu\epsilon\,\partial_\mu\partial_\nu X^a.
$$

The [Clifford algebra](../../../../../clifford-algebra.md) turns the first fermionic term plus the bosonic variation into $iA\partial_\nu X_a\bar\epsilon\gamma^\mu\gamma^\nu\partial_\mu\psi^a$. In the second term, commute the [partial derivatives](../../../../../partial-derivative.md) and use the same algebra: the antisymmetric gamma product drops out, leaving $iA\Box X_a\bar\epsilon\psi^a$. Together they are precisely the [rigid worldsheet supersymmetry boundary term](../../../../../rigid-worldsheet-supersymmetry-boundary-term.md):

$$
\boxed{\delta\mathcal L_0=\partial_\mu J^\mu,\qquad J^\mu=i\sqrt{\frac{\alpha'}2}\,\partial_\nu X_a\bar\epsilon\gamma^\mu\gamma^\nu\psi^a.}
$$

Therefore $\delta S=-(4\pi\alpha')^{-1}\int_{\partial\Sigma}d\Sigma_\mu\,J^\mu$. It vanishes on a closed or periodic worldsheet, for compactly supported changes, or under compatible supersymmetric endpoint conditions. The local total-derivative identity is off shell; the boundary assumptions are needed to call the integrated action invariant.

The flat-gauge qualification is substantive. On an arbitrary curved worldsheet, spinors need a [zweibein](../../../../../zweibein.md) and [spin connection](../../../../../spin-connection.md) and a constant spinor parameter need not exist. A fully covariant locally supersymmetric action also involves the [worldsheet gravitino](../../../../../worldsheet-gravitino.md); the isolated ordinary-derivative expression does not prove rigid invariance for arbitrary $h_{\mu\nu}$. We have proved the intended rigid symmetry of its flat gauge-fixed action, with the fermionic term inside the same integral and overall normalization. If the displayed last term were read as outside the integral, it would not even define an action.

For phenomenology, [bosonic string theory](../../../../../bosonic-string-theory.md) has no spacetime [fermions](../../../../../fermion.md) and its usual vacuum contains a [tachyon](../../../../../tachyon.md). The [spinning string](../../../../../spinning-string.md) has a [Ramond sector](../../../../../ramond-sector.md), whose fermionic zero modes form a spacetime [Clifford algebra](../../../../../clifford-algebra.md) and give spacetime spinor states, as well as a [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md). In suitable consistent theories the [GSO projection](../../../../../gso-projection.md) removes the tachyonic NS ground state and keeps the appropriate Ramond chirality. The [critical dimension of the RNS superstring](../../../../../critical-dimension-of-the-rns-superstring.md) is 10 rather than 26: $D$ [bosons](../../../../../boson.md) and $D$ real [fermions](../../../../../fermion.md) have matter [central charge](../../../../../central-charge.md) $3D/2$ per chiral sector, while the reparameterization and superconformal ghosts contribute $-26+11=-15$, so the total anomaly cancels at $D=10$.

**Suitable GSO-projected superstrings admit spacetime [fermions](../../../../../fermion.md) and a tachyon-free spectrum, making them more promising for particle physics than the bosonic string.** Rigid [worldsheet supersymmetry](../../../../../worldsheet-supersymmetry.md) alone does not establish a tachyon-free spacetime theory or realistic phenomenology. The projection, consistent sectors and [compactification in string theory](../../../../../compactification-in-string-theory.md) are additional input; spacetime supersymmetry and a realistic four-dimensional spectrum are not automatic consequences of this classical action.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 306](../../paper-306-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
