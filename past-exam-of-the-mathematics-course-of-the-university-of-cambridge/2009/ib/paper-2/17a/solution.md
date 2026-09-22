<h1 id="17a/solution">Solution</h1>

↑ **Parent:** [17A](../17a.md)

The vacuum [Maxwell equations](../../../../../maxwell-equations.md) are $\nabla\cdot E=\nabla\cdot B=0$, $\nabla\times E=-B_t$ and $\nabla\times B=E_t/c^2$. Taking the curl of Faraday's equation and using $\nabla\times(\nabla\times E)=\nabla(\nabla\cdot E)-\nabla^2E$ gives $-\nabla^2E=-E_{tt}/c^2$. The same calculation for Ampère's equation gives $\nabla^2B=B_{tt}/c^2$. Hence **each Cartesian component satisfies the [electromagnetic wave equation](../../../../../electromagnetic-wave-equation.md)**.

Model the walls as a [perfect conductor](../../../../../perfect-conductor.md), with no oscillating fields in its interior. The tangential [electric field](../../../../../electric-field.md) is zero at the surface, otherwise it would drive unbounded conductor currents. The normal [magnetic field](../../../../../magnetic-field.md) is zero, since the divergence-free field has a continuous normal component and the interior oscillating field is zero. Thus $n\times E=0$ and $n\cdot B=0$. Normal $E$ and tangential $B$ may be nonzero because surface charge and surface current support their jumps.

The PDF writes the full [magnetic field](../../../../../magnetic-field.md) as $B=B_0(x,y)\hat z e^{i(kz-\omega t)}$. Taken literally, this cannot be a nonzero travelling wave: $\nabla\cdot B=ikB_z$, so for $k\ne0$ it forces $B_z=0$. The subsequent requests require transverse components. The consistent intended reading is **$B_z=B_0(x,y)e^{i(kz-\omega t)}$**, with transverse fields determined by the [Maxwell equations](../../../../../maxwell-equations.md). Use that reading below.

All fields have the same $z,t$ factor. Put $\Delta=(\omega/c)^2-k^2$. The harmonic [Maxwell equations](../../../../../maxwell-equations.md) are $\nabla\times E=i\omega B$ and $\nabla\times B=-i\omega E/c^2$. Their $x$ and $y$ components give

$$
E_y=-\frac{c^2k}{\omega}B_x-\frac{ic^2}{\omega}\partial_xB_z,\qquad
E_x=\frac{c^2k}{\omega}B_y+\frac{ic^2}{\omega}\partial_yB_z,
$$

together with $\partial_yE_z-ikE_y=i\omega B_x$ and $ikE_x-\partial_xE_z=i\omega B_y$. Substitution and solving, for $\Delta\ne0$, gives

$$
\boxed{B_x=\frac i\Delta\left(k\partial_xB_z-\frac\omega{c^2}\partial_yE_z\right),\qquad
B_y=\frac i\Delta\left(k\partial_yB_z+\frac\omega{c^2}\partial_xE_z\right).}
$$

The corresponding electric components are

$$
E_x=\frac i\Delta(k\partial_xE_z+\omega\partial_yB_z),\qquad
E_y=\frac i\Delta(k\partial_yE_z-\omega\partial_xB_z).
$$

For a [transverse electric mode of a rectangular waveguide](../../../../../transverse-electric-mode-of-a-rectangular-waveguide.md), $E_z=0$. The [electromagnetic wave equation](../../../../../electromagnetic-wave-equation.md) becomes

$$
(\partial_x^2+\partial_y^2+\Delta)B_0=0.
$$

At $x=0,a$, the tangential component $E_y=-i\omega\partial_xB_z/\Delta$ vanishes, so $\partial_xB_0=0$; at $y=0,b$, the corresponding condition $E_x=0$ gives $\partial_yB_0=0$. These are [Neumann boundary conditions](../../../../../neumann-boundary-condition.md), and the normal-$B$ conditions give the same conclusions through the displayed transverse magnetic components. Separation gives

$$
B_0=C_{mn}\cos\frac{m\pi x}{a}\cos\frac{n\pi y}{b},\qquad
\Delta=\kappa_{mn}^2=\left(\frac{m\pi}{a}\right)^2+\left(\frac{n\pi}{b}\right)^2,
$$

where $m,n\ge0$ are integers and $(m,n)\ne(0,0)$. The constant candidate is not a physical oscillating mode: its transverse derivatives vanish, so it has $E=0$ and Faraday's equation forces $B=0$ for $\omega\ne0$. More generally a hollow single-conductor guide has no transverse-electromagnetic zero-cutoff mode: its transverse electrostatic potential is harmonic with the same constant boundary value, hence constant, leaving zero transverse field.

The dispersion relation is $\omega^2=c^2(k^2+\kappa_{mn}^2)$. The [waveguide cutoff frequency](../../../../../waveguide-cutoff-frequency.md) for this mode is $\omega_{mn}=c\kappa_{mn}$; below it $k$ is imaginary and the field is evanescent. Since $a\ge b$, the lowest cutoff occurs at $(m,n)=(1,0)$:

$$
\boxed{\omega_c=\frac{\pi c}{a},\qquad f_c=\frac c{2a}.}
$$

For a mode propagating in the positive $z$ direction ($k>0$), above its own cutoff $\omega_{mn}$, the [phase velocity](../../../../../phase-velocity.md) and [group velocity](../../../../../group-velocity.md) are

$$
\boxed{v_{\mathrm{ph}}=\frac\omega k=\frac c{\sqrt{1-(\omega_{mn}/\omega)^2}}>c,\qquad
v_g=\frac{d\omega}{dk}=c\sqrt{1-(\omega_{mn}/\omega)^2}<c.}
$$

These [waveguide phase and group velocities](../../../../../waveguide-phase-and-group-velocities.md) have product $c^2$. The superluminal phase speed describes motion of a constant phase, while a narrow wave packet travels at the subluminal [group velocity](../../../../../group-velocity.md); it does not transmit information faster than light. At cutoff $k=0$ there is no travelling mode with nonzero longitudinal flux.

## ↑ Ancestors (10)

1. [17A](../17a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
