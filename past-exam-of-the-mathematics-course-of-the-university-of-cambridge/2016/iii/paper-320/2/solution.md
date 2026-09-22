<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A spherically symmetric stellar model has no preferred direction in the tangent plane at a fixed radius. Rotations about the radial axis exchange its two transverse [velocity](../../../../../velocity.md) directions, so $\langle v_\theta^2\rangle=\langle v_\phi^2\rangle$. This uses [spherical symmetry](../../../../../spherical-symmetry.md) of the [velocity](../../../../../velocity.md) distribution, not just a spherical [mass density](../../../../../density.md).

The [augmented density](../../../../../augmented-stellar-density.md) $\rho(r,\psi)$ treats radius and [relative potential](../../../../../relative-potential.md) as independent variables, agreeing with the physical density only along $\psi=\psi(r)$. For any regular bound spherical [galactic distribution function](../../../../../galactic-distribution-function.md) $F(E,L)$, write $P_r=\int v_r^2F\,d^3v$ and $P_t=\int v_\theta^2F\,d^3v$. At fixed $r$, $F_\psi=F_E$ and $\partial_{v_r}F=-v_rF_E$. [Integration by parts](../../../../../integration-by-parts.md) therefore gives

$$
\partial_\psi P_r=\int v_r^2F_E\,d^3v=-\int v_r\partial_{v_r}F\,d^3v=\rho.
$$

For $v_t^2=v_\theta^2+v_\phi^2$, the [velocity](../../../../../velocity.md) measure is $2\pi v_t\,dv_t\,dv_r$, and $rF_L=\partial_{v_t}F+v_tF_E$. Integrating the transverse derivative gives $-2P_r$, while integrating the radial derivative in $\int v_r^2v_t^2F_E\,d^3v$ gives $2P_t$. Consequently

$$
\partial_rP_r=\frac{2}{r}(P_t-P_r),\qquad\partial_r(r^2P_r)=2rP_t,
$$

where $\psi$ is fixed. These identities show that the augmented representation holds for any such spherical distribution, not only a monomial ansatz. With radial pressure vanishing at the zero-binding boundary, set

$$
A(r,\psi)=P_r(r,\psi)=\int_0^\psi\rho(r,q)\,dq.
$$

 Along the physical curve, the chain rule gives $dA/dr=\int_0^\psi\partial_r\rho(r,q)\,dq+\rho(r,\psi)\psi'(r)$. The [Spherical Jeans equation](../../../../../spherical-jeans-equation.md) then requires

$$
B\equiv\rho\langle v_\theta^2\rangle=A+\frac r2\int_0^\psi\partial_r\rho(r,q)\,dq=\frac{1}{2r}\int_0^\psi\partial_r[r^2\rho(r,q)]\,dq.
$$

Thus the [Jeans moments from an augmented density](../../../../../jeans-moments-from-an-augmented-density.md) are

$$
\boxed{\rho\langle v_r^2\rangle=\int_0^\psi\rho(r,q)\,dq,\qquad\rho\langle v_\theta^2\rangle=\frac1{2r}\int_0^\psi\partial_r[r^2\rho(r,q)]\,dq.}
$$

The partial derivative holds $q$ fixed. Substitution cancels the integral of $\partial_r\rho$ and leaves precisely $\rho\psi'$ in the [Spherical Jeans equation](../../../../../spherical-jeans-equation.md). This is a representation by a chosen [augmented density](../../../../../augmented-stellar-density.md), not a unique solution determined by the one-variable density: different extensions off the physical curve encode different anisotropies, and not every formal extension necessarily gives a nonnegative [galactic distribution function](../../../../../galactic-distribution-function.md).

For the [hypervirial density-potential family](../../../../../hypervirial-density-potential-family.md), differentiate the potential and use the [spherical shell theorem](../../../../../spherical-shell-theorem.md):

$$
\psi'=-\frac{GM r^{p-1}}{(a^p+r^p)^{1+1/p}},\qquad M(<r)=-\frac{r^2\psi'}{G}=\frac{M r^{p+1}}{(a^p+r^p)^{1+1/p}}.
$$

Differentiating $M(<r)$ and dividing by $4\pi r^2$ gives

$$
\boxed{\rho=\frac{(p+1)M}{4\pi}\frac{a^p r^{p-2}}{(a^p+r^p)^{2+1/p}}.}
$$

The enclosed mass tends to $M$ at infinity and to zero at the centre for every $p>0$. The same result follows from $\nabla^2\psi=-4\pi G\rho$, with the stated sign convention.

From now on set $G=M=a=1$. The separable [augmented density](../../../../../augmented-stellar-density.md) is $\rho(r,q)=(p+1)r^{p-2}q^{2p+1}/(4\pi)$. Integrating it gives

$$
A=\frac{\rho\psi}{2(p+1)},\qquad B=\frac p2 A,
$$

and hence

$$
\boxed{\langle v_r^2\rangle=\frac{\psi}{2(p+1)},\qquad\langle v_\theta^2\rangle=\langle v_\phi^2\rangle=\frac{p\psi}{4(p+1)}.}
$$

