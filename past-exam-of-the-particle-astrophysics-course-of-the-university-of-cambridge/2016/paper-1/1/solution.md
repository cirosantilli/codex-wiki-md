<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The known active [neutrinos](../../../../neutrino.md) are too light and too fast to supply the dominant [cold dark matter](../../../../cold-dark-matter.md). Their relativistic decoupling leaves substantial [free streaming](../../../../free-streaming.md), which erases rather than seeds sufficiently small-scale structure; their allowed [mass](../../../../mass.md) density is also inadequate for the dominant cold component. Changing a light active [neutrino](../../../../neutrino.md) from Dirac to Majorana does not remove those problems. What can change the picture is an enlarged neutral-fermion sector containing sterile states with different [masses](../../../../mass.md), production and decay rates. A sufficiently long-lived [sterile neutrino](../../../../sterile-neutrino.md) in a Majorana state can be a dark-matter candidate; Majorana character alone supplies neither stability nor the correct abundance.

For the [spinor](../../../../spinor.md) calculation, put $a=p_z/(E+m)$ and define $A=N(1-a)/2$, $B=N(1+a)/2$. Applying the given [chiral projectors](../../../../chiral-projector.md) gives

$$
U_{1L}=A\begin{pmatrix}1\\0\\-1\\0\end{pmatrix},\qquad
U_{1R}=B\begin{pmatrix}1\\0\\1\\0\end{pmatrix},\qquad
V_{2R}=B\begin{pmatrix}1\\0\\1\\0\end{pmatrix}.
$$

Consequently

$$
\overline U_{1R}U_{1L}=2AB
=\frac{E+m}{2}\left(1-\frac{p_z^2}{(E+m)^2}\right)=m,
\qquad
\overline V_{2R}U_{1L}=2AB=m,
$$

where the last equality uses $E^2-p_z^2=m^2$. Same-chirality [Lorentz scalar](../../../../lorentz-scalar.md) products instead vanish: for example $\overline U_{1L}U_{1L}=0$. The nonzero overlaps demonstrate the [Lorentz scalar](../../../../lorentz-scalar.md) structures coupling left and right [chirality](../../../../chirality-physics.md). For $U$ to $U$ this is a particle-number-preserving Dirac coupling; for $U$ to the charge-conjugate $V$ sector it can describe a lepton-number-violating Majorana coupling.

There is a normalization subtlety: both displayed overlaps equal the on-shell [mass](../../../../mass.md) parameter used to define the [spinors](../../../../spinor.md). A [chiral scalar spinor overlap](../../../../chiral-scalar-spinor-overlap.md) verifies a coupling structure without fixing an independent Lagrangian coefficient $M_L$. Repeating the on-shell construction with mass parameter $M_L$ would instead give the corresponding overlap $M_L$; this is a different input, rather than a newly derived parameter. The independent coefficients of a [Dirac mass term](../../../../dirac-mass-term.md) and a [Majorana mass term](../../../../majorana-mass-term.md) are defined by

$$
\mathcal L_m=-m(\bar\nu_R\nu_L+\bar\nu_L\nu_R)
-\frac12\left(M_L\overline{\nu_L^c}\nu_L+
M_R\overline{\nu_R^c}\nu_R+\mathrm{h.c.}\right).
$$

The Majorana terms connect a field with its charge conjugate and violate the corresponding continuous [lepton](../../../../lepton.md) phase symmetry by two units. With only unbroken [Standard Model](../../../../standard-model-split.md) [gauge symmetry](../../../../gauge-invariance.md), a left-handed Majorana [mass](../../../../mass.md) also requires [electroweak symmetry breaking](../../../../electroweak-symmetry-breaking.md) or an appropriate higher-dimensional operator; it is not an arbitrary gauge-invariant bare [mass](../../../../mass.md) for a [lepton](../../../../lepton.md) doublet.

Use an all-left-handed Weyl [basis](../../../../basis.md) $\mathbf n_L=(\nu_L,\nu_R^c)^T$. For real parameters the [one-family Dirac-Majorana mass matrix](../../../../one-family-dirac-majorana-mass-matrix.md) is

