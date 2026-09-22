<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the leading vertically averaged horizontal momentum equations of a [thin disk](../../../../../../thin-disk.md). For an isothermal [ideal gas](../../../../../../ideal-gas.md), write $P=\int p\,dz=c_s^2\Sigma$, with constant [isothermal sound speed](../../../../../../isothermal-sound-speed.md) $c_s$. The [disk scale height](../../../../../../disk-scale-height.md) is of order $H=c_s/\Omega_z$; this is exact for local isothermal vertical hydrostatic balance and remains the thickness scale for the estimate. Put $\epsilon=H/r\ll1$. The [alpha disk](../../../../../../alpha-disk.md) prescription gives

$$
\nu\sim\alpha c_sH\sim\alpha\epsilon^2r^2\Omega_z.
$$

At fixed radii of order $a$ inside the plunge and away from the marginal orbit, $|v_r|,v_\phi$ and $r\Omega_z$ are fixed numerical multiples of $(GM/a)^{1/2}$. Hence the inflow time is dynamical, while the [viscous timescale](../../../../../../viscous-timescale.md) is longer by $1/(\alpha\epsilon^2)$.

The [Paczyński-Wiita ballistic plunge](../../../../../../paczynski-wiita-ballistic-plunge.md) obeys $v_rv_r'-v_\phi^2/r=-\Phi'$ and $v_rj_0'=0$ exactly. For smoothly varying disk quantities on scale $r$, the pressure correction to radial acceleration has magnitude $c_s^2/r$, and the viscous correction is of order $\nu v/r^2$. Relative to the orbital acceleration scale $r\Omega_z^2$, these are respectively

$$
\boxed{O(\epsilon^2)\quad\text{and}\quad O(\alpha\epsilon^2)}.
$$

Finite-height corrections to the mid-plane gravitational force are also $O(\epsilon^2)$ by reflection symmetry. Thus the leading horizontal flow is $\mathbf u_h=\mathbf v+O(\epsilon^2v)$, with specific angular momentum differing from $j_0$ by a fraction $O(\alpha\epsilon^2)$ over a dynamical transit, for $\alpha\lesssim1$. Vertical structure and the smaller vertical velocity must be supplied by the thin-disk expansion; they are not specified by the planar ballistic expression.

This estimate is not uniform at the marginal orbit. In the ballistic solution, steady mass conservation gives

$$
\Sigma=\frac{\dot M}{2\pi r|v_r|}
=\frac{\dot M\sqrt a}{\pi\sqrt{GM}}\frac{\sqrt{r-a}}{(3a-r)^{3/2}}.
$$

Consequently $d\ln\Sigma/dr=[2(r-a)]^{-1}+3[2(3a-r)]^{-1}$. Writing $\delta=3a-r\ll a$, the pressure acceleration scales as $c_s^2/\delta$, while the net ballistic radial force scales as $(GM/a^2)(\delta/a)^2$. Their ratio is $O[\epsilon^2(a/\delta)^3]$, evaluated with the characteristic thickness near $3a$. A transonic matching layer of width $\delta/a=O(\epsilon^{2/3})$ is therefore needed. The approximation concerns the bulk plunging flow outside that layer, not a uniform relative approximation arbitrarily close to $3a$.

For the torque comparison, the steady angular-momentum flux is $\mathcal G-\dot Mj=\mathrm{constant}$, where $\mathcal G=-2\pi\nu\Sigma r^3\Omega'$ is the [viscous torque in an accretion disk](../../../../../../viscous-torque-in-an-accretion-disk.md). Inside the plunge, $\Omega=j_0/r^2$, so

$$
\mathcal G=4\pi\nu\Sigma j_0,\qquad
\frac{\mathcal G}{\dot Mj_0}=\frac{2\nu}{r|v_r|}=O(\alpha\epsilon^2).
$$

Outside, the approximately circular disk has $\mathcal G=\dot M[j(r)-j_0]+O(\alpha\epsilon^2\dot Mj_0)$, since the inner plunge torque is small. At $4a$,

$$
j(4a)-j_0=\left(\frac83-\frac{3\sqrt3}{2}\right)\sqrt{GMa}>0,
$$

a fixed number independent of disk thickness. At $2a$, radial infall is dynamical and the inner torque is $O(\alpha\epsilon^2\dot Mj_0)$. Therefore the [weak viscous torque in a thin-disk plunging region](../../../../../../weak-viscous-torque-in-a-thin-disk-plunging-region.md) estimate gives

$$
\boxed{\frac{\mathcal G(2a)}{\mathcal G(4a)}=O\!\left[\alpha\left(\frac Hr\right)^2\right]}.
$$

The numerical prefactor need not be small; the suppression is an asymptotic statement in the thin-disk parameter. Rapid infall and its low surface density explain why a nearly zero inner torque is a useful leading boundary condition for the outer accretion disk.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
