<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use units $c=1$ and take the initially expanding branch with ordinary positive matter or radiation density. In the [Friedmann-Lemaître-Robertson-Walker metric](../../../../../friedmann-lemaitre-robertson-walker-metric.md), $k=+1,0,-1$ respectively describe positive, zero and negative spatial curvature. Separately conserved [pressureless matter](../../../../../pressureless-matter.md) has $\rho_M\propto a^{-3}$ and [radiation in cosmology](../../../../../radiation-in-cosmology.md) has $\rho_R\propto a^{-4}$, so either dominates the curvature and vacuum terms sufficiently far back on a hot Big Bang branch.

With negligible [cosmological constant](../../../../../cosmological-constant.md), a spatially flat radiation universe has $a\propto t^{1/2}$ and a flat matter universe has $a\propto t^{2/3}$; both expand forever while decelerating. An open universe also expands forever and eventually becomes approximately curvature dominated, with $a\propto t$. A closed universe containing only ordinary matter/radiation reaches a maximum size and recollapses. For example, dust gives $\dot a^2=C/a-k$ with $C>0$, so only $k=+1$ admits the positive turning point $a=C$.

**Curvature alone does not determine the fate when the cosmological constant is retained.** Positive $\Lambda$ can cause late accelerated expansion and prevent even a closed universe from recollapsing; whether a closed expanding branch turns around depends on the relative matter and vacuum terms. Negative $\Lambda$ can cause recollapse even for flat or open spatial sections. These statements follow by inspecting $\dot a^2=C/a-k+\Lambda a^2/3$ for dust; the curvature sign is a geometrical classification, not by itself a universal destiny criterion.

Define the [critical density](../../../../../critical-density.md) $\rho_c=3H^2/(8\pi G)$ and [cosmological density parameters](../../../../../cosmological-density-parameter.md) $\Omega_M=\rho_M/\rho_c$, $\Omega_R=\rho_R/\rho_c$, $\Omega_\Lambda=\Lambda/(3H^2)$ and $\Omega_k=-k/(a^2H^2)$. The [Friedmann equation](../../../../../friedmann-equations.md) gives $\Omega_M+\Omega_R+\Omega_\Lambda+\Omega_k=1$. Dividing the [Friedmann acceleration equation](../../../../../friedmann-acceleration-equation.md) by $-H^2$ gives

$$
q=\frac{4\pi G}{3H^2}(\rho+3P)-\Omega_\Lambda
=\frac12\Omega_M+\Omega_R-\Omega_\Lambda.
$$

Consequently

$$
\boxed{q=\frac12\Omega_M-\Omega_\Lambda\quad\text{for dust plus vacuum},\qquad q=\Omega_R-\Omega_\Lambda\quad\text{for radiation plus vacuum}.}
$$

The [deceleration parameter](../../../../../deceleration-parameter.md) measures the sign and size of the acceleration relative to $aH^2$: $q>0$ means deceleration, $q<0$ accelerated expansion and $q=0$ instantaneously zero acceleration. In particular a falling [Hubble parameter](../../../../../hubble-parameter.md) alone does not imply deceleration, since $q=-1-\dot H/H^2$.

For conformal time $d\eta=dt/a$, the [conformal Hubble parameter](../../../../../conformal-hubble-parameter.md) is $\mathcal H=aH$. Using matter conservation and differentiating $\Omega_M\propto\rho_M/H^2$,

$$
\frac{\dot\Omega_M}{\Omega_M}=-3H-2\frac{\dot H}{H}=H(2q-1),\qquad
\boxed{\Omega_M'=\mathcal H\Omega_M(\Omega_M-1-2\Omega_\Lambda).}
$$

This is the [matter density flow with a cosmological constant](../../../../../matter-density-flow-with-a-cosmological-constant.md). Neglecting $\Omega_\Lambda$ during matter domination reduces it to the requested relation

$$
\boxed{\Omega_M'=\mathcal H\Omega_M(\Omega_M-1).}
$$

That last equation is not exact with nonzero $\Lambda$. For example, a flat dust-plus-vacuum state with $(\Omega_M,\Omega_\Lambda)=(0.9,0.1)$ gives $\Omega_M'/\mathcal H=-0.27$, whereas the matter-only expression gives $-0.09$.

For the [flatness problem](../../../../../flatness-problem.md), let $\Omega_{\rm tot}=\Omega_M+\Omega_R+\Omega_\Lambda$. Curvature satisfies $\Omega_{\rm tot}-1=k/(aH)^2$, so

$$
\frac{d\log|\Omega_{\rm tot}-1|}{d\log a}=2q.
$$

In decelerating near-flat radiation and matter eras, deviations therefore grow as $a^2$ and $a$ respectively. Maintaining small curvature at a late epoch requires very small early deviations unless a prior mechanism suppresses them. [Cosmic inflation](../../../../../cosmic-inflation-split.md), with $q\simeq-1$, drives the deviation down approximately as $a^{-2}$. If vacuum energy is present, flatness means $\Omega_{\rm tot}=1$, not $\Omega_M=1$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