$$
\boxed{\mathcal M=\begin{pmatrix}M_L&m\\m&M_R\end{pmatrix},\qquad
\mathcal L_m=-\frac12\overline{\mathbf n_L^{\,c}}\mathcal M\mathbf n_L+\mathrm{h.c.}}
$$

Writing $(\nu_{1L},\nu_{2L})^T=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}(\nu_L,\nu_R^c)^T$ gives an orthogonal diagonalization, with $\tan2\theta=2m/(M_R-M_L)$ up to the rotation-sign convention. Massive-particle [chirality](../../../../chirality-physics.md) and [helicity](../../../../helicity.md) are not identical; the familiar left/right [helicity](../../../../helicity.md) language becomes an approximation in the relativistic regime.

The [characteristic polynomial](../../../../characteristic-polynomial.md) is

$$
\det(\mathcal M-\lambda\mathbf1)
=\lambda^2-(M_L+M_R)\lambda+M_LM_R-m^2.
$$

Its roots are

$$
\boxed{\lambda_\pm=\frac12\left[M_R+M_L\pm
\sqrt{(M_R-M_L)^2+4m^2}\right].}
$$

For Majorana [fermions](../../../../fermion.md) the nonnegative physical [masses](../../../../mass.md), as explained by [physical Majorana mass and signed eigenvalue](../../../../physical-majorana-mass-and-signed-eigenvalue.md), are $|\lambda_\pm|$ after a possible field rephasing; a negative real [eigenvalue](../../../../eigenvalue.md) is not a negative physical [rest mass](../../../../invariant-mass.md). When $M_R\gg |m|,|M_L|$,

$$
\lambda_{\rm light}\simeq M_L-\frac{m^2}{M_R},\qquad
\lambda_{\rm heavy}\simeq M_R+\frac{m^2}{M_R}.
$$

The light state is predominantly $\nu_L-(m/M_R)\nu_R^c$, while the heavy state is predominantly $\nu_R^c+(m/M_R)\nu_L$. Each [mass](../../../../mass.md) [eigenstate](../../../../eigenstate.md) combines its Weyl component and charge conjugate to form a Majorana field.

For $M_R=10^{12}\,\mathrm{GeV}$, **the heavy [mass](../../../../mass.md) is approximately $10^{12}\,\mathrm{GeV}$**. In the type-I limit $M_L\simeq0$,

$$
\boxed{m_{\rm light}\simeq10^{-3}
\left(\frac{m}{1\,\mathrm{GeV}}\right)^2\,\mathrm{eV}.}
$$

The [seesaw light-mass estimate needs a Dirac scale](../../../../seesaw-light-mass-estimate-needs-a-dirac-scale.md): no unique numerical light [mass](../../../../mass.md) follows because the Dirac [mass](../../../../mass.md) and $M_L$ were not supplied. As an explicitly conditional illustration, choosing $m=100\,\mathrm{GeV}$ and $M_L=0$ gives $10\,\mathrm{eV}$; this is an assumed Dirac scale, not additional exam data or a prediction from $M_R$ alone. A heavy seesaw state is also not automatically stable enough to be [dark matter](../../../../dark-matter.md).

<a id="1/image-a-large-right-handed-mass-produces-reciprocal-light-and-heavy-scales"></a>
![](../../../../past-exam-of-the-particle-astrophysics-course-of-the-university-of-cambridge/2016/paper-1-seesaw-scales.png)

