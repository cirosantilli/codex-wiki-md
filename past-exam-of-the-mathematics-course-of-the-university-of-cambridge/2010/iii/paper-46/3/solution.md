<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use $\hbar=c=1$ and normalize the interaction of [quartic scalar field theory](../../../../../quartic-interaction.md) as $\lambda\phi^4/4!$. For a renormalized $n$-point [connected correlation function](../../../../../connected-correlation-function.md), adopt $\phi_B=Z_\phi^{1/2}\phi_R$ and $\gamma_\phi=\tfrac12\mu\,d\log Z_\phi/d\mu$. Independence of bare quantities from the [renormalization scale](../../../../../renormalization-scale.md) gives the [Callan-Symanzik equation](../../../../../callan-symanzik-equation.md)

$$
\left[\mu\partial_\mu+\beta(\lambda)\partial_\lambda+\gamma_{m^2}(\lambda)m^2\partial_{m^2}+n\gamma_\phi(\lambda)\right]G_R^{(n)}=0,
$$

where $\beta=\mu\,d\lambda/d\mu$ and $\gamma_{m^2}=\mu\,d\log m^2/d\mu$, with bare parameters fixed. A convention using proper vertices reverses the field-normalization term, so the choice of Green's function must be stated.

Solve it by characteristics: set $\mu(s)=\mu_0e^s$, $d\lambda(s)/ds=\beta(\lambda(s))$, and $d\log m^2(s)/ds=\gamma_{m^2}(\lambda(s))$. At fixed external momenta,

$$
G_R^{(n)}(\mu(s),\lambda(s),m^2(s))=G_R^{(n)}(\mu_0,\lambda_0,m_0^2)\exp\left[-n\int_0^s\gamma_\phi(\lambda(v))\,dv\right].
$$

This is the [characteristic solution of the multiplicative Callan-Symanzik equation](../../../../../characteristic-solution-of-the-multiplicative-callan-symanzik-equation.md). If the field anomalous dimension vanishes, the function is constant along the running-parameter characteristics. At a massless fixed point with constant anomalous dimension, the normalization factor is a power of $\mu/\mu_0$. Choosing the scale close to a characteristic external momentum avoids large perturbative logarithms.

For the supplied [minimal subtraction scheme](../../../../../minimal-subtraction-scheme.md) relation in [dimensional regularization](../../../../../dimensional-regularization.md) with $d=4-\epsilon$, let $a=3/(16\pi^2)$ and write $\lambda_B=\mu^\epsilon[\lambda+a\lambda^2/\epsilon+O(\lambda^3)]$. Differentiating at fixed bare coupling gives

$$
0=\epsilon\left(\lambda+\frac{a\lambda^2}{\epsilon}\right)+\beta(\lambda)\left(1+\frac{2a\lambda}{\epsilon}\right)+O(\lambda^3).
$$

A consistent expansion yields $\beta=-\epsilon\lambda+a\lambda^2+O(\lambda^3)$. The $-\epsilon\lambda$ term must be retained while it multiplies the pole; setting $\epsilon=0$ prematurely loses the finite result. In four dimensions the [one-loop quartic scalar beta function](../../../../../one-loop-quartic-scalar-beta-function.md) is

$$
\boxed{\beta(\lambda)=\frac{3\lambda^2}{16\pi^2}+O(\lambda^3).}
$$

The one-loop two-point diagram is a momentum-independent [tadpole diagram](../../../../../tadpole-diagram.md), so there is no field wavefunction renormalization at this order and $\gamma_\phi=O(\lambda^2)$. Differentiating the supplied bare-mass relation in the same way gives $\gamma_{m^2}=\lambda/(16\pi^2)+O(\lambda^2)$.

Integrating $d\lambda/d\log\mu=a\lambda^2$ gives the [running coupling](../../../../../running-coupling.md)

$$
\boxed{\lambda(\mu)=\frac{\lambda(\mu_0)}{1-\dfrac{3\lambda(\mu_0)}{16\pi^2}\log(\mu/\mu_0)}.}
$$

For positive coupling it grows toward the ultraviolet and decreases toward the infrared: the theory is not asymptotically free. Its one-loop [Landau pole](../../../../../landau-pole.md) lies at $\mu_L=\mu_0\exp[16\pi^2/(3\lambda(\mu_0))]$. Perturbation theory fails before reaching that pole, so the pole in this approximation alone does not prove the existence of an exact physical divergence. The corresponding one-loop [running mass](../../../../../running-mass.md) satisfies

$$
\boxed{m^2(\mu)=m^2(\mu_0)\left[\frac{\lambda(\mu)}{\lambda(\mu_0)}\right]^{1/3}.}
$$

It follows from $d\log m^2/d\lambda=1/(3\lambda)$. The mass-independent subtraction scheme keeps these beta functions independent of the mass; physical low-energy matching can still require threshold treatment. Running parameters resum the leading logarithms within the regime of small coupling.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
