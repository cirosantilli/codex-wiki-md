<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For adjoint-valued quantities write $(X\times Y)_a=\varepsilon_{abc}X_bY_c$. Substituting the infinitesimal transformation into the [gauge field strength](../../../../../gauge-field-strength.md) and using the [Jacobi identity](../../../../../jacobi-identity.md) gives

$$
\boxed{\delta F_{\mu\nu a}=g\varepsilon_{abc}F_{\mu\nu b}\lambda_c.}
$$

A useful way to organize the calculation is $[D_\mu,D_\nu]X=gF_{\mu\nu}\times X$: the [gauge field strength](../../../../../gauge-field-strength.md) transforms covariantly because the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) does. Thus $\delta(F_a^{\mu\nu}F_{\mu\nu a})=2gF_a^{\mu\nu}\varepsilon_{abc}F_{\mu\nu b}\lambda_c=0$ by antisymmetry. This proves **[gauge invariance](../../../../../gauge-invariance.md) of the [Yang-Mills action](../../../../../yang-mills-action.md)**.

The [Yang-Mills equations](../../../../../yang-mills-equations.md) are $D_\mu F^{\mu\nu}=0$. They determine physical evolution only modulo [gauge redundancy](../../../../../gauge-redundancy.md): gauge transformations with arbitrary spacetime-dependent parameters take solutions to equivalent solutions. In [Hamiltonian mechanics](../../../../../hamiltonian-mechanics.md), $A_0$ has no independent quadratic time-derivative term, and the corresponding equation is a [Gauss law constraint in gauge theory](../../../../../gauss-law-constraint-in-gauge-theory.md). A gauge parameter can vanish with its necessary derivatives on the initial slice yet change the later [potential energy](../../../../../potential-energy.md), so the [potential energy](../../../../../potential-energy.md) itself is not uniquely fixed by initial physical data.

In the uncorrected [path integral](../../../../../path-integral.md), integration along [gauge orbits](../../../../../gauge-orbit.md) overcounts equivalent fields. At the perturbative level the quadratic operator of the [kinetic term](../../../../../kinetic-term.md) has gauge zero modes and no inverse, so it does not supply a [quantum field theory propagator](../../../../../propagator.md). [Gauge fixing](../../../../../gauge-fixing.md) together with the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) removes this obstruction in the local perturbative construction.

For the odd [BRST transformation](../../../../../brst-symmetry.md), products obey the [graded Leibniz rule](../../../../../graded-leibniz-rule.md). The adjoint product with [Grassmann variables](../../../../../grassmann-variable.md) satisfies

$$
X\times Y=-(-1)^{|X||Y|}Y\times X.
$$

In particular, $c\times c$ is not zero, and $c\times Dc=Dc\times c$. The supplied transformations give

$$
s^2A_\mu=D_\mu(sc)+g(sA_\mu)\times c
=-\frac g2D_\mu(c\times c)+g(D_\mu c)\times c=0,
$$

since the even covariant derivative obeys $D(c\times c)=2(Dc)\times c$. For the ghost,

$$
s^2c=-\frac g2\bigl((sc)\times c-c\times(sc)\bigr)
=-g(sc)\times c=\frac{g^2}{2}(c\times c)\times c=0.
$$

The final equality is the [graded Jacobi identity](../../../../../graded-jacobi-identity.md); in components it is the [Jacobi identity](../../../../../jacobi-identity.md) for $\varepsilon_{abc}$ contracted with the totally antisymmetric product of three ghosts. Also $s^2\bar c=-sb=0$ and $s^2b=0$. The square of an odd derivation is an even derivation, because its two mixed product terms cancel. Hence **$s^2=0$ on every polynomial in the fields**, off shell, without imposing field equations.

Let $\Psi=\int d^dx\,[\partial^\mu\bar c_aA_{\mu a}+\xi\bar c_ab_a/2]$ be the [gauge-fixing fermion](../../../../../gauge-fixing-fermion.md). Since $sF=gF\times c$, $s\mathcal L_{\mathrm{YM}}=0$. The [BRST-exact operator](../../../../../brst-exact-operator.md) in $\mathcal L_q=\mathcal L_{\mathrm{YM}}-s\psi$ has zero variation by [BRST nilpotence](../../../../../brst-nilpotence.md), so

