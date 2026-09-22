# Gibbs-Duhem equation

↑ **Parent:** [Thermodynamics](thermodynamics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gibbs–Duhem_equation)

The [Euler theorem for homogeneous functions](euler-theorem-for-homogeneous-functions.md) applied to an [extensive quantity](extensive-quantity.md), together with $dE=T\,dS-p\,dV+\mu\,dN$ give

$$
E=TS-pV+\mu N,
\qquad
S\,dT-V\,dp+N\,d\mu=0.
$$

The [Gibbs-Duhem equation](gibbs-duhem-equation.md) constrains changes of the [intensive quantities](intensive-quantity.md) describing one uniform [thermodynamic phase](thermodynamic-phase.md). For a [mixture](mixture-split.md) with $k$ independently specified component amounts, its molar form is

$$
S\,dT-V\,dp+\sum_{i=1}^k n_i\,d\mu_i=0.
$$

Here $S$ is [entropy](entropy-split.md), $V$ is [volume](volume-thermodynamics.md), $T$ is [temperature](temperature-split.md), $p$ is [pressure](pressure-split.md), $n_i$ is the [amount of substance](amount-of-substance.md) of component $i$, and $\mu_i$ is its molar [chemical potential](chemical-potential-split.md). This assumes a [simple compressible system](simple-compressible-system.md) whose bulk [internal energy](internal-energy-split.md) is an [extensive quantity](extensive-quantity.md); additional [work](work.md) coordinates require additional terms.[Howard DeVoe, Thermodynamics and Chemistry, second edition, version 10, §9.2.8, printed p. 240, equations 9.2.42–9.2.44](thermodynamics-and-chemistry-by-howard-devoe.md)

The proof exposes the source of the constraint. For [internal energy](internal-energy-split.md) $E(S,V,n_1,\ldots,n_k)$, replication of the whole [thermodynamic phase](thermodynamic-phase.md) by a factor $\lambda$ gives $E(\lambda S,\lambda V,\lambda n_1,\ldots,\lambda n_k)=\lambda E(S,V,n_1,\ldots,n_k)$. The [Euler theorem for homogeneous functions](euler-theorem-for-homogeneous-functions.md) and the fundamental [differential](differential-of-a-smooth-map.md) of [internal energy](internal-energy-split.md) therefore give

$$
E=TS-pV+\sum_i\mu_i n_i,
\qquad
dE=T\,dS-p\,dV+\sum_i\mu_i\,dn_i.
$$

Taking the [differential](differential-of-a-smooth-map.md) of the first equation produces all the terms in the second, plus $S\,dT-V\,dp+\sum_i n_i\,d\mu_i$. Subtraction proves the [Gibbs-Duhem equation](gibbs-duhem-equation.md). Thus the constraint comes from two descriptions of the same [state function](state-function.md), rather than an assumed microscopic interaction model.

At fixed [temperature](temperature-split.md) and [pressure](pressure-split.md), divide by $n=\sum_i n_i>0$ and introduce the [mole fractions](mole-fraction.md) $x_i=n_i/n$:

$$
\sum_i x_i\,d\mu_i=0.
$$

The [chemical potentials](chemical-potential-split.md) cannot be varied independently. In a two-component [mixture](mixture-split.md), put $x_A=x$ and $x_B=1-x$. Within a smooth single-[thermodynamic phase](thermodynamic-phase.md) region with $0<x<1$,

$$
x\left(\frac{\partial\mu_A}{\partial x}\right)_{T,p}
+(1-x)\left(\frac{\partial\mu_B}{\partial x}\right)_{T,p}=0,
\qquad
d\mu_B=-\frac{x}{1-x}\,d\mu_A.
$$

One [chemical potential](chemical-potential-split.md) fixes the other's change, but determining its absolute value still requires a reference value. This does not say $\mu_A=\mu_B$: equality at [phase coexistence](phase-coexistence.md) concerns the same [chemical species](chemical-species.md) in different [thermodynamic phases](thermodynamic-phase.md). Nor does the constraint say $dG=0$ whenever [temperature](temperature-split.md) and [pressure](pressure-split.md) are fixed; changing composition still contributes $\sum_i\mu_i\,dn_i$ to the [Gibbs free energy](gibbs-free-energy.md).

**Table of contents**

- [Ideal binary Gibbs-Duhem cancellation](ideal-binary-gibbs-duhem-cancellation.md)
- [Binary activity-coefficient consistency](binary-activity-coefficient-consistency.md)
- [Mixture measurements and the Gibbs-Duhem constraint](mixture-measurements-and-the-gibbs-duhem-constraint.md)

## ↑ Ancestors (5)

1. [Thermodynamics](thermodynamics-split.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Binary activity-coefficient consistency](binary-activity-coefficient-consistency.md)
- [Euler relation in thermodynamics](euler-relation-in-thermodynamics.md)
- [Euler theorem for homogeneous functions](euler-theorem-for-homogeneous-functions.md)
- [Gibbs-Duhem equation](gibbs-duhem-equation.md)
- [Isothermal compressibility from chemical-potential response](isothermal-compressibility-from-chemical-potential-response.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-310/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2/37b/c/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2015/paper-1/1/b/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019/section-a/1/solution.md)
