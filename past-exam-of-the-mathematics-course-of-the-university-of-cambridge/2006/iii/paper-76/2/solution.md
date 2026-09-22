<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take any fixed material subvolume $B_0$ of the [reference configuration](../../../../../reference-configuration.md), with outward [normal vector](../../../../../normal-vector.md) $N$, current particle [velocity](../../../../../velocity.md) $v_i=\dot x_i$, and positive [temperature](../../../../../temperature.md) $\theta$. The [first law of thermodynamics](../../../../../first-law-of-thermodynamics.md), including [kinetic energy](../../../../../kinetic-energy.md), is

$$
\frac{d}{dt}\int_{B_0}\rho_0\left(u+\tfrac12v_iv_i\right)dX=\int_{B_0}\rho_0(r+g_iv_i)dX+\int_{\partial B_0}(N_IP_{Ii}v_i-N_Iq_I^0)\,dA_0.
$$

The heat-flux sign is negative because $N_Iq_I^0$ is outward. The [Second law of thermodynamics](../../../../../second-law-of-thermodynamics.md) supplies the corresponding integral [Lagrangian entropy inequality](../../../../../lagrangian-entropy-inequality.md):

$$
\frac{d}{dt}\int_{B_0}\rho_0\eta\,dX\geq\int_{B_0}\frac{\rho_0r}{\theta}\,dX-\int_{\partial B_0}\frac{N_Iq_I^0}{\theta}\,dA_0.
$$

The temperature in each supply or flux term is the local temperature, not a common temperature pulled outside the integrals.

Apply the [divergence theorem](../../../../../divergence-theorem.md) and use the reference [momentum conservation](../../../../../momentum-conservation.md) equation $\rho_0\dot v_i=P_{Ii,I}+\rho_0g_i$. In the total-energy equation, the kinetic derivative cancels the body-force work and the $v_iP_{Ii,I}$ term. Since $v_{i,I}=\dot F_{iI}$, the remaining local [Lagrangian internal energy balance](../../../../../lagrangian-internal-energy-balance.md) and [Lagrangian entropy inequality](../../../../../lagrangian-entropy-inequality.md) are

$$
\boxed{\rho_0\dot u=\rho_0r-q_{I,I}^0+P_{Ii}\dot F_{iI}},\qquad
\boxed{\rho_0\dot\eta\geq\frac{\rho_0r}{\theta}-\left(\frac{q_I^0}{\theta}\right)_{,I}}.
$$

They hold pointwise because $B_0$ was arbitrary. In particular,

$$
\rho_0\theta\dot\eta\geq\rho_0r-q_{I,I}^0+\frac{q_I^0\theta_{,I}}{\theta}.
$$

The specific [Helmholtz free energy](../../../../../helmholtz-free-energy.md) is $\psi=u-\theta\eta$. Substitution yields its balance

$$
\rho_0(\dot\psi+\eta\dot\theta+\theta\dot\eta)=\rho_0r-q_{I,I}^0+P_{Ii}\dot F_{iI},
$$

and elimination of the heat supply yields the [Clausius-Duhem inequality](../../../../../clausius-duhem-inequality.md)

$$
P_{Ii}\dot F_{iI}-\rho_0(\dot\psi+\eta\dot\theta)-\frac{q_I^0\theta_{,I}}{\theta}\geq0.
$$

For $\psi=\psi(F,\theta,\xi_r)$, expand the derivative to obtain

$$
(P_{Ii}-\rho_0\psi_{,F_{iI}})\dot F_{iI}-\rho_0(\psi_{,\theta}+\eta)\dot\theta+\rho_0f_r\dot\xi_r-\frac{q_I^0\theta_{,I}}\theta\geq0,\qquad f_r=-\psi_{,\xi_r}.
$$

The usual [Coleman-Noll procedure](../../../../../coleman-noll-procedure.md) admits independent reversible choices of $\dot F$ and $\dot\theta$ at a fixed state. Their coefficients must vanish, since either sign and arbitrary magnitude would otherwise violate the inequality. Thus

$$
\boxed{P_{Ii}=\rho_0\psi_{,F_{iI}},\qquad\eta=-\psi_{,\theta}},\qquad
\boxed{\rho_0f_r\dot\xi_r-\frac{q_I^0\theta_{,I}}\theta\geq0}.
$$

