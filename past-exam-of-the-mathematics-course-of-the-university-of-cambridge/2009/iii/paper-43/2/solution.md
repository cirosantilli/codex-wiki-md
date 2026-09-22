<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take the [connected correlation function](../../../../../connected-correlation-function.md)

$$
G(r)=\langle\sigma_0\sigma_r\rangle-\langle\sigma_0\rangle\langle\sigma_r\rangle.
$$

For a massive phase its large-distance form is an algebraic prefactor times $e^{-|r|/\xi}$, defining the exponential [correlation length](../../../../../correlation-length.md) $\xi$. To specify the normalization of [magnetic susceptibility](../../../../../magnetic-susceptibility.md), add $-h\sum_r\sigma_r$ to the energy and differentiate the mean spin. Translation invariance gives the [correlation-function susceptibility sum rule](../../../../../correlation-function-susceptibility-sum-rule.md)

$$
\boxed{\chi=\frac{\partial M}{\partial h}=\frac{\beta_{\rm th}}N\operatorname{Var}\left(\sum_r\sigma_r\right)=\beta_{\rm th}\sum_rG(r),\qquad \beta_{\rm th}=(k_BT)^{-1}.}
$$

Using the dimensionless source $\beta_{\rm th}h$ removes the prefactor $\beta_{\rm th}$. Below the transition, use a selected pure phase rather than a mixture of the two magnetizations, which would have a macroscopic disconnected fluctuation.

