<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $v_i=\dot x_i$ and use a fixed arbitrary material subvolume $B_0$ in the [reference configuration](../../../../../reference-configuration.md), with outward unit normal $N_I$. The reference mass density $\rho_0$ is time independent. The global [momentum conservation](../../../../../momentum-conservation.md) law is

$$
\frac d{dt}\int_{B_0}\rho_0v_i\,dX
=\int_{\partial B_0}P_{Ii}N_I\,dS+\int_{B_0}\rho_0g_i\,dX.
$$

The [divergence theorem](../../../../../divergence-theorem.md), differentiation under the integral, and arbitrariness of $B_0$ give

$$
\boxed{\rho_0\dot v_i=P_{Ii,I}+\rho_0g_i.}
$$

The global [conservation of energy](../../../../../conservation-of-energy.md) law includes both [internal energy](../../../../../internal-energy.md) and [kinetic energy](../../../../../kinetic-energy.md):

$$
\frac d{dt}\int_{B_0}\rho_0\left(u+\frac12v_iv_i\right)dX
=\int_{\partial B_0}(P_{Ii}v_i-q_I^0)N_I\,dS
+\int_{B_0}\rho_0(g_iv_i+r)\,dX.
$$

Here $q^0$ is outgoing [heat flux](../../../../../heat-flux-density.md) per reference area. Localizing gives

$$
\rho_0\dot u+\rho_0v_i\dot v_i
=P_{Ii,I}v_i+P_{Ii}v_{i,I}-q_{I,I}^0
+\rho_0g_iv_i+\rho_0r.
$$

Subtract the scalar product of the local [momentum conservation](../../../../../momentum-conservation.md) law with $v$. Since $v_{i,I}=\dot F_{iI}$, this proves the [Lagrangian internal energy balance](../../../../../lagrangian-internal-energy-balance.md)

$$
\boxed{\rho_0\dot u=P_{Ii}\dot F_{iI}+\rho_0r-q_{I,I}^0.}
$$

For positive [temperature](../../../../../temperature.md) $\theta$, the global [entropy](../../../../../entropy.md) inequality is

$$
\frac d{dt}\int_{B_0}\rho_0\eta\,dX
\geq\int_{B_0}\frac{\rho_0r}{\theta}\,dX
-\int_{\partial B_0}\frac{q_I^0N_I}{\theta}\,dS.
$$

Its local excess is a nonnegative production density $\gamma$. Expanding the divergence of $q^0/\theta$ proves the [Lagrangian entropy inequality](../../../../../lagrangian-entropy-inequality.md) in the requested equality form:

$$
\boxed{\rho_0\dot\eta
=\frac{\rho_0r-q_{I,I}^0}{\theta}
+\frac{\theta_{,I}q_I^0}{\theta^2}+\gamma,
\qquad\gamma\geq0.}
$$

No constitutive assumption on the [heat flux](../../../../../heat-flux-density.md) was needed for these balance identities.

For the [reference-configuration jump balances](../../../../../reference-configuration-jump-balances.md), make the orientation convention explicit. Write $[a]=a^+-a^-$ and let $n^0$ point from the minus side to the plus side. Let $c$ be the actual interface speed in direction $n^0$. A signed level function $\phi$ with the plus side $\phi>0$ obeys $\phi_t=-c|\nabla_X\phi|$ on the interface. For $a=a^-+[a]H(\phi)$, the singular time derivative is $-c[a]\delta_S$; the singular reference divergence of $b$ is $n_I^0[b_I]\delta_S$. Thus a local conservation law $a_t=\operatorname{Div}b+$ bounded sources has the [Rankine-Hugoniot condition](../../../../../rankine-hugoniot-conditions.md)

$$
-c[a]=n_I^0[b_I].
$$

This is also the shrinking moving-pillbox calculation of the global law: finite volume supplies have no surviving surface term.

To match the displayed positive-sign momentum jump in the paper, use its speed parameter as $V=-c$, so the interface travels in direction $-Vn^0$. Assuming continuous $\rho_0$ and no surface force or energy supply, the jump laws are then

$$
\boxed{\rho_0V[v_i]=n_I^0[P_{Ii}],}
$$



$$
\boxed{\rho_0V\left[u+\frac12v_iv_i\right]
=n_I^0[P_{Ii}v_i-q_I^0],}
$$

and, from $\partial_t(\rho_0\eta)+\operatorname{Div}(q^0/\theta)\geq\rho_0r/\theta$,

$$
\boxed{\rho_0V[\eta]+n_I^0[q_I^0/\theta]\geq0.}
$$

The last inequality is nonnegative entropy production concentrated on the interface. Temperature and flux in the entropy term are the traces on their respective sides; one cannot take a common temperature outside the jump unless it is continuous.

If $V$ is instead defined as the interface speed in direction $n^0$, all three $V$ terms above acquire a minus sign. In particular the printed positive-sign momentum formula requires the opposite speed convention; changing just the order of the jump does not remove this convention issue. If reference density is discontinuous, replace $\rho_0[a]$ by the jump $[\rho_0a]$ of the complete conserved density.

An equivalent internal-energy jump follows by subtracting the kinetic-energy jump using $[|v|^2/2]=\{v_i\}[v_i]$, where $\{a\}=(a^++a^-)/2$:

$$
\rho_0V[u]=n_I^0\{P_{Ii}\}[v_i]-n_I^0[q_I^0].
$$

The averaged traction appears because $[P_{Ii}v_i]=\{P_{Ii}\}[v_i]+[P_{Ii}]\{v_i\}$; using a one-sided traction would generally be incorrect.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