Internal-variable evolution and heat conduction must satisfy this remaining inequality. Substituting the constitutive relations back into the energy balance gives

$$
\boxed{\rho_0\theta\dot\eta=\rho_0r-q_{I,I}^0+\rho_0f_r\dot\xi_r}.
$$

**The last printed equation is missing a factor $\rho_0$ on its internal-variable term.** The PDF defines $f_r=-\psi_{,\xi_r}$ with $\psi$ per unit mass, so the expression above is the dimensionally consistent consequence. Equivalently define the volumetric [thermodynamic force conjugate to an internal variable](../../../../../thermodynamic-force-conjugate-to-an-internal-variable.md) $\widehat f_r=-\rho_0\psi_{,\xi_r}$; the term is then $\widehat f_r\dot\xi_r$ with no extra density. The two conventions must not be mixed.

For [thermoelasticity with a temperature-dependent constraint](../../../../../thermoelasticity-with-a-temperature-dependent-constraint.md), admissible rates obey

$$
\phi_{,F_{iI}}\dot F_{iI}=h'(\theta)\dot\theta.
$$

The reversible coefficient functional need now vanish only on this tangent hyperplane. Hence it can be a scalar multiple $q$ of the constraint normal:

$$
P_{Ii}-\rho_0\psi_{,F_{iI}}=q\phi_{,F_{iI}},\qquad -\rho_0(\psi_{,\theta}+\eta)=-qh'(\theta).
$$

Therefore

$$
\boxed{P_{Ii}=\rho_0\psi_{,F_{iI}}+q\phi_{,F_{iI}},\qquad\eta=-\psi_{,\theta}+\frac{q}{\rho_0}h'(\theta)}.
$$

The reaction terms cancel on admissible rates, leaving the same internal-variable/conduction inequality and entropy heating equation. The multiplier $q$ is determined by equilibrium and boundary conditions rather than by the free energy alone.

For [linear thermoelasticity with prescribed thermal volume](../../../../../linear-thermoelasticity-with-prescribed-thermal-volume.md), write $F=I+H$, $H_{ij}=u_{i,j}$, and $\vartheta=\theta-\theta_0$. Hold the [internal variables](../../../../../internal-variable.md) fixed in this reversible linearization, and evaluate all derivatives below at $(I,\theta_0)$ and zero reaction. The stress-free reference state has $\psi_{,F}=0$. Since $\partial\det F/\partial F=I$ there, first-order nominal and [Cauchy stress tensors](../../../../../cauchy-stress-tensor.md) agree. Their constitutive laws become

$$
\boxed{\sigma_{ji}=C_{jilk}u_{k,l}+\beta_{ji}\vartheta+q\delta_{ji}},\qquad
\boxed{\rho_0(\eta-\eta_0)=C_e\vartheta-\beta_{ji}u_{i,j}+qh'(\theta_0)},
$$

where equality of mixed free-energy derivatives gives

$$
\boxed{C_{jilk}=\rho_0\psi_{,F_{ij}F_{kl}},\qquad\beta_{ji}=\rho_0\psi_{,F_{ij}\theta},\qquad C_e=-\rho_0\psi_{,\theta\theta}}.
$$

The linearized constraint is $u_{i,i}=h'(\theta_0)\vartheta$. Thus volume is thermally prescribed; strict temperature-independent [incompressibility](../../../../../incompressible-flow.md) corresponds to $h'=0$. The coefficient $C_e$ is an entropy slope; the corresponding volumetric [heat capacity](../../../../../heat-capacity.md) at fixed deformation is $\theta_0C_e$.

Together with $\rho_0\ddot u_i=\sigma_{ji,j}+\rho_0g_i$, the first-order thermal balance is $\theta_0(C_e\dot\vartheta-\beta_{ji}\dot u_{i,j}+h'(\theta_0)\dot q)=\rho_0r-q_{I,I}^0$. A heat-flux constitutive law completes the evolution problem. The paired signs of the coupling tensor follow from the same free energy, rather than from separately postulated mechanical and thermal equations.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
