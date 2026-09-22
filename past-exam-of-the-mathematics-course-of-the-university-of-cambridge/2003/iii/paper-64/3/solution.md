<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use $S(z)=\sigma+k_xU(z)$, $k^2=k_x^2+k_y^2>0$ and primes for $z$ derivatives. Time dependence is $e^{i\sigma t}$, so exponential growth means $\operatorname{Im}\sigma<0$. The constant [mass density](../../../../../density.md) and incompressible [velocity](../../../../../velocity.md) give

$$
ik_xu+ik_yv+w'=0.
$$

All magnetic factors below use the source convention $\mu_0=1$.

Linearizing the [ideal magnetohydrodynamic momentum equation](../../../../../ideal-magnetohydrodynamic-momentum-equation.md), the advective perturbation is $iS\mathbf u_1+U'w\mathbf e_x$. The magnetic force is $(\nabla\times\mathbf b)\times B\mathbf e_x$, whose $x$ component vanishes. Thus the three component equations are

$$
\begin{aligned}
i\rho Su+\rho U'w&=-ik_xp_1,\\
i\rho Sv-B(ik_xb_y-ik_yb_x)&=-ik_yp_1,\\
i\rho Sw-B(ik_xb_z-b_x')&=-p_1'.
\end{aligned}
$$

In particular the vertical equation has the pressure-gradient and magnetic signs printed in the PDF.

The incompressible [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md) can be written $D\mathbf B/Dt=(\mathbf B\cdot\nabla)\mathbf u$. Linearizing it gives

$$
iSb_x=ik_xBu+U'b_z,
\qquad iSb_y=ik_xBv,
\qquad iSb_z=ik_xBw.
$$

For $S\ne0$, these are

$$
\boxed{b_x=\frac{k_xB}{S}\left(u-\frac{iU'w}{S}\right),
\qquad b_y=\frac{k_xB}{S}v,
\qquad b_z=\frac{k_xB}{S}w.}
$$

The $U'b_z$ term is essential: a perturbed vertical magnetic component is stretched by the background [shear flow](../../../../../shear-flow.md). Differentiating these amplitudes and using incompressibility also verifies $ik_xb_x+ik_yb_y+b_z'=0$.

For completeness, substitution into all three [momentum](../../../../../momentum.md) equations gives

$$
\begin{aligned}
i\rho Su+\rho U'w&=-ik_xp_1,\\
i\rho Sv&=-ik_yp_1+\frac{k_xB^2}{S}
\left(\zeta-\frac{k_yU'w}{S}\right),\\
i\rho Sw-\frac{ik_x^2B^2}{S}w
+k_xB^2\left(\frac uS-\frac{iU'w}{S^2}\right)'&=-p_1',
\end{aligned}
$$

where $\zeta=ik_xv-ik_yu$ is the vertical [vorticity](../../../../../vorticity.md) amplitude. Multiplying the $y$ equation by $k_x$ and subtracting $k_y$ times the $x$ equation eliminates [pressure](../../../../../pressure.md):

$$
\left(\rho S-\frac{k_x^2B^2}{S}\right)
\left(\zeta-\frac{k_yU'w}{S}\right)=0.
$$

Therefore, away from $\rho S^2=k_x^2B^2$,

$$
\boxed{\zeta=\frac{k_yU'w}{S},\qquad i\rho Sv=-ik_yp_1.}
$$

This is the nonresonant reduction relevant to the instability calculation. Division at the [Alfvén wave](../../../../../alfven-wave.md) resonance would be invalid. For a concrete counterexample to an unrestricted reading, take constant $U$, $k_y=0$, $S=\pm k_xB/\sqrt\rho$, $v=a(z)$ and $b_y=k_xBa(z)/S$, with all other amplitudes zero. Every smooth $a(z)$ solves the original linear system, but $\zeta=ik_xa(z)$ need not vanish. These transverse resonant waves do not drive $w$. A genuinely growing mode in a real background has complex $S$ and cannot satisfy either $S=0$ or $S^2=k_x^2B^2/\rho$ on the real $z$ axis. This explains exactly when the requested reductions may be used.

On that nonresonant branch, multiply the horizontal equations by $k_x$ and $k_y$ and add. Incompressibility gives $k_xu+k_yv=iw'$, so

$$
-\rho Sw'+\rho k_xU'w=-ik^2p_1,
\qquad
\boxed{ik^2p_1=\rho Sw'-\rho k_xU'w.}
$$

Combining incompressibility with [vorticity](../../../../../vorticity.md), multiply its first equation by $k_x$ and subtract $k_y$ times the definition of $\zeta$. This gives

$$
\boxed{ik^2u=-k_xw'-k_y\zeta
=-\left(k_xw'+\frac{k_y^2U'}S w\right).}
$$

Consequently

$$
\frac uS-\frac{iU'w}{S^2}
=\frac{ik_x}{k^2}\left(\frac{w'}S-\frac{k_xU'w}{S^2}\right)
=\frac{ik_x}{k^2}\left(\frac wS\right)'.
$$

Substitute this and the derivative of the displayed [pressure](../../../../../pressure.md) relation into vertical [momentum](../../../../../momentum.md). Multiplication by $k^2/i$ gives

$$
\left[\rho Sw'-\rho k_xU'w\right]'
=k^2\rho Sw+k_x^2B^2\left[\left(\frac wS\right)''-\frac{k^2w}S\right].
$$

Expanding the second derivative once gives exactly the requested vertical-velocity equation:

$$
\boxed{\begin{aligned}
\left[\rho Sw'-\rho k_xU'w\right]'
&=k^2\rho Sw+k_x^2B^2\left[\left(\frac{w'}S\right)'-\frac{k^2w}S\right]\\
&\quad-k_x^3B^2\left(\frac{U'w}{S^2}\right)'.
\end{aligned}}
$$

To take the discontinuous-layer limit without multiplying distributions, introduce $f=w/S$. It is proportional to the normal [displacement](../../../../../displacement.md): the material kinematic condition is $w=iS\eta$, so $f=i\eta$. Since $S'=k_xU'$, $Sw'-S'w=S^2f'$. The same equation becomes the [displacement equation for a parallel magnetic shear flow](../../../../../displacement-equation-for-a-parallel-magnetic-shear-flow.md)

$$
\boxed{\left[(\rho S^2-k_x^2B^2)f'\right]'
-k^2(\rho S^2-k_x^2B^2)f=0.}
$$

The physical interface condition is continuity of $f$, because both fluids move the same interface. For constant $U_j$ on each side, away from resonance the coefficient is constant and nonzero, so $f''-k^2f=0$. Requiring decay at infinity and matching $f(0)$ yields

$$
\boxed{w(z)=
\begin{cases}
A(\sigma+k_xU_2)e^{-kz},&z>0,\\
A(\sigma+k_xU_1)e^{kz},&z<0.
\end{cases}}
$$

The exponent is $z$, as in the actual PDF; the converted TeX's $x$ there is a transcription error.

Integrate the conservative [displacement](../../../../../displacement.md) equation across a layer of thickness $2\varepsilon$. Its undifferentiated term has an integral tending to zero, while the derivative gives

$$
[(\rho S^2-k_x^2B^2)f']_{0^-}^{0^+}=0.
$$

Equivalently, the perturbed [magnetohydrodynamic total pressure](../../../../../magnetohydrodynamic-total-pressure.md) is $p_1+Bb_x=(\rho S^2-k_x^2B^2)f'/(ik^2)$ and is continuous. With $f'_+=-kA$ and $f'_-=kA$, a nontrivial amplitude requires

$$
\boxed{\rho(\sigma+k_xU_2)^2+\rho(\sigma+k_xU_1)^2=2k_x^2B^2.}
$$

This is also the rigorous thin-layer integration of the original vertical equation, after combining the derivative terms before taking the limit.

Put $\overline U=(U_1+U_2)/2$ and $\Delta U=U_2-U_1$. Completing the square gives the [dispersion relation](../../../../../dispersion-relation.md)

$$
\boxed{\sigma=-k_x\overline U
\pm k_x\sqrt{\frac{B^2}{\rho}-\frac{(\Delta U)^2}{4}}.}
$$

For $(\Delta U)^2<4B^2/\rho$ both interface frequencies are real, so there is **no exponentially growing interface mode**. Above that threshold, the growing sign has [growth rate](../../../../../growth-rate.md) $|k_x|\sqrt{(\Delta U)^2/4-B^2/\rho}$. This is [magnetic stabilization of an equal-density vortex sheet](../../../../../magnetic-stabilization-of-an-equal-density-vortex-sheet.md): [magnetic tension](../../../../../magnetic-tension.md) from bending the field overcomes the kinetic shear driving [Kelvin-Helmholtz instability](../../../../../kelvin-helmholtz-instability.md). Equality is marginal and the strict stable condition avoids its double-root degeneracy. The case $k_x=0$ has no streamwise shear drive and has the neutral interface frequency $\sigma=0$; the nonzero-frequency elimination should be interpreted by the original equations or a limiting [displacement](../../../../../displacement.md) formulation in that case. The horizontal $k_y$ affects the exponential decay length through $k$, but not the stated threshold.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
