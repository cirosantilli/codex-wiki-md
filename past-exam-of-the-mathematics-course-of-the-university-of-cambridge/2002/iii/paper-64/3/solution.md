<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [correlation length](../../../../../correlation-length.md) is the distance over which fluctuations remain appreciably correlated. More precisely, in a massive phase the large-distance [connected correlation function](../../../../../connected-correlation-function.md)

$$
G_c(x)=\langle\phi(x)\phi(0)\rangle-\langle\phi\rangle^2
$$

has an exponential factor $e^{-|x|/\xi}$, possibly multiplied by a power. Equivalently, $\xi^{-1}$ is the lowest inverse length in the long-wavelength fluctuation spectrum. In the [Gaussian field theory](../../../../../gaussian-field-theory.md) with unit gradient coefficient, $\widetilde G_c(q)\propto(q^2+m_R^2)^{-1}$ gives $\xi=1/m_R$ for positive renormalized mass.

At an ordinary [continuous phase transition](../../../../../continuous-phase-transition.md), the restoring force for long-wavelength order-parameter fluctuations vanishes and there is no finite correlation scale. The critical [connected correlation function](../../../../../connected-correlation-function.md) decays as a power rather than exponentially, so $\xi$ diverges. The [correlation-function susceptibility sum rule](../../../../../correlation-function-susceptibility-sum-rule.md) relates [magnetic susceptibility](../../../../../magnetic-susceptibility.md) to the integral of this [connected correlation function](../../../../../connected-correlation-function.md); its divergence is consistent with correlations extending over increasingly large distances. Interactions change the powers, so the renormalized mass and the bare mass need not vanish at the same temperature.

Absorb the thermal normalization into the action and set

$$
r=u^2=\frac{m^2(\Lambda,T)}{\Lambda^2},\qquad
\lambda=g(\Lambda,T)\Lambda^{-\epsilon},\qquad
d=4-\epsilon,\qquad
K_d=\frac{\Omega_d}{(2\pi)^d}.
$$

Here $r$, although denoted $u^2$ in the question, is a signed mass-squared coordinate, not a nonnegative square. This matters because its interacting fixed-point value is negative. Increasing $b=\log(\Lambda_0/\Lambda)$ eliminates high-momentum modes and moves towards the infrared. The initial values at $b=0$ are $r_0=m^2(\Lambda_0,T)/\Lambda_0^2$ and $\lambda_0=g(\Lambda_0,T)\Lambda_0^{-\epsilon}$.

To derive the flow, use the [momentum-shell decomposition of a scalar field](../../../../../momentum-shell-decomposition-of-a-scalar-field.md) $\phi=\varphi+\chi$, where $\chi$ has momenta $\Lambda e^{-db}<|q|<\Lambda$. Its [Gaussian shell covariance](../../../../../gaussian-shell-covariance.md) is $(q^2+m^2)^{-1}$. Integrating out $\chi$ while preserving low-momentum observables gives

$$
S_{\mathrm{eff}}[\varphi]=S_0[\varphi]
-\log\left\langle e^{-V[\varphi+\chi]}\right\rangle_>,
\qquad V=\frac g{4!}\int d^dx\,(\varphi+\chi)^4.
$$

The [cumulant expansion of a coarse-grained free energy](../../../../../cumulant-expansion-of-a-coarse-grained-free-energy.md) yields $\langle V\rangle_>-\frac12\langle V^2\rangle_{>,c}+\cdots$. By [Wick theorem](../../../../../wick-s-theorem.md),

$$
\langle V\rangle_>=\frac g{24}\int d^dx\,
\left[\varphi^4+6\varphi^2G_>(0)+3G_>(0)^2\right].
$$

The last term is field independent, while the quadratic term gives the [one-loop shell mass renormalization in scalar quartic theory](../../../../../one-loop-shell-mass-renormalization-in-scalar-quartic-theory.md)

$$
\delta m^2=\frac g2 I_1,\qquad
I_1=\int_{\mathrm{shell}}\frac{d^dq}{(2\pi)^d}
\frac1{q^2+m^2}.
$$

This tadpole is independent of the external momentum, so no gradient renormalization occurs at this order.

For the quartic correction, the mixed vertex is $(g/4)\int\varphi^2\chi^2$. Its connected second cumulant uses $\langle\chi^2(x)\chi^2(y)\rangle_c=2G_>(x-y)^2$ and gives

$$
-\frac{g^2}{16}\int d^dx\,d^dy\,
\varphi^2(x)\varphi^2(y)G_>(x-y)^2.
$$

Extracting the local zero-external-momentum quartic interaction, the integral over $x-y$ is $I_2=\int_{\mathrm{shell}}d^dq\,(2\pi)^{-d}(q^2+m^2)^{-2}$. Comparing its coefficient with $g\varphi^4/4!$ gives the [one-loop shell quartic renormalization](../../../../../one-loop-shell-quartic-renormalization.md)

$$
\delta g=-\frac32g^2I_2.
$$

The negative sign comes from the second cumulant; the numerical factor incorporates the three quartic channels.

For the thin spherical shell, radial integration gives

$$
I_1=K_d\frac{\Lambda^{d-2}}{1+r}\,db+O(db^2),
\qquad
I_2=K_d\frac{\Lambda^{d-4}}{(1+r)^2}\,db+O(db^2).
$$