With $\psi=(1+r^p)^{-1/p}$ these are the requested radial expressions. The [velocity-anisotropy parameter](../../../../../velocity-anisotropy-parameter.md) is $\beta=1-p/2$, and the total mean square speed is $\langle v^2\rangle=\psi/2$.

The local kinetic-energy density is $t=\rho\langle v^2\rangle/2=\rho\psi/4$. With the potential zero at infinity, the gravitational energy density is $w=\rho\Phi/2=-\rho\psi/2$, where $\Phi=-\psi$. Therefore

$$
\boxed{2t+w=0\quad\text{at every radius}.}
$$

This is the [local virial relation of the hypervirial model](../../../../../local-virial-relation-of-the-hypervirial-model.md), a special property stronger than the global [virial theorem](../../../../../virial-theorem.md). To compute the global energies as well, set $I=\int\rho\psi\,d^3x$. The substitution $u=r^p$ yields the [global binding integral of the hypervirial model](../../../../../global-binding-integral-of-the-hypervirial-model.md)

$$
I=\frac{p+1}{p}\int_0^\infty u^{1/p}(1+u)^{-2-2/p}\,du=\frac{p+1}{p}\frac{\Gamma(1+1/p)^2}{\Gamma(2+2/p)}.
$$

The [beta function](../../../../../beta-function.md) integral converges for all $p>0$. Thus

$$
\boxed{T=\frac I4,\qquad W=-\frac I2,\qquad2T+W=0.}
$$

Restoring dimensions multiplies $I,T,W$ by $GM^2/a$.

To derive the [hypervirial distribution function](../../../../../hypervirial-distribution-function.md), let $E=\psi-v^2/2$ be the positive [relative energy](../../../../../relative-energy.md) and $L=rv\sin\vartheta$ the magnitude of the [specific angular momentum](../../../../../specific-angular-momentum.md). Seek $F=C L^{p-2}E^s$ for $E>0$ and zero otherwise. Its density is

$$
\rho=2\pi C r^{p-2}\int_0^\pi\sin^{p-1}\vartheta\,d\vartheta\int_0^{\sqrt{2\psi}}v^p(\psi-v^2/2)^s\,dv.
$$

The angular integral is $\sqrt\pi\Gamma(p/2)/\Gamma((p+1)/2)$. Substitution $z=v^2/(2\psi)$ makes the radial integral

$$
2^{(p-1)/2}\psi^{s+(p+1)/2}B\left(\frac{p+1}{2},s+1\right).
$$

Matching the augmented-density power $\psi^{2p+1}$ gives $s=(3p+1)/2$. Matching its coefficient gives the [normalization of the hypervirial distribution function](../../../../../normalization-of-the-hypervirial-distribution-function.md)

$$
\boxed{F(E,L)=C L^{p-2}E^{(3p+1)/2},\qquad C=\frac{(p+1)\Gamma(2p+2)}{2^{(p+5)/2}\pi^{5/2}\Gamma(p/2)\Gamma((3p+3)/2)}.}
$$

All integrals are finite in [velocity](../../../../../velocity.md) for $p>0$, and $C>0$. Because $E$ and $L$ are orbital integrals, this is a steady solution by the [Jeans theorem](../../../../../jeans-theorem.md). As checks, $p=1$ gives $C=3/(4\pi^3)$ for the [Hernquist model](../../../../../hernquist-model.md), and $p=2$ gives $C=24\sqrt2/(7\pi^3)$ for the isotropic [Plummer model](../../../../../plummer-model.md).

**The density and potential do not uniquely fix the stellar distribution.** The preceding coefficient is fixed within the chosen separable power-law model, but [nonuniqueness of spherical galactic distribution functions](../../../../../nonuniqueness-of-spherical-galactic-distribution-functions.md) remains without that extra restriction. An explicit positive counterexample uses the same $p=2$ density. Define the [Osipkov-Merritt distribution function](../../../../../osipkov-merritt-distribution-function.md) variable $Q=E-L^2/2$ and take

$$
F_{\mathrm{OM}}(E,L)=\frac{3}{\sqrt2\pi^3}Q^{3/2}\quad(Q>0),\qquad F_{\mathrm{OM}}=0\quad(Q\leq0).
$$

Rescale the transverse [velocity](../../../../../velocity.md) by $\sqrt{1+r^2}$. Then $Q=\psi-[v_r^2+(1+r^2)v_t^2]/2$ and the [velocity](../../../../../velocity.md) Jacobian contributes $(1+r^2)^{-1}$. Direct integration gives

$$
\rho_{\mathrm{OM}}=\frac{3}{4\pi}\frac{\psi^3}{1+r^2}=\frac{3}{4\pi}\psi^5,
$$

exactly the same [Plummer model](../../../../../plummer-model.md) density. This [anisotropic Plummer distribution with unit anisotropy radius](../../../../../anisotropic-plummer-distribution-with-unit-anisotropy-radius.md) has $\beta=r^2/(1+r^2)$, so it is distinct from the isotropic $E^{7/2}$ distribution while remaining positive and spherical. Its second moments differ, so it does not share the extra augmented-density and local-virial restrictions of the chosen hypervirial model.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 320](../../paper-320-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
