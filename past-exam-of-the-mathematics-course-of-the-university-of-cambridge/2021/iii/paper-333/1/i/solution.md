<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The basic state has [velocity field](../../../../../../velocity-field.md)

$$
\boldsymbol U=(0,\Lambda x,0)
$$

and [buoyancy](../../../../../../buoyancy.md) $B=N^2z$. For disturbances independent of $y$, the [linearized equations](../../../../../../linearized-equation.md) are

$$
u_t-fv=-p_x,\qquad
v_t+(f+\Lambda)u=0,\qquad
w_t=-p_z+b,
$$



$$
b_t+N^2w=0,\qquad u_x+w_z=0.
$$

Substituting a [plane wave](../../../../../../plane-wave.md) proportional to $\exp[i(kx+mz-\omega t)]$ and eliminating $p$, $v$, and $b$ gives the [dispersion relation](../../../../../../dispersion-relation.md)

$$
\omega^2=\frac{N^2k^2+f(f+\Lambda)m^2}{k^2+m^2}.
$$

Thus the requested coefficients are

$$
\widetilde f^{\,2}=f(f+\Lambda),\qquad \widetilde g=N^2.
$$

An [instability](../../../../../../instability.md) exists precisely when some [wavenumber](../../../../../../wavenumber.md) pair makes $\omega^2<0$. Since the [Brunt–Väisälä frequency](../../../../../../buoyancy-frequency.md) satisfies $N^2>0$, this is possible exactly when

$$
f(f+\Lambda)<0.
$$

The basic [relative vorticity](../../../../../../relative-vorticity.md) is $\Lambda\boldsymbol e_z$, so its [absolute vorticity](../../../../../../absolute-vorticity.md) is $(f+\Lambda)\boldsymbol e_z$. Its [Ertel potential vorticity](../../../../../../ertel-potential-vorticity.md) is therefore

$$
Q=(f+\Lambda)N^2.
$$

The instability criterion can consequently be written as $fQ<0$: the vertical absolute vorticity has the opposite sign to the planetary vorticity. This is [inertial instability](../../../../../../inertial-instability.md), approached most directly by disturbances with $|m/k|\gg1$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
