<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the homogeneous [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) condition $k(\rho_0)\rho_0=a_0f(\rho_0)$. Evaluate $D_1,D_2$ at $(a_0,\rho_0)$ and abbreviate

$$
f_0=f(\rho_0),\quad f'_0=f'(\rho_0),\quad
\kappa=k(\rho_0)+\rho_0k'(\rho_0),\quad
c=\kappa-a_0f'_0.
$$

The quantity $c$ is the chemical relaxation rate with the cell density held fixed. Derivatives of $D_1,D_2$ do not enter this [linear stability analysis](../../../../../linear-stability.md): they multiply spatial derivatives of the homogeneous background or products of perturbations. For a [Fourier mode](../../../../../fourier-mode.md) with time dependence $e^{st}$, put $z=|\mathbf q|^2$ and write

$$
s\binom{\widehat a}{\widehat\rho}=M(z)\binom{\widehat a}{\widehat\rho},\qquad
M(z)=\begin{pmatrix}-D_2z&D_1z\\ f_0&-c-D_\rho z\end{pmatrix}.
$$

Consequently

$$
\operatorname{tr}M=-c-(D_2+D_\rho)z,\qquad
\det M=z[D_2(c+D_\rho z)-D_1f_0].
$$

At $z=0$, the [eigenvalues](../../../../../eigenvalue.md) are $0$ and $-c$. The neutral cell-density mode reflects [mass conservation](../../../../../mass-conservation.md), not decay of every homogeneous perturbation.

Write $a=D_2>0$, $b=D_\rho>0$, $C=D_1f_0$, and interpret production physically as $f_0\geq0$. If $c\geq0$, the [trace-determinant stability criterion](../../../../../trace-determinant-stability-criterion.md) shows that an unstable nonzero [wavenumber](../../../../../wavenumber.md) exists precisely when $C>ac$. The unstable band is

$$
0<z<z_c,\qquad z_c=\frac{C-ac}{ab}.
$$

If $c<0$, the chemical field is already unstable at zero [wavenumber](../../../../../wavenumber.md); arbitrarily small positive [wavenumbers](../../../../../wavenumber.md) are unstable too. Since $C\geq0$, this also implies $C>ac$. Thus, on the infinite plane, **the undivided [Keller--Segel aggregation threshold](../../../../../keller-segel-aggregation-threshold.md) is**

$$
\boxed{D_1f_0>D_2(\kappa-a_0f'_0).}
$$

For $\kappa>0$, dividing by $D_2\kappa$ gives the requested form

$$
\boxed{\frac{D_1f_0}{D_2\kappa}+\frac{a_0f'_0}{\kappa}>1.}
$$

At equality there is no strictly growing mode when $c\geq0$; nonzero spatial modes decay. On a finite domain, a permitted nonzero [wavenumber](../../../../../wavenumber.md) must actually lie in the unstable band. If one allows a signed production function, the displayed matrix and [trace-determinant stability criterion](../../../../../trace-determinant-stability-criterion.md) remain valid, but the simplification using $C\geq0$ must be revisited.

**The printed hypotheses do not ensure $\kappa>0$.** Positivity of the degradation rate $k$ alone is insufficient. For a concrete counterexample, take $k(\rho)=e^{-2\rho}$, $f(\rho)=e^{-2}$, $a_0=\rho_0=1$, and $D_1=D_2=D_\rho=1$. The homogeneous [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) condition holds, all rates and transport coefficients are positive, but $\kappa=c=-e^{-2}$. The printed left-hand side equals $-1$, although $\det M=z(z-2e^{-2})<0$ for $0<z<2e^{-2}$. These spatial modes grow. If $\kappa=0$, the printed expression is undefined. The undivided criterion and the matrix above resolve both cases.

To find the [fastest-growing Keller--Segel mode](../../../../../fastest-growing-keller-segel-mode.md), use the larger [eigenvalue](../../../../../eigenvalue.md)

$$
s_+(z)=-\frac{c+(a+b)z}{2}+\frac12\sqrt{[c+(b-a)z]^2+4Cz}.
$$

For $C>0$ the square root is real. Put $p=a+b$ and $d=b-a$. Differentiation gives

$$
s_+'(z)=-\frac p2+\frac{d(c+dz)+2C}{2\sqrt{(c+dz)^2+4Cz}}.
$$

A positive maximizing [wavenumber](../../../../../wavenumber.md) exists in either of two growing cases: $c\geq0$, $C>ac$, or $c<0$, $C>-bc$. Equivalently, $C>\max(ac,-bc)$. In this range $C+dc>0$, and

$$
s_+''(z)=-\frac{2C(C+dc)}{[(c+dz)^2+4Cz]^{3/2}}<0.
$$

Thus the stationary point is the unique maximum. The derivative condition yields

$$
ab[(c+dz_*)^2+4Cz_*]=C(C+dc).
$$

Solving it, with the root that satisfies the unsquared derivative equation, gives

$$
\boxed{z_*=
\begin{cases}
\displaystyle\frac{p\sqrt{C(C+dc)/(ab)}-dc-2C}{d^2},&a\ne b,\\[6pt]
\displaystyle\frac{C^2/a^2-c^2}{4C},&a=b.
\end{cases}\qquad
\ell_*=\frac{2\pi}{\sqrt{z_*}}.}
$$

For $c=0$, the unequal-diffusivity expression simplifies to $z_*=C/[\sqrt{ab}(\sqrt a+\sqrt b)^2]$, also agreeing with the equal-diffusivity limit. The formula maximizes the full two-field growth rate; it makes no instantaneous-chemical approximation. Every direction of $\mathbf q$ with this length is equivalent by [rotational symmetry](../../../../../rotational-symmetry.md).

If $c<0$ but $0\leq C\leq-bc$, the maximum instead occurs at $z=0$: **the fastest mode is homogeneous, with $s_*=-c$ and infinite [wavelength](../../../../../wavelength.md)**. For $C>0$, its initial derivative is $-b+C/(-c)\leq0$. If $C+dc\geq0$ the derivative thereafter decreases, while if $C+dc<0$ it increases towards the still-negative large-$z$ limit; either way no positive-$z$ maximum is missed. At $C=0$, the two [eigenvalues](../../../../../eigenvalue.md) are simply $-az$ and $-c-bz$, giving the same conclusion. In a finite box, maximize $s_+$ over the allowed [Fourier modes](../../../../../fourier-mode.md); excluding the homogeneous mode can change the selected length. In a stable parameter range there is no fastest-growing mode.

The first ratio compares the positive feedback loop “more cells produce more attractant, which draws in more cells” with spreading by cell [diffusion](../../../../../diffusion.md) and removal of chemical perturbations. Its numerator $D_1f_0$ measures [chemotaxis](../../../../../chemotaxis.md) together with attractant production; its denominator $D_2\kappa$ measures dispersal together with incremental degradation. **This competition between directed [chemotaxis](../../../../../chemotaxis.md) and cell [diffusion](../../../../../diffusion.md) produces spatial aggregation.** The second ratio compares the concentration dependence of chemical production, $a_0f'_0$, with incremental degradation $\kappa$. Positive $f'_0$ amplifies chemical fluctuations, whereas negative $f'_0$ suppresses them. It changes the chemical relaxation available to the [chemotaxis](../../../../../chemotaxis.md) feedback loop and can itself destabilize the homogeneous chemical field. Chemical [diffusion](../../../../../diffusion.md) $D_\rho$ suppresses short scales and sets the selected [wavelength](../../../../../wavelength.md), but does not change the infinite-plane long-wave threshold. These interpretations as ratios of stabilizing and destabilizing processes assume $\kappa>0$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
