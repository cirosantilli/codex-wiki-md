<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

At the [stellar surface boundary condition](../../../../../stellar-surface-boundary-condition.md), match the interior to a [stellar atmosphere](../../../../../stellar-atmosphere.md), rather than setting the [temperature](../../../../../temperature.md) and [pressure](../../../../../pressure.md) to zero at an arbitrary radius. At a [photosphere](../../../../../photosphere.md) of radius $R$, the [enclosed mass](../../../../../enclosed-mass.md) is $M$, the [luminosity](../../../../../luminosity.md) is $L$, and the outward [radiative flux](../../../../../radiative-flux.md) defines the [effective temperature](../../../../../effective-temperature.md) through $F=L/(4\pi R^2)=\sigma_{\rm SB}T_{\rm eff}^4$. With no external illumination the incoming [specific intensity](../../../../../specific-intensity.md) satisfies $I_\nu(0,\mu)=0$ for $\mu<0$. A deeper boundary is matched to the nearly isotropic [radiative diffusion](../../../../../radiative-diffusion.md) field. A [grey atmosphere](../../../../../grey-atmosphere.md) commonly matches near $\tau=2/3$; under the [Eddington surface boundary condition](../../../../../eddington-surface-boundary-condition.md) this gives $T=T_{\rm eff}$. For roughly constant gravity and [opacity](../../../../../opacity.md), the total [pressure](../../../../../pressure.md) rises by $g\tau/\kappa$ relative to its outer boundary value; if radiation supplies appreciable support, the gas-pressure gradient uses the effective gravity $g-\kappa F/c$ instead.

Take $z$ increasing outward and $\mu$ the outward direction cosine. If $j_\nu$ is emission per unit path length and solid angle, the [radiative transfer equation](../../../../../radiative-transfer-equation.md) is

$$
\mu\frac{\partial I_\nu}{\partial z}=j_\nu-\rho\kappa_\nu I_\nu.
$$

Define inward-increasing [optical depth](../../../../../optical-depth.md) by $d\tau_\nu=-\rho\kappa_\nu dz$ and the [source function](../../../../../radiative-transfer-source-function.md) by $S_\nu=j_\nu/(\rho\kappa_\nu)$. Then $\mu\partial_{\tau_\nu}I_\nu=I_\nu-S_\nu$. This states the emission-coefficient convention; if $j_\nu$ is defined per unit mass instead, the emission term is $\rho j_\nu$.

For frequency-integrated intensity, introduce the [radiation-field moments](../../../../../radiation-field-moment.md)

$$
J=\frac12\int_{-1}^1I\,d\mu,\qquad H=\frac12\int_{-1}^1\mu I\,d\mu,\qquad K=\frac12\int_{-1}^1\mu^2I\,d\mu,\qquad F=4\pi H,\qquad cP_{\rm rad}=4\pi K.
$$

The first angular approximation writes $I\simeq J+3\mu H$. Its odd part does not contribute to $K$, so

$$
\boxed{K=\frac J3,\qquad cP_{\rm rad}=\frac{4\pi}3J.}
$$

This is the [Eddington closure approximation](../../../../../eddington-closure-approximation.md), not an exact description of the escaping angular distribution. An approximate surface condition takes the outgoing hemisphere to have direction-independent intensity $I_0$ and the incoming hemisphere to be dark. Its moments give $F=\pi I_0$ and $J(0)=I_0/2=F/(2\pi)$. Integrating the moment equations with the closure then gives $J=3F(\tau+2/3)/(4\pi)$; in thermal equilibrium, $J=a_{\rm rad}cT^4/(4\pi)$ gives $T^4=(3/4)T_{\rm eff}^4(\tau+2/3)$. This derives the usual approximate photospheric matching condition rather than imposing a zero surface [temperature](../../../../../temperature.md). For conservative [coherent isotropic scattering](../../../../../coherent-isotropic-scattering.md), $S=J$. Integrating the transfer equation gives $dH/d\tau=0$ and $dK/d\tau=H$, the moment conditions for [radiative equilibrium](../../../../../radiative-equilibrium.md).

The exponential ansatz in the PDF has a genuine consistency problem. Compute its moments before making any approximation. For a nonsingular real intensity on all $-1\le\mu\le1$, take $|\epsilon|<1$ and define

$$
A_0=\frac12\int_{-1}^1\frac{d\mu}{1+\epsilon\mu}=\frac{\operatorname{atanh}\epsilon}{\epsilon},\qquad A_1=\frac{1-A_0}{\epsilon},\qquad A_2=\frac{A_0-1}{\epsilon^2}.
$$

