<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $u=\cos\theta$ for the direction cosine and $B=j/\kappa=\sigma T^4/\pi$ for the [radiative transfer source function](../../../../../radiative-transfer-source-function.md). Integrating the [radiative transfer equation](../../../../../radiative-transfer-equation.md) $u\,\partial_\tau I=I-B$ over [solid angle](../../../../../solid-angle.md) gives

$$
\frac{dF}{d\tau}=\int(I-B)\,d\Omega=4\pi(J-B).
$$

[Radiative equilibrium](../../../../../radiative-equilibrium.md) makes the [radiative flux](../../../../../radiative-flux.md) $F$ constant, so **$J=B=j/\kappa$**.

For $I=A+Cu$, the [radiation-field moments](../../../../../radiation-field-moment.md) are

$$
J=\frac12\int_{-1}^1I\,du=A,\qquad F=2\pi\int_{-1}^1uI\,du=\frac{4\pi C}{3},\qquad cP_r=2\pi\int_{-1}^1u^2I\,du=\frac{4\pi A}{3}.
$$

Consequently the [Eddington closure approximation](../../../../../eddington-closure-approximation.md) holds. Substituting into the [radiative transfer equation](../../../../../radiative-transfer-equation.md), with $B=J=A$, gives $uA'+u^2C'=Cu$. Equality for every $u$ requires $A'=C$ and $C'=0$, with $C=3F/(4\pi)$. The stipulated inward hemispheric [radiative flux](../../../../../radiative-flux.md) at the surface is

$$
F_{\rm in}=2\pi\int_{-1}^0u(A_0+Cu)\,du=-\pi A_0+\frac{2\pi C}{3}.
$$

Putting this equal to zero fixes $A_0=2C/3$, hence $A=C(\tau+2/3)$. Using $A=\sigma T^4/\pi$ and the [effective temperature](../../../../../effective-temperature.md) definition $F=\sigma T_e^4$ gives the [grey atmosphere](../../../../../grey-atmosphere.md) law

$$
\boxed{T^4=\frac34T_e^4\left(\tau+\frac23\right)},\qquad \boxed{T_0=2^{-1/4}T_e}.
$$

The [positivity limitation of a linear Eddington intensity](../../../../../positivity-limitation-of-a-linear-eddington-intensity.md) matters here: the formal surface intensity $I(0,u)=C(2/3+u)$ is negative for $u<-2/3$. Thus this angular ansatz gives the requested [Eddington surface boundary condition](../../../../../eddington-surface-boundary-condition.md) for approximate moments; vanishing integrated inward flux is not an exact, nonnegative, pointwise no-incoming radiation field.

Neglecting [radiation pressure](../../../../../radiation-pressure.md), the [stellar hydrostatic equation](../../../../../hydrostatic-pressure-support-equation.md) and the definition of [optical depth](../../../../../optical-depth.md) give [hydrostatic equilibrium in optical depth](../../../../../hydrostatic-equilibrium-in-optical-depth.md), $dP/d\tau=g/\kappa$. Since $T^4=T_0^4(1+3\tau/2)$, putting $v=T^4$ gives

$$
\frac{d(P^\alpha)}{dv}=\frac{2\alpha g}{3\kappa_0T_0^4}v^{\beta-1}.
$$

Taking $P(0)=0$ and $\alpha>0$, the [grey-atmosphere pressure with power-law opacity](../../../../../grey-atmosphere-pressure-with-power-law-opacity.md) is therefore

$$
\boxed{P^\alpha=\frac{2\alpha g}{3\beta\kappa_0T_0^4}\left(T^{4\beta}-T_0^{4\beta}\right)}\qquad(\beta\ne0).
$$

**The pressure formula printed in the PDF is missing the factor $1/\beta$.** Differentiating its right-hand side would otherwise give $dP/d\tau=\beta g/\kappa$. For $\beta=0$ the correct [limit](../../../../../limit-of-a-function.md) is $P^\alpha=2\alpha g\log(T^4/T_0^4)/(3\kappa_0T_0^4)$.

At the specified matching location, the [luminosity](../../../../../luminosity.md) relation makes $F=L_r/(4\pi r^2)=\sigma T^4$, hence $T=T_e$, $T^4=2T_0^4$ and $\tau=2/3$. Multiplying the corrected pressure relation by $\kappa_0T^{4-4\beta}/g$ gives

$$
\boxed{\frac{P\kappa}{g}=\frac{4\alpha}{3\beta}\left(1-2^{-\beta}\right)}.
$$

This agrees with the PDF's final [surface boundary condition for a power-law-opacity grey atmosphere](../../../../../surface-boundary-condition-for-a-power-law-opacity-grey-atmosphere.md). It also extends to negative $\beta$ wherever the model applies; at $\beta=0$, its continuous [limit](../../../../../limit-of-a-function.md) is $P\kappa/g=4\alpha\log2/3$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
