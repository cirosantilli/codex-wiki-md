<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a homogeneous canonical [inflaton](../../../../../inflaton.md), $\rho_\phi=\dot\phi^2/2+V$ and $P_\phi=\dot\phi^2/2-V$. [Vacuum domination by a scalar field](../../../../../vacuum-domination-by-a-scalar-field.md) requires positive potential energy to dominate both kinetic energy and any competing material components. Then $P_\phi\simeq-\rho_\phi$ and the expansion is nearly vacuum-like. Exact scalar-driven acceleration requires $\rho_\phi+3P_\phi<0$, equivalently $\dot\phi^2<V$; potential domination is a stronger condition.

The [slow-roll approximation](../../../../../slow-roll-approximation.md) additionally neglects $\ddot\phi$ compared with $3H\dot\phi$ in the [inflaton equation of motion](../../../../../inflaton-equation-of-motion.md). Define the unreduced [Planck mass](../../../../../planck-mass.md) $m_{\rm pl}=G^{-1/2}$; it differs from the [reduced Planck mass](../../../../../reduced-planck-mass.md) by $\sqrt{8\pi}$. Sufficient potential-flatness conditions are

$$
\epsilon_V=\frac{m_{\rm pl}^2}{16\pi}\left(\frac{V'}V\right)^2\ll1,\qquad
|\eta_V|=\left|\frac{m_{\rm pl}^2}{8\pi}\frac{V''}V\right|\ll1,
$$

together with approach to the slow-roll attractor. The reduced equations are $H^2\simeq8\pi V/(3m_{\rm pl}^2)$ and $3H\dot\phi\simeq-V'$.

For $V=m^2\phi^2/2$, take $m>0$ and the positive-field rolling branch. Then

$$
H\simeq\sqrt{\frac{4\pi}{3}}\frac{m\phi}{m_{\rm pl}},\qquad
\dot\phi\simeq-\frac{m^2\phi}{3H}=-\frac{mm_{\rm pl}}{2\sqrt{3\pi}}.
$$

The field velocity is constant to this order. Choosing the start at $t=0$ gives the [quadratic-potential slow-roll solution](../../../../../quadratic-potential-slow-roll-solution.md)

$$
\boxed{\phi(t)=\phi_i-\frac{mm_{\rm pl}}{2\sqrt{3\pi}}t.}
$$

The PDF puts $\pi$ inside this square root; the converted TeX incorrectly moves it outside. Next integrate $d\log a/d\phi=H/\dot\phi=-4\pi\phi/m_{\rm pl}^2$:

$$
\boxed{a(t)=a_0\exp\left[\frac{2\pi}{m_{\rm pl}^2}\bigl(\phi_i^2-\phi(t)^2\bigr)\right].}
$$

Thus the [number of e-folds](../../../../../number-of-e-folds.md) is the logarithmic expansion, not the expansion factor itself:

$$
\boxed{N=\log\frac{a_f}{a_i}=\int_{t_i}^{t_f}Hdt=\frac{2\pi}{m_{\rm pl}^2}(\phi_i^2-\phi_f^2).}
$$

Here $\epsilon_V=\eta_V=m_{\rm pl}^2/(4\pi\phi^2)$. The usual [quadratic-inflation endpoint estimate](../../../../../quadratic-inflation-endpoint-estimate.md) sets $\epsilon_V\simeq1$, giving

$$
\boxed{\phi_{\rm end}\simeq\frac{m_{\rm pl}}{\sqrt{4\pi}},\qquad
N_{\rm total}\simeq\frac{2\pi\phi_i^2}{m_{\rm pl}^2}-\frac12.}
$$

This is an endpoint estimate, not an exact result from the full equations. Exact acceleration ends at the [Hubble slow-roll parameter](../../../../../hubble-slow-roll-parameter.md) $\epsilon_H=1$, equivalently $\dot\phi^2=V$. Inserting the slow-roll velocity into that last condition instead gives $\phi\simeq m_{\rm pl}/\sqrt{6\pi}$; the different order-one coefficient illustrates the failing approximation at the endpoint. A precise value requires the full scalar and Friedmann evolution. The large initial-field contribution to $N$ is unaffected by that order-one uncertainty.

Finally $V(\phi_i)\sim m_{\rm pl}^4$ gives $\phi_i^2\sim2m_{\rm pl}^4/m^2$. The [quadratic-inflation expansion from Planck density](../../../../../quadratic-inflation-expansion-from-planck-density.md) is therefore

$$
\boxed{N_{\rm total}\sim4\pi\left(\frac{m_{\rm pl}}m\right)^2,\qquad
\frac{a_{\rm end}}{a_0}\sim\exp\left[4\pi\left(\frac{m_{\rm pl}}m\right)^2\right].}
$$

For $m\ll m_{\rm pl}$ this is enormous and the initial field is in the slow-roll regime. No unique numerical factor follows without specifying $m/m_{\rm pl}$. Extrapolating the classical model from Planck density is only a formal estimate; it does not establish control of quantum-gravity corrections at that starting scale.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
