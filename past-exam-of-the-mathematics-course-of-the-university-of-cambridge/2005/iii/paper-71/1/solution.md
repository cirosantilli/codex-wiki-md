<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use signed [velocities](../../../../../velocity.md) in the [shock frame](../../../../../shock-frame.md); the [Mach number](../../../../../mach-number.md) depends on their squares. For a genuine nonradiative [perfect gas](../../../../../ideal-gas.md) [shock wave](../../../../../shock-wave.md), the [Rankine-Hugoniot conditions for a perfect gas](../../../../../rankine-hugoniot-conditions-for-a-perfect-gas.md) give a common [mass flux](../../../../../mass-flux.md) $j=\rho_Lu_L=\rho_Ru_R$, a common [momentum flux](../../../../../momentum-flux.md) $p+\rho u^2$, and a common specific stagnation [enthalpy](../../../../../enthalpy.md) $\gamma p/[(\gamma-1)\rho]+u^2/2$. Here $e$ in the given [equation of state](../../../../../equation-of-state.md) is [specific internal energy](../../../../../specific-internal-energy.md), despite the source's informal “energy density” wording.

Put $r=\rho_R/\rho_L$, $P=p_R/p_L$ and $M^2=\rho_Lu_L^2/(\gamma p_L)$. Mass and momentum give $u_R=u_L/r$ and $P=1+\gamma M^2(1-1/r)$. Substituting these into the energy relation and clearing denominators gives

$$
(r-1)\left[((\gamma-1)M^2+2)r-(\gamma+1)M^2\right]=0.
$$

The $r=1$ factor is the no-jump solution. On the nontrivial [shock wave](../../../../../shock-wave.md) branch,

$$
\boxed{r=\frac{(\gamma+1)M^2}{(\gamma-1)M^2+2},\qquad
P=\frac{2\gamma M^2-(\gamma-1)}{\gamma+1}.}
$$

In particular $r-1=2(M^2-1)/[(\gamma-1)M^2+2]$. With $\gamma>1$, compression is therefore equivalent to $M_L^2>1$. The other [Mach number](../../../../../mach-number.md) is

$$
M_R^2=\frac{M_L^2}{rP}
=\frac{(\gamma-1)M_L^2+2}{2\gamma M_L^2-(\gamma-1)}.
$$

Positive [pressure](../../../../../pressure.md) makes its denominator positive, and $M_R^2-1$ has the opposite sign to $M_L^2-1$. Thus a nontrivial physical [shock wave](../../../../../shock-wave.md) has a supersonic side and a subsonic side; the entropy-admissible flow goes from the former to the latter.

The [shock compression ratio](../../../../../shock-compression-ratio.md) also yields $u_Lu_R=(\gamma-1)u_L^2/(\gamma+1)+2\gamma p_L/[(\gamma+1)\rho_L]$. Rearranging produces the first [velocity](../../../../../velocity.md) identity in the question. The [pressure](../../../../../pressure.md) relation gives the second identity in the equivalent form

$$
p_R=\frac{2\rho_Lu_L^2-(\gamma-1)p_L}{\gamma+1}.
$$

The numerator here contains [mass density](../../../../../density.md), as the original PDF shows; the converted TeX incorrectly replaces that [mass density](../../../../../density.md) by [pressure](../../../../../pressure.md).

For reflection, the once-shocked gas is the common left state in both applications. Before rebound, its [velocity](../../../../../velocity.md) in the [shock frame](../../../../../shock-frame.md) is $a=u_s-U_+<0$ and the gas ahead has [velocity](../../../../../velocity.md) $-U_+$; after rebound, it is $b=u_s+U_->0$ and the gas next to the wall has [velocity](../../../../../velocity.md) $U_-$. In both cases the right [velocity](../../../../../velocity.md) minus the left [velocity](../../../../../velocity.md) equals $-u_s$. Applying the first identity therefore gives the same [quadratic equation](../../../../../quadratic-equation.md),

$$
v^2-\frac{\gamma+1}{2}u_sv-\frac{\gamma p_s}{\rho_s}=0,
$$

with roots $a$ and $b$. Their opposite signs distinguish the two roots, so **$\boxed{(u_s-U_+)(u_s+U_-)=-\gamma p_s/\rho_s}$**.

Write $q_0=p_0/p_s$, $q_1=p_1/p_s$. The [pressure](../../../../../pressure.md) identity applied to each [shock wave](../../../../../shock-wave.md) gives

$$
a^2=\frac{p_s}{2\rho_s}[(\gamma+1)q_0+\gamma-1],\qquad
b^2=\frac{p_s}{2\rho_s}[(\gamma+1)q_1+\gamma-1].
$$

Squaring the root-product relation and eliminating the [velocities](../../../../../velocity.md) yields

$$
[(\gamma+1)q_0+\gamma-1][(\gamma+1)q_1+\gamma-1]=4\gamma^2,
$$

and hence the [normal shock reflection at a rigid wall](../../../../../normal-shock-reflection-at-a-rigid-wall.md) relation

$$
\boxed{\frac{p_1}{p_s}=\frac{3\gamma-1-(\gamma-1)p_0/p_s}{\gamma-1+(\gamma+1)p_0/p_s}.}
$$

Taking $p_0/p_s\to0$ gives **$\boxed{p_1/p_s\to(3\gamma-1)/(\gamma-1)}$**; for a [monatomic gas](../../../../../monatomic-gas.md) this limiting amplification is six.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