Choose a nonnegative [blocking kernel](../../../../../blocking-kernel.md) $K_b(\sigma',\sigma)$ normalized by $\sum_{\sigma'}K_b(\sigma',\sigma)=1$. It may enforce a block average, a majority rule or a chosen rescaled coarse spin. Define the transformed weight by

$$
e^{-\beta_{\rm th}[H(u',\sigma')+N'C']}=
\sum_\sigma K_b(\sigma',\sigma)e^{-\beta_{\rm th}[H(u,\sigma)+NC]}.
$$

Summing this identity over coarse spins shows exact preservation of the [partition function](../../../../../canonical-partition-function.md). The geometrical changes are **$a'=ba$ and $N'=N/b^D$**. A coordinate rescaling subsequently restores the reference cutoff if desired. The transformation is exact only if all generated operators are retained; a finite-coupling truncation is an approximation.

Define the coupling-independent term generated when $C=0$ by

$$
\sum_\sigma K_b(\sigma',\sigma)e^{-\beta_{\rm th}H(u,\sigma)}
=e^{-\beta_{\rm th}[H(R_bu,\sigma')+N'c(u)]}.
$$

Restoring the original $C$ gives the [identity-operator contribution to renormalization-group free energy](../../../../../identity-operator-contribution-to-renormalization-group-free-energy.md):

$$
\boxed{u_{p+1}=R_b(u_p),\qquad C_{p+1}=b^DC_p+c(u_p).}
$$

The parameter $C_p$ is an accumulated additive energy per coarse site. It multiplies the identity operator and leaves normalized spin probabilities unchanged, but it must be kept when calculating the absolute [free energy](../../../../../thermodynamic-free-energy.md). It records the eliminated-mode entropy and the normalization of their statistical measure.

Use an energy-per-site convention: $F(u,C)=-\log Z(u,C,N)/(\beta_{\rm th}N)$ and $f(u)=F(u,0)$, so $F=f+C$. Partition-function invariance gives

$$
F(u_p,C_p)=b^{-D}F(u_{p+1},C_{p+1}).
$$

Consequently, with $g(u)=b^{-D}c(u)$,

$$
f(u)=b^{-D}f(R_bu)+g(u),\qquad
\boxed{f(u_0)=b^{-pD}f(u_p)+\sum_{j=0}^{p-1}b^{-jD}g(u_j).}
$$

This is the [additive free-energy recursion under blocking](../../../../../additive-free-energy-recursion-under-blocking.md). In a dimensionless free-energy convention multiply $f,C,c,g$ by $\beta_{\rm th}$; the same recursion holds. The inhomogeneous term comes from the generated identity operator, not from a change in the spin-dependent couplings alone.

The affine equation naturally applies to the unsubtracted free energy. To extract its singular part, write $f=f_{\rm reg}+F_s$ and choose a regular background satisfying $f_{\rm reg}(u)=b^{-D}f_{\rm reg}(R_bu)+g(u)$. Subtraction then gives $F_s(u)=b^{-D}F_s(R_bu)$. This [analytic subtraction of an inhomogeneous renormalization recursion](../../../../../analytic-subtraction-of-an-inhomogeneous-renormalization-recursion.md) is justified when the eliminated finite-shell contribution is analytic near the fixed point and admits a regular subtraction. It can fail in a resonant direction, producing additive logarithms. The simple homogeneous formulas also assume the remaining [irrelevant operators](../../../../../irrelevant-operator.md) are not [dangerously irrelevant couplings](../../../../../dangerously-irrelevant-coupling.md), and that [marginal operators](../../../../../marginal-operator.md) do not produce unaccounted logarithmic corrections. Calling the quantity in the affine equation “singular” does not make $g$ vanish automatically.

Near a [renormalization-group fixed point](../../../../../renormalization-group-fixed-point.md) $u_*$, linearize the coupling map. In scaling coordinates $v_i$, write $v_i'=b^{\lambda_i}v_i$ to leading order. Here $b^{\lambda_i}$ is a discrete multiplier, whereas $\lambda_i$ is its logarithmic scaling exponent. A [relevant operator](../../../../../relevant-operator.md) has $\lambda_i>0$ and grows under coarse-graining; an [irrelevant operator](../../../../../irrelevant-operator.md) has $\lambda_i<0$ and decays. A [marginal operator](../../../../../marginal-operator.md) needs nonlinear analysis. Tuning the relevant fields to zero places the system on the [critical surface](../../../../../critical-surface.md). At the fixed point the spin field is rescaled as $\sigma'(x')=b^{\Delta_\sigma}\sigma_<(bx')$ with $\Delta_\sigma=(D-2+\eta)/2$. Its conjugate source therefore has $\lambda_h=D-\Delta_\sigma=(D+2-\eta)/2$. This accounts for both coupling and spin rescaling; the field normalization is part of the transformation, not a change in the physical microscopic spin length.

Assume the thermal field $t=(T-T_c)/T_c$ and magnetic field $h$ are the only remaining relevant directions. The homogeneous [scaling hypothesis for critical phenomena](../../../../../scaling-hypothesis-for-critical-phenomena.md) gives

$$
F_s(t,h)=b^{-pD}F_s(b^{p\lambda_t}t,b^{p\lambda_h}h).
$$

Choose the stopping scale with $b^{p\lambda_t}|t|=1$. Then

$$
\boxed{F_s(t,h)=|t|^{D/\lambda_t}f_\pm\left(h/|t|^{\lambda_h/\lambda_t}\right),}
$$

where **$f_+$ is the branch for $t>0$ and $f_-$ the branch for $t<0$**. Nonuniversal metric factors can be absorbed into the definitions of $t,h$ and these functions. Correlation lengths transform as $\xi(t)=b^p\xi(b^{p\lambda_t}t)$, so $\nu=1/\lambda_t$. Differentiating the singular free energy twice with respect to temperature gives $C_s\propto|t|^{D/\lambda_t-2}$, and hence the [hyperscaling relation](../../../../../hyperscaling-relation.md)

$$
\boxed{\alpha=2-D\nu.}
$$

Two source derivatives similarly give $\gamma=(2\lambda_h-D)/\lambda_t$. A single source derivative gives the ordered-branch exponent $\beta=(D-\lambda_h)/\lambda_t$, and setting $t=0$ and scaling $h$ to one gives $\delta=\lambda_h/(D-\lambda_h)$ when the corresponding magnetization branch exists. These show explicitly how the [critical exponents](../../../../../critical-exponent.md) follow from the fixed-point scaling eigenvalues.

The independent correlation derivation uses $G(r)=A r^{-(D-2+\eta)}f_G(r/\xi)$ with a single crossover scaling function. For lattice spacing $a$, the singular continuum contribution to the [magnetic susceptibility](../../../../../magnetic-susceptibility.md) is

$$
\chi_s\simeq\beta_{\rm th}a^{-D}A S_D\int_a^\infty r^{1-\eta}f_G(r/\xi)\,dr
\sim\beta_{\rm th}a^{-D}A S_D\xi^{2-\eta}\int_0^\infty s^{1-\eta}f_G(s)\,ds.
$$

Here $S_D$ is the area of the unit $(D-1)$-sphere. The final integral is finite and nonzero when $\eta<2$, $f_G(0)$ is finite and nonzero, and the tail decays exponentially. Microscopic distances contribute a regular background. With $\xi\sim|t|^{-\nu}$ this proves the [Fisher scaling relation](../../../../../fisher-scaling-relation.md)

$$
\boxed{\chi_s\propto\xi^{2-\eta},\qquad \gamma=(2-\eta)\nu.}
$$

There is an amplitude qualification in the printed large-distance formula: its tail has the Gaussian shape and, taken literally with amplitude independent of $\xi$, integrates to a term proportional to $\xi^2$. For a nonzero anomalous exponent it must instead be matched to the critical short-distance normalization. The [matching the amplitude of a massive critical correlation tail](../../../../../matching-the-amplitude-of-a-massive-critical-correlation-tail.md) gives

$$
G(r)\sim A_\infty\,\xi^{-\eta}\frac{\xi}{(\xi r)^{(D-1)/2}}e^{-r/\xi},\qquad r\gg\xi.
$$

At $r=s\xi$ this has precisely the same overall $\xi^{-(D-2+\eta)}$ scaling as the critical form. Thus the requested identity uses the full scaling hypothesis, or equivalently this implicit amplitude factor. The printed tail without it is consistent as written in the Gaussian case $\eta=0$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
