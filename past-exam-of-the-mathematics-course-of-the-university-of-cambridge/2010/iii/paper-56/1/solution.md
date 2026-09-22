<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use mostly-plus Lorentzian signature and $\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}$, with antisymmetrized gamma products of unit weight. A [Majorana spinor](../../../../../majorana-spinor.md) obeys a reality condition under [charge conjugation](../../../../../charge-conjugation.md):

$$
\boxed{\psi^c=C\overline\psi^{\,T}=\psi,\qquad C\gamma^\mu C^{-1}=-(\gamma^\mu)^T.}
$$

A [Weyl spinor](../../../../../weyl-spinor.md) instead has definite [chirality](../../../../../chirality-physics.md),

$$
\boxed{P_\pm\psi=\psi,\qquad P_\pm=\tfrac12(1\pm\gamma_5).}
$$

A four-dimensional [Majorana spinor](../../../../../majorana-spinor.md) has four real components, while a [Weyl spinor](../../../../../weyl-spinor.md) has two complex components. [Charge conjugation](../../../../../charge-conjugation.md) reverses [chirality](../../../../../chirality-physics.md) in this signature, so a nonzero spinor cannot satisfy both conditions simultaneously.

For the [Dirac equation](../../../../../dirac-equation.md) $(\not\partial+m)\psi=0$, the derivative term reverses [chirality](../../../../../chirality-physics.md) because $\gamma_5$ anticommutes with every [gamma matrix](../../../../../gamma-matrices.md), whereas the [mass](../../../../../mass.md) term preserves it. Projecting a purely chiral spinor equation onto its two chiralities therefore gives both $\not\partial\psi=0$ and $m\psi=0$. Thus **a nonzero four-component [Weyl spinor](../../../../../weyl-spinor.md) satisfying this uncoupled [Dirac equation](../../../../../dirac-equation.md) must be massless**. A [Majorana spinor](../../../../../majorana-spinor.md) contains conjugate opposite-chirality components and can have a nonzero [mass](../../../../../mass.md). Its charge-conjugation reality condition identifies particle and antiparticle operators, so **a Majorana particle is its own antiparticle**. A Weyl field does not by itself impose that identification.

This does not forbid writing a [Majorana mass term](../../../../../majorana-mass-term.md) for a neutral two-component Weyl field: such a term couples the field to its conjugate, and the resulting four-component massive field is Majorana, not a purely chiral solution of the uncoupled [Dirac equation](../../../../../dirac-equation.md).

For the [Rarita-Schwinger field](../../../../../rarita-schwinger-field.md), set $\chi=\gamma^\mu\psi_\mu$ and $d=\partial^\mu\psi_\mu$. The antisymmetric kinetic operator is invariant under

$$
\delta\psi_\mu=\partial_\mu\eta,
$$

because commuting derivatives contract to zero against $\gamma^{\mu\nu\rho}$. Expanding its gamma product gives

$$
E^\mu=\gamma^{\mu\nu\rho}\partial_\nu\psi_\rho
=\not\partial\psi^\mu-\partial^\mu\chi+\gamma^\mu(\not\partial\chi-d).
$$

Gamma contraction gives $\gamma_\mu E^\mu=2(\not\partial\chi-d)$, so the equation implies $d=\not\partial\chi$ and $\not\partial\psi^\mu=\partial^\mu\chi$.

For a [Fourier mode](../../../../../fourier-mode.md) with [momentum](../../../../../momentum.md) $k$, if $k^2\ne0$ the latter identity gives $k^2\psi^\mu=k^\mu\not k\chi$. The mode is proportional to $k^\mu$ and hence pure gauge. Every physical nonzero-momentum mode therefore has **$k^2=0$**. For a null mode, choose an index with $k^\mu\ne0$. The same equation makes $\chi$ an element of the image of $\not k$, allowing a gauge choice with $\chi=0$. The field equations then reduce to

$$
\boxed{\gamma\cdot\psi=0,\qquad\partial\cdot\psi=0,\qquad\not\partial\psi_\mu=0.}
$$

Residual [gauge transformations](../../../../../gauge-transformation.md) obey $\not\partial\eta=0$.

Take a null [momentum](../../../../../momentum.md) in the third spatial direction. Residual gauge freedom and transversality remove the temporal and longitudinal [vector](../../../../../vector.md) components, leaving two transverse [vector](../../../../../vector.md) polarizations. Their helicities are $\pm1$, while on-shell spinor helicities are $\pm1/2$. The gamma-trace constraint removes the two combinations of total [helicity](../../../../../helicity.md) $\pm1/2$ and retains the aligned combinations of [helicity](../../../../../helicity.md) $\pm3/2$. Explicitly, in a [chiral representation](../../../../../chiral-gamma-matrix-representation.md) the transverse gamma contractions use $\sigma_1\pm i\sigma_2$, which annihilate the correspondingly aligned [spin](../../../../../spin.md) states and act nontrivially on the opposite states. Thus a Majorana [Rarita-Schwinger field](../../../../../rarita-schwinger-field.md) has **two physical massless polarizations**. The Majorana assumption is the one relevant to simple [supergravity](../../../../../supergravity.md); a complex vector-spinor has these helicities for its particle and independent antiparticle modes.

A consistent free massive deformation is the algebraic term

$$
\mathcal L_m=\frac m2\overline\psi_\mu\gamma^{\mu\nu}\psi_\nu
$$

added to a kinetic term $-\tfrac12\overline\psi_\mu\gamma^{\mu\nu\rho}\partial_\nu\psi_\rho$. Its equation is

$$
\gamma^{\mu\nu\rho}\partial_\nu\psi_\rho-m\gamma^{\mu\rho}\psi_\rho=0.
$$

For $m\ne0$, divergence and gamma contraction give, respectively,

$$
\gamma^{\mu\rho}\partial_\mu\psi_\rho=0,\qquad
2\gamma^{\nu\rho}\partial_\nu\psi_\rho-3m\gamma^\rho\psi_\rho=0.
$$

These imply the [massive Rarita-Schwinger constraints](../../../../../massive-rarita-schwinger-constraints.md) $\chi=0$ and $d=0$, and the remaining equation is $(\not\partial+m)\psi_\mu=0$. Squaring gives $(\Box-m^2)\psi_\mu=0$ in the chosen signature. The [gauge symmetry](../../../../../gauge-invariance.md) is lost. In the rest frame, transversality sets the temporal component to zero; three spatial [vector](../../../../../vector.md) components times two on-shell spinor states give six states, and gamma trace removes the two spin-one-half states. The result is **four massive spin-$3/2$ states**, with [spin](../../../../../spin.md) projections $\pm3/2,\pm1/2$. In [supergravity](../../../../../supergravity.md) the additional longitudinal states can be supplied by the [super-Higgs mechanism](../../../../../super-higgs-mechanism.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
