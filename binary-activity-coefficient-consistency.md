# Binary activity-coefficient consistency

↑ **Parent:** [Gibbs-Duhem equation](gibbs-duhem-equation.md)

For a nonideal [chemical solution](solution-chemistry.md), write its [thermodynamic activities](thermodynamic-activity.md) on a [mole fraction](mole-fraction.md) basis as $a_A=x\gamma_A$ and $a_B=(1-x)\gamma_B$. Use composition-independent pure-component reference [chemical potentials](chemical-potential-split.md) at the same [temperature](temperature-split.md) and [pressure](pressure-split.md):

$$
\mu_A=\mu_A^*+RT\ln(x\gamma_A),
\qquad
\mu_B=\mu_B^*+RT\ln[(1-x)\gamma_B].
$$

The [activity coefficients](activity-coefficient.md) describe departure from the [ideal solution](ideal-solution.md) under that reference convention.[Thermodynamics and Chemistry, §9.5.1, printed p. 259, reference states; §9.5.3, printed p. 261, equation 9.5.14](thermodynamics-and-chemistry-by-howard-devoe.md)

At fixed [temperature](temperature-split.md) and [pressure](pressure-split.md), insert these expressions into the [Gibbs-Duhem equation](gibbs-duhem-equation.md). The [ideal solution](ideal-solution.md) terms cancel because $x\,d\ln x+(1-x)\,d\ln(1-x)=dx-dx=0$. What remains is

$$
x\,d\ln\gamma_A+(1-x)\,d\ln\gamma_B=0.
$$

Thus two independent fits to measured [activity coefficients](activity-coefficient.md) can each look smooth while failing to describe one possible [Gibbs free energy](gibbs-free-energy.md). This is a necessary consistency condition; satisfying it alone does not establish experimental accuracy or [thermodynamic stability](thermodynamic-stability.md).

For an original algebraic example, suppose at one fixed [temperature](temperature-split.md) and [pressure](pressure-split.md) that $\ln\gamma_A=\alpha(1-x)^2$, with dimensionless constant $\alpha$. The constraint requires $d\ln\gamma_B/dx=2\alpha x$. With the pure-B normalization $\gamma_B(0)=1$, [integration](integral-split.md) gives

$$
\ln\gamma_B=\alpha x^2.
$$

For $\alpha=1/2$ and $x=1/4$, the [derivatives](derivative.md) of the two [logarithms](logarithm.md) are $-3/4$ and $1/4$; their weighted sum is $-3/16+3/16=0$. Choosing $\ln\gamma_B=\alpha x$ instead would give a weighted sum $3/16$ at that composition, contradicting the [Gibbs-Duhem equation](gibbs-duhem-equation.md). These are invented model functions, with no claim to fit a particular [mixture](mixture-split.md).

The fixed-[temperature](temperature-split.md), fixed-[pressure](pressure-split.md) restriction matters. Along a path with changing [temperature](temperature-split.md) or [pressure](pressure-split.md), the general equation contains $S\,dT-V\,dp$, and the reference [chemical potentials](chemical-potential-split.md) and $RT$ also change. Across [phase coexistence](phase-coexistence.md), apply the relation separately within each smooth [thermodynamic phase](thermodynamic-phase.md); do not differentiate a discontinuous switch between phases as if it were a single composition curve.

## ↑ Ancestors (6)

1. [Gibbs-Duhem equation](gibbs-duhem-equation.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
