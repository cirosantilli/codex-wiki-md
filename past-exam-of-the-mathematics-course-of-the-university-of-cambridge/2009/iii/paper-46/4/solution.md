<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [string nonlinear sigma model](../../../../../string-nonlinear-sigma-model.md) regards the target-space metric, the [Kalb–Ramond field](../../../../../kalb-ramond-field.md) and the [dilaton](../../../../../dilaton.md) as couplings of the two-dimensional worldsheet theory. Schematically its Euclidean terms are

$$
\frac{1}{4\pi\alpha'}\int\sqrt h\,h^{ab}G_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu
+\frac{i}{4\pi\alpha'}\int\epsilon^{ab}B_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu
+\frac{1}{4\pi}\int\sqrt h\,\Phi(X)R^{(2)}.
$$

Quantization produces running background couplings and a possible [worldsheet Weyl anomaly](../../../../../worldsheet-weyl-anomaly.md). Gauge-fixed matter bosons contribute [central charge](../../../../../central-charge.md) $D$, while the reparameterization [bc ghost system](../../../../../bc-system.md) contributes $-26$ in each chirality. In the critical flat background cancellation therefore requires $D=26$. In a curved background, vanishing improved [sigma-model beta functions](../../../../../sigma-model-beta-function.md) further imposes field equations for $G,B,\Phi$. For example, the leading metric condition is

$$
R_{\mu\nu}-\tfrac14H_{\mu\rho\sigma}H_\nu{}^{\rho\sigma}+2\nabla_\mu\nabla_\nu\Phi=0,\qquad H=dB.
$$

These are spacetime conditions because the couplings are functions of the embedding coordinates, not additional worldsheet coordinates.

The leading equations arise by varying the [string-frame massless effective action](../../../../../string-frame-massless-effective-action.md)

$$
\boxed{S_{\mathrm{eff}}=\frac1{2\kappa_0^2}\int d^{26}X\,\sqrt{-G}\,e^{-2\Phi}
\left[R+4(\nabla\Phi)^2-\frac1{12}H_{\mu\nu\rho}H^{\mu\nu\rho}+O(\alpha')\right].}
$$

The factor $e^{-2\Phi}$ is the sphere contribution in the [string genus expansion](../../../../../string-genus-expansion.md). Higher sigma-model orders generate higher-derivative terms in the $\alpha'$ expansion; higher genera give string-loop corrections. Thus conformal consistency of the quantum worldsheet determines the low-energy target equations and their action. This is a massless-sector truncation: the bosonic [tachyon](../../../../../tachyon.md) is not removed by writing an action only for $G,B,\Phi$.

For a brane embedding $X^\mu(\xi)$, the [D-brane worldvolume pullbacks](../../../../../d-brane-worldvolume-pullbacks.md) are

$$
\boxed{\gamma_{ab}=G_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu,\qquad
B_{ab}=B_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu.}
$$

The [dilaton](../../../../../dilaton.md) is evaluated at the embedding. When $T_p$ denotes the physical tension in a background with constant mode $\Phi_0$, the convention is $\widetilde\Phi=\Phi(X)-\Phi_0$, so $e^{-\widetilde\Phi}=1$ in that vacuum. Equivalently one can use $\widetilde\Phi=\Phi(X)$ and a coefficient with the constant $e^{-\Phi_0}$ not already included. The physics is the same; the two conventions must not count that constant factor twice.

Several features motivate the [Dirac-Born-Infeld action](../../../../../dirac-born-infeld-action.md). Without gauge or two-form fields, it is the relativistic induced-volume action for a tensionful extended object. An open-string boundary couples to its gauge potential $A$, so a bulk transformation $B\mapsto B+d\Lambda$ is canceled by $A\mapsto A-P[\Lambda]/(2\pi\alpha')$. Thus only $P[B]+2\pi\alpha'F$ can enter. For slowly varying constant field strength, the open-string disk partition function resums its dependence into the determinant; expansion gives the Maxwell kinetic term. The disk has [Euler characteristic](../../../../../euler-characteristic.md) one, giving $e^{-\Phi}$ rather than the closed-string sphere's $e^{-2\Phi}$. [Worldvolume](../../../../../worldvolume.md) covariance and the induced metric then combine these ingredients into the determinant expression.

Explicitly, in flat background and static gauge $X^a=\xi^a$ with transverse fluctuations $X^I$, the weak-field expansion starts as

$$
\sqrt{-\det(\eta_{ab}+\partial_aX^I\partial_bX^I+2\pi\alpha'F_{ab})}
=1+\frac12\partial_aX^I\partial^aX^I+\frac{(2\pi\alpha')^2}{4}F_{ab}F^{ab}+\cdots.
$$

The linear term in the antisymmetric matrix $F$ vanishes; the quadratic term follows from expanding $\tfrac12\operatorname{Tr}\log(1+2\pi\alpha'\eta^{-1}F)$. Thus the [DBI action](../../../../../dirac-born-infeld-action.md) contains both the scalar and gauge kinetic energies, while higher powers and derivatives are string-scale corrections.

For two coincident [D-branes](../../../../../d-brane.md), an oriented open string has independent labels $r,s\in\{1,2\}$ at its ends. Its [Chan-Paton factors](../../../../../chan-paton-factor.md) are the matrix units $E_{rs}$. The four massless vector modes span the Lie algebra of $U(2)$: diagonal strings supply the two Abelian fields, and oppositely oriented interbrane strings supply the off-diagonal modes. Joining strings multiplies these matrices, producing the non-Abelian commutators. Transverse vector polarizations become [adjoint scalar fields](../../../../../adjoint-scalar-field.md). This is [Coincident-D-brane gauge enhancement](../../../../../coincident-d-brane-gauge-enhancement.md).

The massless gauge/scalar dynamics reduce to dimensionally reduced [Yang-Mills theory](../../../../../yang-mills-theory.md) in a flat background with constant [dilaton](../../../../../dilaton.md) and vanishing pulled-back $B$, at energies and field variations well below the string scale. More precisely, derivative corrections satisfy $\alpha'E^2\ll1$, and one expands in small dimensionless field strengths and scalar gradients rather than retaining the full nonlinear determinant. Weak [string coupling](../../../../../string-coupling.md) suppresses loop corrections. After subtracting the constant brane vacuum energy and using the scalar normalization fixed below, the coefficient is

$$
\boxed{g_{\mathrm{YM}}^{-2}=(2\pi\alpha')^2T_p.}
$$

A bosonic brane additionally has an open-string [tachyon](../../../../../tachyon.md); the displayed action governs its massless sector and is not a stable complete truncation. For supersymmetric branes the corresponding leading action also has the massless fermions.

There is a sign qualification in the printed scalar potential. With the stated $D_a\phi=\partial_a\phi+i[A_a,\phi]$, take $A_a,\phi^I$ Hermitian and $[\phi^I,\phi^J]^2$ to mean the literal matrix product. Then dimensional reduction has

$$
F_{aI}=D_a\phi^I,\qquad F_{IJ}=i[\phi^I,\phi^J].
$$

Consequently $F_{IJ}F^{IJ}=-[\phi^I,\phi^J]^2$. The consistent low-energy action is

$$
S_{\mathrm{YM}}=-\frac1{g_{\mathrm{YM}}^2}\int d^{p+1}\xi\,\operatorname{Tr}
\left[\frac14F_{ab}F^{ab}+\frac12D_a\phi^ID^a\phi^I-\frac14\sum_{I\ne J}[\phi^I,\phi^J]^2\right].
$$

This is the [Hermitian commutator potential in D-brane Yang-Mills theory](../../../../../hermitian-commutator-potential-in-d-brane-yang-mills-theory.md). Its potential energy is $-\sum\operatorname{Tr}[\phi^I,\phi^J]^2/(4g_{\mathrm{YM}}^2)\geq0$, because a Hermitian-matrix commutator is anti-Hermitian. For a concrete check, take $\phi^1=v\sigma_1$, $\phi^2=v\sigma_2$ with [Pauli matrices](../../../../../pauli-matrices.md). Then $[\phi^1,\phi^2]^2=-4v^4I$, so the literal printed plus sign would make the static energy negative and unbounded below. The printed plus sign is consistent only if its square denotes the positive norm $[\phi^I,\phi^J]^\dagger[\phi^I,\phi^J]$, rather than a literal square. The gauge-boson mass calculation below uses the unambiguous kinetic terms.

In an ordinary separated-brane vacuum the scalar expectation values commute and can be simultaneously diagonalized:

$$
\langle\phi^I\rangle=\begin{pmatrix}v_1^I&0\\0&v_2^I\end{pmatrix}.
$$

Their eigenvalue vectors specify the transverse positions, up to the normalization to be determined. The trace encodes the center of mass; their difference encodes separation. When the two vectors coincide, every $U(2)$ transformation commutes with the vacuum. When they are distinct, only independent diagonal phases do, so **the unbroken group is $U(1)\times U(1)$**. The off-diagonal vectors acquire mass by the [Higgs mechanism](../../../../../higgs-mechanism.md).

Write the off-diagonal entries of $A_a$ as $W_a$ and $W_a^*$ and put $\Delta v^I=v_1^I-v_2^I$. At a constant diagonal vacuum, $D_a\phi^I=i[A_a,\langle\phi^I\rangle]$, so

$$
\operatorname{Tr}(D_a\phi^ID^a\phi^I)=2(\Delta v^I)^2W_a^*W^a.
$$

The quadratic off-diagonal gauge kinetic term is $-f_{ab}^*f^{ab}/(2g_{\mathrm{YM}}^2)$ with $f_{ab}=\partial_aW_b-\partial_bW_a$, and the scalar kinetic term supplies $-\sum_I(\Delta v^I)^2W_a^*W^a/g_{\mathrm{YM}}^2$. Comparing these with the complex massive-vector action gives

$$
\boxed{m_W^2=\sum_I(v_1^I-v_2^I)^2.}
$$

Here the term W-boson means this broken-generator vector, not specifically an electroweak particle. The normalization places the gauge coupling outside the action, so no extra $g_{\mathrm{YM}}$ multiplies these $v_r^I$; rescaling to canonically normalized [scalar fields](../../../../../scalar-field.md) moves that coupling into the usual Higgs mass formula.

The corresponding open-string vector oscillator stretched over distance $L=|X_1-X_2|$ has classical stretching mass $TL=L/(2\pi\alpha')$. Its unstretched mass contribution vanishes because it is the vector level, rather than the bosonic [tachyon](../../../../../tachyon.md) level. Equating it with the gauge-theory mass gives

$$
\boxed{|X_1-X_2|=2\pi\alpha'|v_1-v_2|,\qquad X_r^I=2\pi\alpha'v_r^I.}
$$

The component relation follows by rotational covariance and a common choice of transverse origin; a uniform translation adds the same constant to both brane coordinates. This is the [D-brane scalar-position normalization](../../../../../d-brane-scalar-position-normalization.md). Together with the [string tension](../../../../../string-tension.md) determined in Question 1, it fixes the exact normalization of scalar eigenvalues as brane positions.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
