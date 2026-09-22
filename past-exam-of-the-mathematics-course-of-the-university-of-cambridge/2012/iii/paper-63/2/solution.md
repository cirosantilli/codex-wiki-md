<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $u=\cos\theta$, $S=j/\kappa$ and use axial symmetry. The [radiative flux](../../../../../radiative-flux.md) is $F=2\pi\int_{-1}^1uI\,du$. Integrating the [radiative transfer equation](../../../../../radiative-transfer-equation.md) over directions gives

$$
\frac{dF}{d\tau}=4\pi(J-S).
$$

There are no energy sources in the atmosphere, so [radiative equilibrium](../../../../../radiative-equilibrium.md) makes $F$ constant. Consequently

$$
\boxed{J=S=\frac{j}{\kappa}=\frac{\sigma T^4}{\pi}.}
$$

For the linear angular approximation $I=A+Cu$, the [radiation-field moments](../../../../../radiation-field-moment.md) are

$$
J=A,\qquad F=\frac{4\pi}{3}C,\qquad
cP_r=2\pi\int_{-1}^1u^2(A+Cu)\,du=\frac{4\pi}{3}A.
$$

Thus it satisfies the [Eddington closure approximation](../../../../../eddington-closure-approximation.md), and

$$
\boxed{cP_r=\frac{4\pi}{3}J,\qquad C=\frac{3F}{4\pi}.}
$$

Since $F$ is constant, $C'=0$. Substitution in the [radiative transfer equation](../../../../../radiative-transfer-equation.md), using $S=A$, gives $uA'=Cu$, hence $\boxed{A'=C}$.

In this moment approximation, the inward hemispheric flux at the surface is

$$
F_{\rm in}=-2\pi\int_{-1}^0u(A_0+Cu)\,du
=\pi A_0-\frac{2\pi}{3}C.
$$

Setting this boundary moment to zero gives $A_0=2C/3$. Therefore

$$
A(\tau)=\frac{3F}{4\pi}\left(\tau+\frac23\right).
$$

Combining it with the thermal [source function](../../../../../radiative-transfer-source-function.md) and $F=\sigma T_e^4$ gives the [grey atmosphere](../../../../../grey-atmosphere.md) temperature law:

$$
\boxed{T^4=\frac34T_e^4\left(\tau+\frac23\right),\qquad
T_0=2^{-1/4}T_e.}
$$

**The surface condition is an approximate angular-moment condition.** If the affine intensity were interpreted as an exact nonnegative boundary radiation field, no incident radiation would require $I(0,u)=0$ for every $u<0$; a linear polynomial vanishing on that interval would have $A_0=C=0$ and no outward flux either. The derived formal profile indeed has $I(0,-1)=-F/(4\pi)<0$. This [positivity limitation of a linear Eddington intensity](../../../../../positivity-limitation-of-a-linear-eddington-intensity.md) is why one uses the [Eddington surface boundary condition](../../../../../eddington-surface-boundary-condition.md) as a moment closure, not the affine ansatz as an exact emergent angular intensity. An outward direction-independent intensity with no inward intensity gives the same boundary moments.

For the gas-pressure-dominated atmosphere, combine $dP/dz=-\rho g$ with $d\tau/dz=-\kappa\rho$. Thus the [hydrostatic equilibrium in optical depth](../../../../../hydrostatic-equilibrium-in-optical-depth.md) is $dP/d\tau=g/\kappa$. Let $w=T^4$. The [grey atmosphere](../../../../../grey-atmosphere.md) law implies $dw/d\tau=3T_0^4/2$. With the specified power-law [opacity](../../../../../opacity.md),

$$
\frac{d(P^\alpha)}{dw}
=\frac{2\alpha g}{3\kappa_0T_0^4}\,w^{\beta-1}.
$$

At the outer vacuum limit take $P=0$ and $T=T_0$. Since $\alpha,\beta>0$, integration gives

$$
\boxed{P^\alpha=\frac{2\alpha g}{3\beta\kappa_0T_0^4}
\left(T^{4\beta}-T_0^{4\beta}\right).}
$$

This is the [grey-atmosphere pressure with power-law opacity](../../../../../grey-atmosphere-pressure-with-power-law-opacity.md) relation.

At the matching radius the local [radiative flux](../../../../../radiative-flux.md) is $L_r/(4\pi r^2)=\sigma T^4$. In the thin [plane-parallel atmosphere](../../../../../plane-parallel-atmosphere.md) approximation this equals $F=\sigma T_e^4$, so $T=T_e$ and $T^4=2T_0^4$. Multiplying the pressure relation by $\kappa_0T^{4-4\beta}/g$ yields the required **surface pressure-opacity relation**

$$
\boxed{\frac{P\kappa}{g}
=\frac{2\alpha}{3\beta}\frac{T^4}{T_0^4}
\left[1-\left(\frac{T_0}{T}\right)^{4\beta}\right]
=\frac{4\alpha}{3\beta}(1-2^{-\beta}).}
$$

Here $P\kappa$ is a product, not a pressure subscript.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
