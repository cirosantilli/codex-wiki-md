<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let

$$
I=\int_Vr^2\,dm,
\qquad
T=\frac12\int_V|\dot{\mathbf r}|^2\,dm,
$$

be the scalar moment of inertia and total kinetic energy. Since

$$
\frac12\ddot I=2T+\int_V\rho\mathbf r\cdot\ddot{\mathbf r}\,dV,
$$

substitution of the [Euler momentum equation](../../../../../euler-equations-for-an-inviscid-fluid.md) reduces the stress contribution, by the [divergence theorem](../../../../../divergence-theorem.md) and isotropic pressure $\mathbf P=P\mathbf 1$, to

$$
-\int_V\mathbf r\cdot\nabla P\,dV
=3\int_VP\,dV-3P_sV.
$$

For self-gravity, $\int\rho\mathbf r\cdot\mathbf F\,dV=\Omega$, where $\Omega<0$ is the gravitational potential energy. Thus the [stellar virial theorem](../../../../../stellar-virial-theorem.md) is

$$
\boxed{\frac12\ddot I=2T+3\int_VP\,dV-3P_sV+\Omega}.
$$

Apply hydrostatic equilibrium to the isothermal core, taking its boundary pressure to be $P_c$. Its ideal-gas pressure integral scales as $\int P,dV\propto M_cT_c$, its volume as $R_c^3$, and its gravitational energy as $-GM_c^2/R_c$. The virial theorem therefore gives

$$
3P_cV_c=3\int_{
m core}P\,dV+\Omega_c,
$$

or, after absorbing fixed dimensional and structural factors into positive constants,

$$
\boxed{P_c=\lambda\frac{M_cT_c}{R_c^3}-\eta\frac{M_c^2}{R_c^4}},
\qquad \lambda,eta>0.
$$

Hydrogen-burning reactions are extremely temperature-sensitive, so expansion cools and suppresses burning while contraction heats and enhances it. This [stellar thermostat](../../../../../stellar-thermostat.md) keeps the shell and adjoining isothermal core near an approximately fixed $T_c$.

At fixed $M_c,T_c$, differentiating $P_c(R_c)$ gives

$$
\boxed{R_{c,\max}=\frac{4\eta M_c}{3\lambda T_c}},
\qquad
\boxed{P_{c,\max}=\frac{27}{256}
\frac{\lambda^4T_c^4}{\eta^3M_c^2}}.
$$

For a homologous envelope, hydrostatic balance gives $P_c\propto GM^2/R^4$ and the ideal-gas temperature scale gives $T_c\propto GM/R$. Eliminating $R$ yields

$$
\boxed{P_c\propto\frac{T_c^4}{M^2}},
$$

up to composition and gravitational constants common to the sequence. A matching core exists only if this required pressure does not exceed $P_{c,\max}\propto T_c^4/M_c^2$. Therefore

$$
\boxed{M_c<M_{\rm crit}},
\qquad
\boxed{M_{\rm crit}\propto M}.
$$

This maximum fractional isothermal-core mass is the mechanism behind the [Schönberg-Chandrasekhar limit](../../../../../schonberg-chandrasekhar-limit.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
