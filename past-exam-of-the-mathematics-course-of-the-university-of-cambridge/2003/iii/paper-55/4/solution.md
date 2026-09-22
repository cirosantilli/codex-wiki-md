<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Cosmic inflation](../../../../../cosmic-inflation-split.md) addresses the [horizon problem](../../../../../horizon-problem.md) by extending the causal past of the observed region, the [flatness problem](../../../../../flatness-problem.md) by damping the curvature contribution, and the [cosmological monopole problem](../../../../../cosmological-monopole-problem.md) by diluting unwanted relics. A canonical [inflaton](../../../../../inflaton.md) can drive this expansion when its [potential energy](../../../../../potential-energy.md) density exceeds twice its [kinetic energy](../../../../../kinetic-energy.md) density.

Use the unreduced [Planck mass](../../../../../planck-mass.md) $m_P=G^{-1/2}$, consistent with the coefficient in the [Friedmann equation](../../../../../friedmann-equations.md), and take $V_0>0$, $c\ne0$. Seek the [exponential-potential power-law inflation](../../../../../exponential-potential-power-law-inflation.md) solution $\phi=A\log(\beta t)$ and $a=a_*(t/t_*)^p$. The [kinetic energy](../../../../../kinetic-energy.md) density is proportional to $t^{-2}$. The [inflaton potential](../../../../../inflaton-potential.md) must have the same scaling, so

$$
\frac{cA}{m_P}=2,\qquad A=\frac{2m_P}{c},\qquad V(\phi(t))=\frac{V_0}{\beta^2t^2}.
$$

Substitution into the [inflaton equation of motion](../../../../../inflaton-equation-of-motion.md) gives

$$
-A+3pA-\frac{cV_0}{m_P\beta^2}=0,
\qquad\frac{V_0}{\beta^2}=\frac{2m_P^2}{c^2}(3p-1).
$$

The [Friedmann equation](../../../../../friedmann-equations.md) now reduces to

$$
p^2=\frac{8\pi}{3m_P^2}\left(\frac{2m_P^2}{c^2}+\frac{2m_P^2}{c^2}(3p-1)\right)=\frac{16\pi p}{c^2}.
$$

Consequently the nontrivial positive-potential solution is

$$
\boxed{p=\frac{16\pi}{c^2},\qquad
\phi(t)=\frac{2m_P}{c}\log(\beta t),\qquad
\beta^2=\frac{V_0c^2}{2m_P^2(3p-1)},\qquad
a(t)=a_*\left(\frac{t}{t_*}\right)^p.}
$$

A positive $V_0$ requires $p>1/3$. [Accelerating expansion](../../../../../accelerating-expansion-of-the-universe.md) occurs exactly for $p>1$, giving

$$
\boxed{c^2<16\pi.}
$$

This is an exact solution, not a use of the [slow-roll approximation](../../../../../slow-roll-approximation.md). The [first Hubble slow-roll parameter](../../../../../first-hubble-slow-roll-parameter.md) and [equation-of-state parameter](../../../../../equation-of-state-parameter.md) are constant:

$$
\epsilon_H=-\frac{\dot H}{H^2}=\frac1p=\frac{c^2}{16\pi},\qquad
w=-1+\frac{2}{3p}=-1+\frac{c^2}{24\pi}.
$$

If the [reduced Planck mass](../../../../../reduced-planck-mass.md) $M=m_P/\sqrt{8\pi}$ is used instead, the dimensionless exponential slope is $\lambda=c/\sqrt{8\pi}$ and the exponent becomes $p=2/\lambda^2$; these are the same solution.

For $p>1$, the [comoving Hubble radius](../../../../../comoving-hubble-radius.md) decreases as $(aH)^{-1}\propto t^{1-p}$. A region initially in causal contact can grow beyond that radius before the hot [radiation-dominated universe](../../../../../radiation-dominated-universe.md) begins. In the ideal power law extrapolated all the way to $t=0$, the [particle horizon](../../../../../particle-horizon.md) integral $\int_0^t dt'/a(t')$ diverges, so the solution has no finite past particle horizon. A finite, physically trustworthy inflationary interval instead requires a sufficiently large [number of e-folds](../../../../../number-of-e-folds.md) to enlarge an initially causal patch.

For a small curvature contribution, the [Friedmann equation](../../../../../friedmann-equations.md) gives $|\Omega-1|=|k|/(a^2H^2)\propto t^{2-2p}\to0$, solving the [flatness problem](../../../../../flatness-problem.md). Conserved nonrelativistic [magnetic monopoles](../../../../../magnetic-monopole.md) have [number density](../../../../../number-density.md) proportional to $a^{-3}$, while the inflaton [energy density](../../../../../energy-density.md) is proportional to $t^{-2}$; their energy-density ratio therefore falls as $t^{2-3p}$. This gives the required dilution, provided later [reheating](../../../../../reheating.md) does not recreate them. [Inflationary shear damping](../../../../../inflationary-shear-damping.md) similarly suppresses anisotropic expansion.

The main failure is **no automatic graceful exit or reheating**. The [first Hubble slow-roll parameter](../../../../../first-hubble-slow-roll-parameter.md) never reaches one, and the exponential [inflaton potential](../../../../../inflaton-potential.md) has no finite minimum about which the field can oscillate. Additional dynamics are needed for a [graceful exit from inflation](../../../../../graceful-exit-from-inflation.md) and transfer to a hot [radiation-dominated universe](../../../../../radiation-dominated-universe.md). The ideal solution also retains a curvature singularity at $t=0$; solving the [horizon problem](../../../../../horizon-problem.md) does not itself explain the beginning of the universe. For $c=0$, the constant [inflaton potential](../../../../../inflaton-potential.md) instead permits constant-field [de Sitter spacetime](../../../../../de-sitter-spacetime.md) expansion; the logarithmic field solution is inapplicable.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
