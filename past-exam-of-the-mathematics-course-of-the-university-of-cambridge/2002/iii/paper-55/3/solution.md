<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Measure $z$ upwards from the inlet and let $L$ now denote the specific [latent heat](../../../../../latent-heat.md) of [melting](../../../../../melting.md) of the crust. Use the standard approximation of equal solid and [magma](../../../../../magma.md) densities, negligible axial conduction, negligible heat loss beyond the [melting](../../../../../melting.md) walls, and a horizontally well-mixed turbulent flow. The wall is at $T_m$, so newly added wall melt enters with zero excess [temperature](../../../../../temperature.md) $\theta=T-T_m$.

For a slice of [dike](../../../../../dike.md), total [magma](../../../../../magma.md) mass per unit height and out-of-plane length is $\rho b$. Both [melting](../../../../../melting.md) walls add mass at rate $\rho b_t$. Consequently [mass conservation](../../../../../mass-conservation.md) gives

$$
\rho b_t+(\rho bw)_z=\rho b_t,
\qquad\boxed{bw=Q_0.}
$$

The growth of channel storage and mass supplied by [melting](../../../../../melting.md) cancel; omitting the right-hand source would incorrectly force the inlet flux to fill this volume without accounting for the newly melted rock. Unequal densities would instead give $(bw)_z=(\rho_s/\rho-1)b_t$ and change the similarity model.

Let $q_w=\alpha_T\rho c_pw\theta$ be [heat transfer](../../../../../heat-transfer.md) to each wall. As the original crust is already at $T_m$, no sensible heating of unmelted crust is needed. Each wall moves outwards at speed $b_t/2$, so its [Stefan condition](../../../../../stefan-condition.md) is

$$
\rho L\frac{b_t}{2}=q_w,
\qquad\boxed{b_t=\frac{2\alpha_Tc_p}L\,w\theta.}
$$

Excess sensible-heat conservation, including both walls, is

$$
\boxed{\partial_t(b\theta)+\partial_z(bw\theta)
=-2\alpha_Tw\theta.}
$$

Combining these equations, with $H=L/c_p$, gives

$$
\boxed{bT_t+Q_0T_z=-[H+(T-T_m)]b_t.}
$$

The term $(T-T_m)b_t$ is the heat used to warm freshly melted wall material. It cannot simply be dropped from a conservative balance. This is [melt-dilution heat balance in a dike](../../../../../melt-dilution-heat-balance-in-a-dike.md).

At the inlet $bw=Q_0$ and $\theta=\Delta_0=T_0-T_m$. The wall balance there gives $b(0,t)^2=b_0^2+4\alpha_TQ_0t/S$, where $S=L/(c_p\Delta_0)$. At late times neglect $b_0$ in the widened basal region and set

$$
B(t)=\left(\frac{4\alpha_TQ_0t}{S}\right)^{1/2},\quad
\eta=\frac{2\alpha_Tz}{B(t)},\quad
b=B(t)f(\eta),\quad\theta=\Delta_0\vartheta(\eta),\quad
w=\frac{Q_0}{B(t)f(\eta)}.
$$

The basal width and the vertical scale both grow as $\sqrt t$. Substituting into the wall condition gives

$$
\boxed{f(f-\eta f')=\vartheta.}
$$

Conservative heat balance first gives $f\vartheta-\eta(f\vartheta)'+S\vartheta'=-S\vartheta/f$. Eliminating $f-\eta f'$ with the wall equation yields

$$
\boxed{(S-\eta f)\vartheta'=-(S+\vartheta)\frac{\vartheta}{f}.}
$$

The [boundary conditions](../../../../../boundary-condition.md) are $f(0)=1$, $\vartheta(0)=1$, with $f\to0$ in the outer idealized limit; the physical cooled branch also has $\vartheta\to0$. These equations and time-independent boundary data establish the [thermal dike-widening similarity](../../../../../thermal-dike-widening-similarity.md). The condition at infinity is an approximation for matching away from the widened basal region, not a claim that the original finite-width [dike](../../../../../dike.md) literally has zero width.

The inlet is a regular singular point of the first equation. Differentiating it and evaluating the second gives

$$
f'(0)=\vartheta'(0)=-\frac{S+1}{S}.
$$

A regular expansion can still contain an undetermined higher-order coefficient, for example in $f''(0)$; the outer matching condition selects it. Thus specifying the inlet values does not eliminate the boundary-value aspect of the problem. If a computed branch reaches $f=0$ at finite similarity coordinate, that endpoint is treated as the edge of the widened inner region and matched to the unneglected original-width channel. One must not continue $w=Q_0/(Bf)$ through zero width as a physical flow.

For numerical solution, formulate this as a nonlinear two-point boundary-value problem: start from a regular inlet expansion and adjust its free coefficient to meet the outer decay/matching condition, or solve for the profiles and boundary data together on a truncated or compactified similarity interval. Enforce nonnegative width and [temperature](../../../../../temperature.md) excess, check any apparent singularity at $S=\eta f$, and refine the outer matching location until the basal profiles are insensitive to it. No specific algorithm is required.

A useful conservation check follows by adding the latent storage to the sensible storage:

$$
\partial_t\{b(H+\theta)\}+Q_0\theta_z=0.
$$

For a vanishing outer excess-heat flux, integration of the similarity profile gives

$$
\boxed{\int f(\eta)[S+\vartheta(\eta)]\,d\eta=\frac S2,}
$$

where the integral runs over its active widened region. This checks the heat admitted at the base against latent and sensible storage. All factors of two refer to the two channel walls; $b$ is the full width.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
