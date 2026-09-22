<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use target signature $(-,+,\ldots,+)$ and worldsheet signature $(-,+)$. The [Polyakov action](../../../../../polyakov-action.md) has local [worldsheet diffeomorphism](../../../../../worldsheet-diffeomorphism.md) and [Weyl invariance](../../../../../weyl-transformation.md), together with global target-space Poincaré symmetry. Under a worldsheet coordinate change $\sigma\mapsto\sigma'$, the embedding coordinates are scalars and the [worldsheet metric](../../../../../worldsheet-metric.md) is a tensor:

$$
X'^\mu(\sigma')=X^\mu(\sigma),\qquad
g'_{ab}(\sigma')=\frac{\partial\sigma^c}{\partial\sigma'^a}\frac{\partial\sigma^d}{\partial\sigma'^b}g_{cd}(\sigma).
$$

A [Weyl transformation](../../../../../weyl-transformation.md) acts as $g_{ab}\mapsto e^{2\rho(\sigma)}g_{ab}$ and leaves $X$ unchanged. In two dimensions $\sqrt{-g}$ scales by $e^{2\rho}$ and $g^{ab}$ by $e^{-2\rho}$, so the action is invariant. Target translations act by $X^\mu\mapsto X^\mu+a^\mu$, and [Lorentz transformations](../../../../../lorentz-transformation.md) by $X^\mu\mapsto\Lambda^\mu{}_{\nu}X^\nu$ with $\Lambda^{\mathsf T}\eta\Lambda=\eta$; they leave $g$ unchanged. Infinitesimally the latter have $\delta X^\mu=\omega^\mu{}_{\nu}X^\nu$, where $\omega_{\mu\nu}=-\omega_{\nu\mu}$.

Locally, the two diffeomorphism functions put the metric into the form $g_{ab}=e^{2\rho}\eta_{ab}$, and [Weyl invariance](../../../../../weyl-transformation.md) removes the conformal factor. In this [conformal gauge](../../../../../conformal-gauge.md), the embedding coordinates are free [scalar fields](../../../../../scalar-field.md) and satisfy

$$
\boxed{(\partial_\tau^2-\partial_\sigma^2)X^\mu=0.}
$$

The metric equation must still be imposed after [gauge fixing](../../../../../gauge-fixing.md). Varying the ungauged metric gives the [worldsheet stress-energy tensor](../../../../../worldsheet-stress-energy-tensor.md) constraint

$$
\partial_aX\cdot\partial_bX-\tfrac12g_{ab}g^{cd}\partial_cX\cdot\partial_dX=0.
$$

With a dot and prime denoting the two coordinate derivatives, the independent [Virasoro constraints](../../../../../virasoro-constraint.md) are

$$
\boxed{\dot X^2+X'^2=0,\qquad\dot X\cdot X'=0,}
$$

equivalently $(\dot X\pm X')^2=0$. Local [conformal gauge](../../../../../conformal-gauge.md) leaves residual conformal transformations; on general worldsheet topologies it also leaves global moduli, rather than removing all metric information.

For target translations, differentiation of the Lagrangian with respect to $\partial_aX_\mu$ gives the [Noether current](../../../../../noether-current.md)

$$
j^{a\mu}=-\frac{1}{2\pi\alpha'}\sqrt{-g}\,g^{ab}\partial_bX^\mu.
$$

The embedding equation is $\partial_aj^{a\mu}=0$. In [conformal gauge](../../../../../conformal-gauge.md), $j^{\tau\mu}=\dot X^\mu/(2\pi\alpha')$, so integration over the [closed string](../../../../../closed-string.md) gives

$$
\boxed{P^\mu=\frac{1}{2\pi\alpha'}\int_0^{2\pi}\dot X^\mu\,d\sigma.}
$$

Periodic boundary conditions make its time derivative vanish. For an infinitesimal [Lorentz transformation](../../../../../lorentz-transformation.md), the antisymmetric coefficient of $\omega_{\mu\nu}$ gives the current $j^{a,\mu\nu}=X^\mu j^{a\nu}-X^\nu j^{a\mu}$. Its divergence vanishes because the remaining product of embedding derivatives is symmetric in $\mu,\nu$. Thus the [Noether charge](../../../../../noether-charge.md) is

$$
\boxed{J^{\mu\nu}=\frac{1}{2\pi\alpha'}\int_0^{2\pi}(X^\mu\dot X^\nu-X^\nu\dot X^\mu)\,d\sigma.}
$$

These are the [target-space Noether charges of a string](../../../../../target-space-noether-charges-of-a-string.md).

For the circular solution take $R>0$, and let $\boldsymbol e_r=(\cos\sigma,\sin\sigma)$ and $\boldsymbol e_\sigma=(-\sin\sigma,\cos\sigma)$. Its derivatives are

$$
\dot X=(R,-R\sin\tau\,\boldsymbol e_r),\qquad
X'=(0,R\cos\tau\,\boldsymbol e_\sigma).
$$

Each spatial coordinate has equal second derivatives in $\tau$ and $\sigma$, while the time coordinate has both second derivatives zero. Furthermore

$$
\dot X^2=-R^2\cos^2\tau,\qquad X'^2=R^2\cos^2\tau,\qquad\dot X\cdot X'=0,
$$

so both the field equations and the [Virasoro constraints](../../../../../virasoro-constraint.md) hold, including the collapse instants.

At target time $t=X^0=R\tau$, the string is a circle in the $X^1X^2$ plane of radius $R|\cos(t/R)|$. It contracts from radius $R$ to zero and re-expands; the negative cosine reverses material labels by a half-turn rather than creating a negative radius. The spatial configuration repeats after target time $\pi R$. This is a [pulsating circular string](../../../../../pulsating-circular-string.md). Its induced metric degenerates at collapse, but the conformal-gauge embedding and constraints give its continuation.

The integrals of $\sin\sigma$ and $\cos\sigma$ vanish, so the momentum is

$$
\boxed{P^\mu=(R/\alpha',0,0,\ldots),\qquad M=R/\alpha'.}
$$

The spatial velocity is radial, giving zero angular momentum density in the plane; all boost-charge terms integrate to zero as well. Hence **$J^{\mu\nu}=0$ for every pair of indices**.

At maximum expansion, all string elements are instantaneously at rest, and the length is $L_0=2\pi R$. Thus the rest mass per unit length, equal to the [string tension](../../../../../string-tension.md), is

$$
\boxed{\frac{M}{L_0}=\frac{1}{2\pi\alpha'}.}
$$

At other times the instantaneous circumference is $L=2\pi R|\cos\tau|$, and the elements have speed $|\sin\tau|$. Their Lorentz factor is $1/|\cos\tau|$, so the energy remains $TL/\sqrt{1-v^2}=2\pi TR$. The rest-energy density is $T$; the total rest-frame energy divided by the changing circumference is not constant. This distinguishes the requested intrinsic mass density from the larger energy density of moving string elements.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