**[Figure 1](#1/image-a-large-right-handed-mass-produces-reciprocal-light-and-heavy-scales). A large right-handed mass produces reciprocal light and heavy scales**. Original exact one-family [eigenvalues](../../../../eigenvalue.md) for $M_L=0$, expressed relative to an unspecified fixed Dirac [mass](../../../../mass.md). Negative signed [eigenvalues](../../../../eigenvalue.md) are shown by their positive physical [masses](../../../../mass.md); no numerical Dirac [mass](../../../../mass.md) is assumed.

The conventional minimal [Pati-Salam model](../../../../pati-salam-model.md) [gauge group](../../../../gauge-group.md) is

$$
\boxed{SU(4)_C\times SU(2)_L\times SU(2)_R.}
$$

The group printed in this paper is different: it contains two $SU(4)$ factors and only one $SU(2)$. This is a discrepancy in the original PDF, not just in the transcription. The standard-model discussion below uses the conventional intended [Pati-Salam model](../../../../pati-salam-model.md) model. A literal theory with the printed product would require additional [fermion](../../../../fermion.md) representations and symmetry-breaking data that are not specified.

The [Pati-Salam model](../../../../pati-salam-model.md) unifies the three [quark](../../../../quark.md) [color charges](../../../../color-charge.md) with [lepton number](../../../../lepton-number.md) as a fourth [color charge](../../../../color-charge.md). A family forms $(4,2,1)$ left-handed and $(4,1,2)$ right-handed multiplets, including a [right-handed neutrino](../../../../right-handed-neutrino.md). The extended [color charge](../../../../color-charge.md) group contains quark-lepton [gauge bosons](../../../../gauge-boson.md), while the right-handed weak factor supplies right-handed charged currents after symmetry breaking. The [Pati-Salam charge embedding](../../../../pati-salam-charge-embedding.md) is

$$
Q=T_{3L}+T_{3R}+\frac{B-L}{2}.
$$

The original paper explicitly develops the smaller local subgroup $SU(2)_L\times SU(2)_R\times SU(4)_C$, as well as a larger underlying global structure; neither distinction licenses silently replacing the printed group.[§II.B, equation (2), printed p. 276; §II.C, charge assignments](../../../../lepton-number-as-the-fourth-color-by-jogesh-pati-and-abdus-salam.md) The product group is a quark-lepton unification scheme rather than a simple [gauge group](../../../../gauge-group.md) with one automatically common coupling. Breaking the right-handed and $B-L$ symmetries can generate a large $M_R$ and light/heavy [Majorana neutrinos](../../../../majorana-neutrino.md) through the seesaw. The [gauge group](../../../../gauge-group.md) alone does not uniquely fix their [masses](../../../../mass.md) or guarantee a dark-matter lifetime.

The most important laboratory test of Majorana character is [neutrinoless double beta decay](../../../../neutrinoless-double-beta-decay.md),

$$
(A,Z)\longrightarrow(A,Z+2)+e^-+e^-,
$$

with no outgoing [neutrinos](../../../../neutrino.md). Under light-neutrino exchange, the amplitude involves

$$
m_{\beta\beta}=\left|\sum_iU_{ei}^{\,2}m_i\right|,\qquad
[T_{1/2}^{0\nu}]^{-1}=G_{0\nu}|\mathcal M_{0\nu}|^2
\left|\frac{m_{\beta\beta}}{m_e}\right|^2.
$$

The coherent squared mixing elements allow phase cancellations. A null result constrains this combination within the assumed mechanism, rather than proving that all [neutrinos](../../../../neutrino.md) are Dirac.

The observable is a peak in summed electron [energy](../../../../energy-split.md) at the decay [Q value](../../../../q-value.md), unlike the continuous two-neutrino spectrum. Enriched source material, large exposure, good [energy](../../../../energy-split.md) resolution, underground operation and radiopure construction suppress backgrounds. [germanium](../../../../germanium.md) arrays use the source as a semiconductor detector; [xenon](../../../../xenon.md) time-projection chambers combine [ionization](../../../../ionization.md), light and event-position information; [bolometers](../../../../bolometer.md) measure deposited [energy](../../../../energy-split.md) through a [temperature](../../../../temperature-split.md) rise. The GERDA collaboration's Phase-I study is a concrete example of an enriched-germanium source-detector search with background suppression.[Abstract and Phase-I source-detector method, arXiv:1307.4720](../../../../results-on-neutrinoless-double-beta-decay-of-76ge-from-gerda-phase-i-by-the-gerda-collaboration.md) [energy](../../../../energy-split.md) calibration, resolution tails, radon and material backgrounds, cosmic-ray vetoes, signal-like event [topology](../../../../topology-split.md) and sideband fits all need independent checks before a Q-value excess is convincing. Collider same-sign dilepton processes can test heavier Majorana states, but require a specified production and decay mechanism. **Lepton-number violation, absolute-mass measurements and oscillation data provide complementary information; oscillations alone do not settle Majorana character.**

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the particle Astrophysics course of the University of Cambridge](../../../split.md)
5. [Particle Astrophysics course of the University of Cambridge](../../../../particle-astrophysics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
