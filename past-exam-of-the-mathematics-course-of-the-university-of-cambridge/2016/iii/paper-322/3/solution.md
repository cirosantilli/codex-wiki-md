<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For constant component masses, the [center of mass](../../../../../center-of-mass.md) frame has $\mathbf r_1=(M_2/M)\mathbf r$ and $\mathbf r_2=-(M_1/M)\mathbf r$. [Newton's law of universal gravitation](../../../../../newton-s-law-of-universal-gravitation.md) gives the relative equation $\ddot{\mathbf r}=-GM\mathbf r/r^3$. Substitution in the component [angular momenta](../../../../../angular-momentum.md) yields

$$
\boxed{\mathbf J=\mu\mathbf h=\mu\mathbf r\times\dot{\mathbf r},\qquad\dot{\mathbf h}=\mathbf r\times\ddot{\mathbf r}=0.}
$$

Here $\mu=M_1M_2/M$ is the [reduced mass](../../../../../reduced-mass.md), while $\mathbf h$ is [specific angular momentum](../../../../../specific-angular-momentum.md).

The printed total-energy expression lacks a factor of $\mu$ in its kinetic term. With the stated physical separation coordinate, the dimensionally consistent total [two-body orbital energy](../../../../../two-body-orbital-energy.md) is

$$
\boxed{E=\frac\mu2|\dot{\mathbf r}|^2-\frac{GM\mu}{r}=\mu\varepsilon,\qquad\varepsilon=\frac12|\dot{\mathbf r}|^2-\frac{GM}{r}.}
$$

The second expression is [specific orbital energy](../../../../../specific-orbital-energy.md); these two conventions must not be mixed. Its conservation follows directly:

$$
\dot E=\mu\dot{\mathbf r}\cdot\left(\ddot{\mathbf r}+\frac{GM\mathbf r}{r^3}\right)=0.
$$

For the [eccentricity vector](../../../../../eccentricity-vector.md), differentiate $GM\mathbf e=\dot{\mathbf r}\times\mathbf h-GM\widehat{\mathbf r}$. Since $\mathbf h$ is constant,

$$
GM\dot{\mathbf e}=-\frac{GM}{r^3}\mathbf r\times(\mathbf r\times\dot{\mathbf r})-GM\left[\frac{\dot{\mathbf r}}r-\frac{\mathbf r(\mathbf r\cdot\dot{\mathbf r})}{r^3}\right]=0.
$$

The cancellation is the [vector triple product identity](../../../../../vector-triple-product.md). Thus **all three corrected Kepler integrals are conserved**. Dotting the eccentricity relation with $\mathbf r$ also gives the useful orbit identity

$$
\boxed{\mathbf e\cdot\mathbf r=\frac{h^2}{GM}-r.}
$$

For [ballistic streamline focusing by a moving star](../../../../../ballistic-streamline-focusing-by-a-moving-star.md), work in the star's rest frame and take the incoming gas to have velocity $v\mathbf e_x$, with downstream behind the star at $x>0$. A streamline with [impact parameter](../../../../../impact-parameter.md) $d>0$ approaches from $(-\infty,d,0)$. Its upstream [specific angular momentum](../../../../../specific-angular-momentum.md) and [eccentricity vector](../../../../../eccentricity-vector.md) are

$$
\mathbf h=-dv\mathbf e_z,\qquad\mathbf e=\mathbf e_x+\frac{dv^2}{GM}\mathbf e_y.
$$

At its downstream axis crossing, $\mathbf r=b\mathbf e_x$. The orbit identity gives $b=d^2v^2/(GM)-b$, hence **the collision distance** is

$$
\boxed{b=\frac{d^2v^2}{2GM}.}
$$

At that point, $h_z=b u_y=-dv$, while the $y$ component of $GM\mathbf e=\mathbf u\times\mathbf h-GM\widehat{\mathbf r}$ gives $dv\,u_x=dv^2$. Therefore

$$
\mathbf u=v\mathbf e_x-\frac{2GM}{dv}\mathbf e_y.
$$

A symmetric streamline with opposite impact parameter has the opposite transverse velocity. Their [shock wave](../../../../../shock-wave.md) removes the opposing transverse motion while preserving the common downstream component. Thus **the remaining velocity is $v\mathbf e_x$ in the star frame**. In the frame where the undisturbed medium is stationary, adding the star's velocity gives zero velocity immediately after this idealized collision.

After transverse [kinetic energy](../../../../../kinetic-energy.md) is dissipated, the remaining [specific orbital energy](../../../../../specific-orbital-energy.md) is $\varepsilon_{\rm after}=v^2/2-GM/b$. It is negative if $b<2GM/v^2$, or equivalently if the upstream [impact parameter](../../../../../impact-parameter.md) satisfies $d<d_{\rm cap}=2GM/v^2$. This is the [post-shock capture criterion in ballistic accretion](../../../../../post-shock-capture-criterion-in-ballistic-accretion.md); bound axial streams can return to the star. The captured incident [mass flux](../../../../../mass-flux.md) through the corresponding disk gives the ballistic [Bondi--Hoyle--Lyttleton accretion rate](../../../../../bondi-hoyle-lyttleton-accretion-rate.md):

$$
\boxed{\dot M=\pi d_{\rm cap}^2\rho v=\frac{4\pi(GM)^2\rho}{v^3}.}
$$

This is the pressureless, dissipative capture model, with the shock's transverse energy unavailable to unbind the wake.

For [wind mass transfer in a binary star](../../../../../wind-mass-transfer-in-a-binary-star.md), steady isotropic donor mass loss gives the local wind [mass density](../../../../../density.md) at the companion:

$$
\rho_w(a)=\frac{-\dot M_1}{4\pi a^2v_w}.
$$

A fast wind has $v_w\gg2\pi a/P$ and a capture scale small compared with $a$, so its relative incident speed is $v_w$ to leading order. Apply the same [Bondi--Hoyle--Lyttleton accretion rate](../../../../../bondi-hoyle-lyttleton-accretion-rate.md) with accretor mass $M_2$ to obtain

$$
\boxed{\dot M_{2,\rm acc}=(-\dot M_1)\frac{G^2M_2^2}{a^2v_w^4}.}
$$

Finally, [Kepler's third law](../../../../../kepler-s-third-law.md) eliminates the unquoted separation, $a=[G(M_1+M_2)P^2/(4\pi^2)]^{1/3}$, giving **the rate in terms of the stated [orbital period](../../../../../orbital-period.md)**:

$$
\boxed{\dot M_{2,\rm acc}=(-\dot M_1)\frac{(2\pi G/P)^{4/3}M_2^2}{(M_1+M_2)^{2/3}v_w^4}.}
$$

Equivalently, the [fast-wind accretion fraction in a circular binary](../../../../../fast-wind-accretion-fraction-in-a-circular-binary.md) is $[M_2/(M_1+M_2)]^2(v_{\rm orb}/v_w)^4$, with $v_{\rm orb}=2\pi a/P$ the relative circular orbital speed. Its smallness is consistent with using an almost undisturbed isotropic [stellar wind](../../../../../stellar-wind.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 322](../../paper-322-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
