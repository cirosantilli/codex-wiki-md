<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md) of the [particle Lagrangian in a shearing sheet](../../../../../../particle-lagrangian-in-a-shearing-sheet.md) are

$$
\ddot x-2\Omega_0\dot y-2q_0\Omega_0^2x=0,\qquad
\ddot y+2\Omega_0\dot x=0,\qquad
\ddot z+\Omega_z^2z=0.
$$

The terms coupling $x$ and $y$ are the [Coriolis acceleration](../../../../../../coriolis-acceleration.md). The [cyclic coordinate](../../../../../../cyclic-coordinate.md) $y$ has conserved [canonical momentum](../../../../../../canonical-momentum.md)

$$
p_y=\frac{\partial L_2}{\partial\dot y}=\dot y+2\Omega_0x.
$$

For a [Newtonian potential of a point mass](../../../../../../newtonian-potential-of-a-point-mass.md), $q_0=3/2$ and $\Omega_z=\kappa_r=\Omega_0$. Set $p_y=\Omega_0x_0/2$ and substitute $\dot y=p_y-2\Omega_0x$ in the radial equation. It becomes $\ddot x+\Omega_0^2(x-x_0)=0$, a [harmonic oscillator equation](../../../../../../simple-harmonic-motion.md) about the [epicyclic guiding center](../../../../../../epicyclic-guiding-center.md) $x_0$. Integration gives

$$
\boxed{\begin{aligned}
x&=x_0+\operatorname{Re}(Ae^{-i\Omega_0t}),\\
y&=y_0-\frac32\Omega_0x_0t+\operatorname{Re}(-2iAe^{-i\Omega_0t}),\\
z&=\operatorname{Re}(Be^{-i\Omega_0t}).
\end{aligned}}
$$

The four real constants in $A,y_0,x_0$ and the two in $B$ account for the six initial position and velocity data.

Expanding the inertial [specific angular momentum](../../../../../../specific-angular-momentum.md) gives $h=h_0+r_0p_y+O(2)$. Thus $p_y$ measures the angular-momentum offset from the reference [circular orbit](../../../../../../circular-orbit.md), and $x_0$ specifies the radius of its associated [epicyclic guiding center](../../../../../../epicyclic-guiding-center.md).

The conserved horizontal energy in the rotating frame is

$$
\varepsilon_h=\frac12(\dot x^2+\dot y^2)-\frac32\Omega_0^2x^2
=\boxed{\frac12\Omega_0^2\left(|A|^2-\frac34x_0^2\right)}.
$$

It is the horizontal part of the local [Jacobi energy in a shearing sheet](../../../../../../jacobi-energy-in-a-shearing-sheet.md), rather than the inertial [specific orbital energy](../../../../../../specific-orbital-energy.md). Its positive term is the [epicyclic energy](../../../../../../epicyclic-energy.md); its negative term is the energy of the background shear at guiding-center position $x_0$. Independently, the vertical [harmonic oscillator](../../../../../../simple-harmonic-motion.md) has conserved energy

$$
\varepsilon_v=\frac12(\dot z^2+\Omega_0^2z^2)
=\boxed{\frac12\Omega_0^2|B|^2}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
