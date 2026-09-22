<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $U=b\xi$ and $D=d\xi$. The [shock wave](../../../../../../shock-wave.md) conditions fix $b=2/(\gamma+1)$ and $d=(\gamma+1)/(\gamma-1)$. The [continuity equation](../../../../../../continuity-equation.md) then reduces to

$$
(b-1)+3b-\beta=0,
$$

so a linear [mass density](../../../../../../density.md) profile requires

$$
\boxed{\beta=4b-1=\frac{7-\gamma}{\gamma+1}}.
$$

Momentum requires $P'=-db(b-1+q)\xi^2$. At this exponent $q=-2(\gamma-1)/(\gamma+1)$, hence integration gives $P=2\xi^3/(\gamma+1)+P_0$. Substitution in the [pressure](../../../../../../pressure.md) equation makes the cubic coefficient vanish because $(\gamma+1)b=2$, while its constant term requires $(3\gamma b-3)P_0=0$. For $\gamma>1$ this implies $P_0=0$. Therefore all three equations and all [shock wave](../../../../../../shock-wave.md) conditions hold for the [linear-profile spherical blast wave](../../../../../../linear-profile-spherical-blast-wave.md),

$$
U=\frac{2\xi}{\gamma+1},\qquad
D=\frac{\gamma+1}{\gamma-1}\xi,\qquad
P=\frac{2\xi^3}{\gamma+1}.
$$

The prescribed range $0<\beta<3$ restricts this family to $1<\gamma<7$.

For $\gamma=5/3$ one has $\beta=2$, $a=2/3$, $U=3\xi/4$, $D=4\xi$ and $P=3\xi^3/4$. The [energy](../../../../../../energy.md) integral is

$$
\int_0^1\left[\frac12DU^2+\frac{P}{\gamma-1}\right]\xi^2\,d\xi
=\int_0^1\frac94\xi^5\,d\xi=\frac38.
$$

Consequently $E=(3\pi/2)CR\dot R^2=(2\pi/3)CR^3/t^2$, which fixes the radius and dimensional fields completely:

$$
\boxed{R(t)=\left(\frac{3E}{2\pi C}\right)^{1/3}t^{2/3},\qquad
u(r,t)=\frac{r}{2t},}
$$



$$
\boxed{\rho(r,t)=\frac{4Cr}{R^3(t)}=\frac{8\pi C^2r}{3Et^2},\qquad
p(r,t)=\frac{Cr^3}{3R^3(t)t^2}=\frac{2\pi C^2r^3}{9Et^4},\quad 0<r<R(t)}.
$$

The [kinetic energy](../../../../../../kinetic-energy.md) and [internal energy](../../../../../../internal-energy.md) integrands are each $9\xi^5/8$, so each accounts for half the explosion [energy](../../../../../../energy.md). Integrating the [mass density](../../../../../../density.md) also gives the correct swept-up mass $4\pi CR$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
