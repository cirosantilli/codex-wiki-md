<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

With no electric force, the [Lorentz force](../../../../../lorentz-force.md) equation is

$$
\boxed{m\ddot{\mathbf x}=e\dot{\mathbf x}\times\mathbf B(\mathbf x,t)}.
$$

Its scalar product with [velocity](../../../../../velocity.md) proves [conservation of energy](../../../../../conservation-of-energy.md) for the particle's [kinetic energy](../../../../../kinetic-energy.md):

$$
\frac{d}{dt}\left(\frac m2|\dot{\mathbf x}|^2\right)=e\dot{\mathbf x}\cdot(\dot{\mathbf x}\times\mathbf B)=0.
$$

If $\mathbf B=\mathcal B(\mathbf x,t)\widehat{\mathbf b}$ with a fixed unit direction $\widehat{\mathbf b}$, then $m\ddot{\mathbf x}\cdot\widehat{\mathbf b}=0$, so the parallel component of [velocity](../../../../../velocity.md) is constant even when the field magnitude varies.

The [angular momentum](../../../../../angular-momentum.md) about the origin does not generally remain constant, because

$$
\dot{\mathbf L}=e\mathbf x\times(\dot{\mathbf x}\times\mathbf B)=e\left[\dot{\mathbf x}(\mathbf x\cdot\mathbf B)-\mathbf B(\mathbf x\cdot\dot{\mathbf x})\right].
$$

For example, at an instant with $\mathbf x=(r_0,0,0)$, $\dot{\mathbf x}=(v_0,0,0)$ and $\mathbf B=(0,0,B)$, its derivative is $(0,0,-eBr_0v_0)$, nonzero when those factors are nonzero. A force perpendicular to [velocity](../../../../../velocity.md) can preserve [kinetic energy](../../../../../kinetic-energy.md) while exerting a nonzero [torque](../../../../../torque.md).

For the constant axial field, Cartesian equations are $m\ddot x=eB\dot y$, $m\ddot y=-eB\dot x$, and $\ddot z=0$. Use the signed projected areal rate $\dot A=(x\dot y-y\dot x)/2=r^2\dot\theta/2$. Then

$$
m\ddot A=\frac m2(x\ddot y-y\ddot x)=-\frac{eB}{2}(x\dot x+y\dot y)=-\frac{eB}{4}\frac{d(r^2)}{dt}.
$$

Thus

$$
\boxed{m\dot A+\frac{eBr^2}{4}=c,\qquad mr^2\dot\theta+\frac{eBr^2}{2}=2c}.
$$

The second equation is the [magnetic axial angular-momentum invariant](../../../../../magnetic-axial-angular-momentum-invariant.md), replacing ordinary conservation of $L_z=mr^2\dot\theta$. In the [symmetric gauge](../../../../../symmetric-gauge.md), the added term is the magnetic contribution to canonical [angular momentum](../../../../../angular-momentum.md); it is the axial component that is conserved, not the full mechanical angular-momentum vector.

Let $v^2=\dot x^2+\dot y^2$ be the constant squared transverse [speed](../../../../../speed.md). If the motion has a nonzero parallel [speed](../../../../../speed.md), $v^2=2K/m-\dot z^2$, where $K$ is total [kinetic energy](../../../../../kinetic-energy.md). Solving the invariant and using $v^2=\dot r^2+r^2\dot\theta^2$ gives

$$
\boxed{\dot\theta=\frac{2c}{mr^2}-\frac{eB}{2m},\qquad \dot r=\pm\sqrt{v^2-\left(\frac{2c}{mr}-\frac{eBr}{2m}\right)^2}}.
$$

The TeX transcription omits the angular equation, which is present in the PDF and restored here. The PDF's positive radial root describes the outward branch only. An inward branch needs the minus sign, with sign changes at radial turning points; polar coordinates themselves are singular at $r=0$. These qualifications are needed for a global description of a cyclotron trajectory whose radius about an arbitrary origin can both increase and decrease.

The initial time-dependent-field discussion treats the stipulated magnetic force as a prescribed particle model. If one additionally imposes full [Maxwell equations](../../../../../maxwell-equations.md) with electric field zero throughout a region, [Faraday law](../../../../../faraday-s-law-of-induction.md) requires the magnetic field there to be time independent. The [energy](../../../../../energy.md) calculation is nevertheless valid for the stated force model; it does not assert existence of a Maxwell-consistent time-dependent field with zero electric field everywhere.

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
