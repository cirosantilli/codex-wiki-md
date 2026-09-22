# Transonic accretion in a power-law tube

↑ **Parent:** [Transonic branch](transonic-branch.md)

Consider steady [isentropic flow](isentropic-flow.md) toward a [Newtonian gravitational potential](newtonian-gravitational-potential.md) $-GM/r$ through a tube of cross-sectional area $A(r)=Cr^n$. Write $v>0$ for the inward speed and use a [polytropic equation of state](polytropic-equation-of-state.md) with [specific-heat ratio](heat-capacity-ratio.md) $\gamma>1$. [Mass conservation](mass-conservation.md) and the [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md) give

$$
\rho v A=\dot M,
\qquad
\left(v-\frac{c_s^2}{v}\right)v'=\frac{nc_s^2}{r}-\frac{GM}{r^2},
$$

where $c_s$ is the [adiabatic sound speed](adiabatic-sound-speed.md). A regular [sonic point](sonic-point.md) therefore has $v_s=c_s$ and $r_s=GM/(nc_s^2)$. The [Bernoulli equation](bernoulli-equation.md), matched to a nearly stationary reservoir with [sound speed](speed-of-sound.md) $c_0$, gives

$$
\frac{v^2}{2}+\frac{c^2}{\gamma-1}-\frac{GM}{r}=\frac{c_0^2}{\gamma-1},
\qquad
c_s^2=\frac{2c_0^2}{(2n+1)-(2n-1)\gamma}.
$$

For $n>1/2$, a finite positive [sonic point](sonic-point.md) requires $1<\gamma<(2n+1)/(2n-1)$. Differentiating the flow equation at that point, with $x=r_sv'_s/c_s$, gives

$$
(\gamma+1)x^2+2n(\gamma-1)x+n^2(\gamma-1)-n=0.
$$

Its [discriminant](discriminant.md) is $4n[(2n+1)-(2n-1)\gamma]$, so the same bound permits real regular slopes. The branch on which the [Mach number](mach-number.md) rises inward selects the negative sign in

$$
x=\frac{-n(\gamma-1)\pm\sqrt{n[(2n+1)-(2n-1)\gamma]}}{\gamma+1}.
$$

For a spherical tube $n=2$, this recovers the $5/3$ threshold of [Bondi accretion](bondi-accretion.md); for a [dipolar flux-tube area](dipolar-flux-tube-area.md), $n=3$ gives $7/5$. The tube approximation must remain valid between the reservoir matching region and the accretor.

## ↑ Ancestors (7)

1. [Transonic branch](transonic-branch.md)
2. [Sonic point](sonic-point.md)
3. [Compressible flow](compressible-flow-split.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-64/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-314/4/c/solution.md)
- [Spherical polytropic flow with adiabatic exponent three halves](spherical-polytropic-flow-with-adiabatic-exponent-three-halves.md)
- [Transonic accretion in a dipolar flux tube](transonic-accretion-in-a-dipolar-flux-tube.md)