The continuous zero limits are $A_0=1$, $A_1=0$, $A_2=1/3$. Direct integration yields

$$
\boxed{J=\alpha(\beta+\tau+\gamma A_0e^{-\delta\tau}),\qquad F(\tau)=4\pi\alpha\left(\frac13+\gamma A_1e^{-\delta\tau}\right),}
$$



$$
\boxed{cP_{\rm rad}=4\pi\alpha\left(\frac{\beta+\tau}{3}+\gamma A_2e^{-\delta\tau}\right).}
$$

For a decaying nontrivial correction, $\delta>0$ and $\gamma\ne0$. Exact constant flux then requires $A_1=0$. But $\operatorname{atanh}\epsilon/\epsilon>1$ for every nonzero real $|\epsilon|<1$, so $A_1=0$ forces $\epsilon=0$. Thus exact [radiative equilibrium](../../../../../radiative-equilibrium.md) cannot imply a small nonzero $\epsilon$ for this ansatz.

Substitution into the full transfer equation makes the obstruction sharper. The exponential coefficient must satisfy, for every $\mu$,

$$
-\delta\mu=1-A_0(1+\epsilon\mu).
$$

Comparing the constant and linear coefficients gives $A_0=1$ and $\delta=A_0\epsilon=\epsilon$. Hence regular real coefficients require $\delta=\epsilon=0$, eliminating any decaying correction. This is the [obstruction to a single smooth exponential mode in conservative grey transfer](../../../../../obstruction-to-a-single-smooth-exponential-mode-in-conservative-grey-transfer.md). **There is no exact nontrivial real solution of the stipulated form with a small nonzero decay parameter.** Choosing, for example, $\epsilon=\delta=0.1$ and $\gamma\ne0$ supplies an explicit counterexample to the claimed exact flux constancy, because $A_1\ne0$.

Several requested conclusions remain useful as formal approximations, provided they are identified as such. If $\delta>0$, the large-depth exponential vanishes, giving $F\to4\pi\alpha/3$, hence $\alpha=3F/(4\pi)$ for the asymptotic physical flux. It also gives $cP_{\rm rad}\to(4\pi/3)J$. Since $A_0=1+\epsilon^2/3+O(\epsilon^4)$, neglecting second-order angular errors yields the formal relation $\delta\simeq\epsilon$. However $A_1=-\epsilon/3+O(\epsilon^3)$, so the finite-depth flux still varies at first order. The formal relation is not an exact transfer or constant-flux solution.

There is also a flux-normalization mismatch in the PDF's last displayed relation. With the same physical $F$ used above, the [Hopf function of a grey atmosphere](../../../../../hopf-function-of-a-grey-atmosphere.md) is defined by

$$
J=\frac{3F}{4\pi}[\tau+q(\tau)].
$$

The PDF's coefficient $3F/4$ would require redefining its $F$ as physical flux divided by $\pi$; it cannot simultaneously use the earlier $\alpha=3F/(4\pi)$ for the same physical flux. With the consistent physical-flux normalization, formal moment matching gives

$$
\beta=q(\infty)=0.71,\qquad\gamma A_0=q(0)-q(\infty)=-0.14.
$$

In the intended small-$\epsilon$ approximation this is

$$
\boxed{\beta\simeq0.71,\qquad\gamma\simeq-0.14.}
$$

The approximate outgoing surface ansatz then gives the [limb darkening](../../../../../limb-darkening.md) ratio

$$
\frac{I(1,0)}{I(0,0)}=\frac{\beta+1+\gamma/(1+\epsilon)}{\beta+\gamma}\ \longrightarrow\ \boxed{\frac{1.57}{0.57}\simeq2.75.}
$$

For finite $\epsilon$, $\gamma=-0.14/A_0$ gives a parameter-dependent ratio, not a unique exact value. The two Hopf endpoint values alone do not determine the exact emergent intensity: the [formal solution of the radiative transfer equation](../../../../../formal-solution-of-the-radiative-transfer-equation.md) uses the entire source profile, $I(0,\mu)=\int_0^\infty J(t)e^{-t/\mu}dt/\mu$ for $\mu>0$. Nor does the simple linear-plus-exponential ansatz satisfy the exact no-incoming-radiation condition for every negative $\mu$. Thus $2.75$ is a clearly labelled approximate disk-centre-to-limb result, not an exact consequence of inconsistent premises.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