$$
\boxed{s\mathcal L_q=0.}
$$

To see the resulting kinetic terms and signs, expand the exact term with $s\bar c=-b$:

$$
-s\psi=(\partial^\mu b_a)A_{\mu a}
+(\partial^\mu\bar c_a)(D_\mu c)_a+\frac\xi2 b_a^2.
$$

After [integration by parts](../../../../../integration-by-parts.md),

$$
\mathcal L_q=\mathcal L_{\mathrm{YM}}-b_a\partial^\mu A_{\mu a}
+\frac\xi2b_a^2-\bar c_a\partial^\mu(D_\mu c)_a.
$$

The auxiliary [Nakanishi-Lautrup field](../../../../../nakanishi-lautrup-field.md) $b$ can be completed into a square and integrated out, giving the gauge-fixing term $-(\partial\cdot A_a)^2/(2\xi)$ for $\xi\ne0$. At $\xi=0$, retain $b$ as the multiplier enforcing the gauge condition rather than divide by $\xi$. The [Grassmann Gaussian integral](../../../../../grassmann-gaussian-integral.md) gives the [determinant](../../../../../determinant.md) of the gauge-condition operator $-\partial\cdot D$. Field-independent normalizations cancel in the normalized integral; insertions involving $b$ can be handled before integration or through its source terms.

At $g=0$ the gauge-fixed quadratic operator is invertible with the usual prescription, and the ghosts have a quadratic [kinetic term](../../../../../kinetic-term.md). The remaining terms are cubic gauge interactions of order $g$, quartic gauge interactions of order $g^2$, and a ghost-gauge interaction of order $g$. Expanding them and using [Wick contractions](../../../../../wick-contraction.md) gives a perturbative expansion for any defined polynomial insertion $X$ of the fields. The exponent is the gauge-fixed [action](../../../../../action.md) $S_q$, as printed in the PDF; the converted TeX incorrectly substitutes $S_A$.

At $\xi=1$, the free gauge [action](../../../../../action.md), up to a boundary term, is $\tfrac12\int A_{\mu a}\Box A_a^\mu$. Its Fourier kernel is $-p^2\eta_{\mu\nu}\delta_{ab}$. With the mostly-plus convention used above, the [Feynman-gauge adjoint propagator](../../../../../feynman-gauge-adjoint-propagator.md) is

$$
\boxed{\langle T A_{\mu a}(x)A_{\nu b}(y)\rangle_0
=\int\frac{d^dp}{(2\pi)^d}\,e^{ip\cdot(x-y)}
\frac{-i\eta_{\mu\nu}\delta_{ab}}{p^2-i\epsilon}.}
$$

This is consistent with the scalar-line convention in Question 2.

Finally define the odd functional $B=\tfrac12\int d^dx\,\bar c_ab_a$. Then $\partial_\xi S_q=-sB$. Differentiating the normalized expectation, including its denominator, gives

$$
\partial_\xi\langle X\rangle
=-i\left[\langle XsB\rangle-\langle X\rangle\langle sB\rangle\right]
$$

for an insertion with no explicit $\xi$ dependence. A physical gauge-invariant insertion $X[A]$ is [BRST-closed](../../../../../brst-closed-operator.md), since its infinitesimal gauge variation vanishes also when the parameter is replaced by $c$. The assumed [BRST Ward identity](../../../../../brst-ward-identity.md) gives $\langle sB\rangle=0$ and $\langle s(XB)\rangle=0$. For an even $X$ with $sX=0$, the latter says $\langle XsB\rangle=0$. Therefore

$$
\boxed{\partial_\xi\langle X\rangle=0.}
$$

The same conclusion holds for any [BRST-closed](../../../../../brst-closed-operator.md) insertion. Mere color-singlet invariance of an arbitrary ghost-dependent expression need not imply $sX=0$; the physical-observable qualification is essential. The proof uses the invariant-measure assumptions encoded in the stated Ward identity.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