The shell is stable when $1+r>0$, including a small negative critical mass. Because $d\Lambda/db=-\Lambda$, differentiating the dimensionless couplings contributes their [engineering dimensions](../../../../../engineering-dimension.md) $2$ and $\epsilon$. Together with the shell corrections this yields the [renormalization-group flow](../../../../../renormalization-group-flow.md)

$$
\boxed{\frac{dr}{db}=2r+\frac{K_d}{2}\frac{\lambda}{1+r},
\qquad
\frac{d\lambda}{db}=\epsilon\lambda-
\frac{3K_d}{2}\frac{\lambda^2}{(1+r)^2}.}
$$

These are the requested equations with $r=u^2$. They express independence of the long-distance theory from the arbitrarily chosen [ultraviolet cutoff](../../../../../ultraviolet-cutoff.md), to the retained perturbative order; higher interactions and gradient corrections enter at higher orders.

Besides the [Gaussian fixed point](../../../../../gaussian-fixed-point.md) $(r,\lambda)=(0,0)$, a nonzero fixed point satisfies

$$
\lambda_*=\frac{2\epsilon}{3K_d}(1+r_*)^2,\qquad
0=2r_*+\frac{\epsilon}{3}(1+r_*).
$$

Thus, within these truncated equations,

$$
r_*=-\frac{\epsilon}{6+\epsilon},\qquad
\lambda_*=\frac{2\epsilon}{3K_d}
\left(\frac6{6+\epsilon}\right)^2.
$$

Since $\Omega_4=2\pi^2$ and $K_4=1/(8\pi^2)$, their leading [epsilon expansion](../../../../../epsilon-expansion.md) is

$$
\boxed{r_*=-\frac{\epsilon}{6}+O(\epsilon^2),\qquad
\lambda_*=\frac{16\pi^2\epsilon}{3}+O(\epsilon^2).}
$$

The rational expressions from the truncated flow are not a calculation of the genuine higher-order coefficients.

To assess stability, linearize in $\delta r,\delta\lambda$ about this [Wilson-Fisher fixed point](../../../../../wilson-fisher-fixed-point.md). The [stability matrix of a renormalization-group fixed point](../../../../../stability-matrix-of-a-renormalization-group-fixed-point.md) is

$$
\mathsf M=
\begin{pmatrix}
2-\dfrac{K_d\lambda_*}{2(1+r_*)^2}
&\dfrac{K_d}{2(1+r_*)}\\
\dfrac{3K_d\lambda_*^2}{(1+r_*)^3}
&\epsilon-\dfrac{3K_d\lambda_*}{(1+r_*)^2}
\end{pmatrix}.
$$

Using the fixed-point equation, its diagonal entries are $2-\epsilon/3$ and $-\epsilon$, respectively. Its upper off-diagonal entry is $1/(16\pi^2)+O(\epsilon)$ and its lower off-diagonal entry is $O(\epsilon^2)$. Hence its [eigenvalues](../../../../../eigenvalue.md) are

$$
y_t=2-\frac{\epsilon}{3}+O(\epsilon^2),\qquad
y_{\mathrm{irr}}=-\epsilon+O(\epsilon^2).
$$

The interaction perturbation along the [critical surface](../../../../../critical-surface.md) decays towards the infrared for small positive $\epsilon$, whereas the thermal perturbation grows. Therefore **infrared attraction requires tuning to the critical surface**. The source's unqualified wording cannot mean attraction in both coupling directions: the positive thermal eigenvalue is precisely what produces the divergence of the [correlation length](../../../../../correlation-length.md). This is the [thermal relevant direction at the Wilson-Fisher fixed point](../../../../../thermal-relevant-direction-at-the-wilson-fisher-fixed-point.md).

Let $\tau$ be the thermal scaling coordinate, a linear combination of $\delta r$ and $\delta\lambda$ corresponding to the relevant left [eigenvector](../../../../../eigenvector.md) of $\mathsf M$. To leading order, $\tau=\delta r+[1/(32\pi^2)+O(\epsilon)]\delta\lambda$ is possible. Its initial value is proportional to $T-T_c$ for a generic thermal path crossing the [critical surface](../../../../../critical-surface.md); the interaction also shifts the nonuniversal value of $T_c$. In the linear regime,

$$
\tau(b)\simeq e^{y_tb}\tau(0).
$$

Choose $b_*$ so that $|\tau(b_*)|$ is of order one. At this scale the dimensionless [correlation length](../../../../../correlation-length.md) is finite. Restoring the eliminated length scale gives

$$
\xi\asymp\Lambda_0^{-1}e^{b_*}
\asymp|\tau(0)|^{-1/y_t}
\asymp|T-T_c|^{-\nu}.
$$

Consequently the [correlation-length critical exponent](../../../../../correlation-length-critical-exponent.md) is

$$
\boxed{\nu=\frac1{2-\epsilon/3+O(\epsilon^2)}
=\frac12+\frac{\epsilon}{12}+O(\epsilon^2).}
$$

There is no field anomalous dimension at one loop in this scalar quartic theory, since the one-loop self-energy is momentum independent; this is consistent with $\eta=O(\epsilon^2)$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
