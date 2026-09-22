<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [inverse temperature](../../../../../../inverse-temperature.md) $\beta_T=(k_BT)^{-1}$, reserving $\beta$ without a subscript for the [critical exponent](../../../../../../critical-exponent.md). Write $c=qJ$; each undirected bond occurs once, so the number of bonds is $Nq/2$. In the [mean-field theory of the Ising model](../../../../../../mean-field-theory-of-the-ising-model.md), write each [Ising spin](../../../../../../ising-spin-variable.md) as $\sigma_i=m+\delta\sigma_i$ and neglect the product of fluctuations:

$$
\sigma_i\sigma_j\simeq m\sigma_i+m\sigma_j-m^2.
$$

The resulting independent-spin [statistical Hamiltonian](../../../../../../statistical-hamiltonian.md) is

$$
H_{\mathrm{MF}}=\frac{Nc}{2}m^2-(h+cm)\sum_i\sigma_i.
$$

The constant corrects the double counting of interaction energy. The [Ising spin](../../../../../../ising-spin-variable.md) sums now factorize and can all be evaluated:

$$
\boxed{Z_{\mathrm{MF}}(h;m)
=e^{-\beta_TNc m^2/2}\left[2\cosh\bigl(\beta_T(h+cm)\bigr)\right]^N.}
$$

This is the approximate [partition function](../../../../../../canonical-partition-function.md) at an assumed mean field; equilibrium fixes $m$ self-consistently. The corresponding [Ising auxiliary mean-field free energy](../../../../../../ising-auxiliary-mean-field-free-energy.md) is

$$
\boxed{A_{\mathrm{aux}}(h,m)
=N\left[\frac c2m^2-k_BT\log\left(2\cosh\frac{h+cm}{k_BT}\right)\right].}
$$

Its equilibrium value gives the mean-field [Helmholtz free energy](../../../../../../helmholtz-free-energy.md) in the imposed field. Away from a [stationary point](../../../../../../stationary-point.md) its parameter $m$ is an assumed field variable, not necessarily the actual mean [Ising spin](../../../../../../ising-spin-variable.md) of that independent-spin distribution.

For the full small-$m$ expansion at fixed $h$, set $t_h=\tanh(\beta_Th)$ and $s_h=\operatorname{sech}^2(\beta_Th)$. Differentiating $\log\cosh z$ gives successive derivatives $t_h$, $s_h$, $-2t_hs_h$, and $2s_h(2-3s_h)$ at $z=\beta_Th$. Therefore

$$
\frac{A_{\mathrm{aux}}(h,m)}N
=-k_BT\log[2\cosh(\beta_Th)]-ct_hm
+\frac12(c-\beta_Tc^2s_h)m^2
+\frac{\beta_T^2c^3t_hs_h}{3}m^3
+\frac{\beta_T^3c^4s_h(3s_h-2)}{12}m^4+O(m^5).
$$

At zero field, [spin inversion symmetry](../../../../../../spin-inversion-symmetry.md) eliminates odd powers and this simplifies to

$$
\boxed{\frac{A_{\mathrm{aux}}(0,m)}N
=-k_BT\log2+\frac c2\left(1-\frac c{k_BT}\right)m^2
+\frac{c^4}{12(k_BT)^3}m^4+O(m^6).}
$$

The quadratic coefficient changes sign and the quartic coefficient is positive at

$$
\boxed{T_c=\frac{qJ}{k_B}=\frac{2DJ}{k_B}.}
$$

Thus the zero-field mean-field prediction is a **continuous, [continuous phase transition](../../../../../../continuous-phase-transition.md)**: the stable zero [spin magnetization](../../../../../../spin-magnetization.md) develops two symmetry-related nonzero minima continuously below $T_c$.

Both requested routes give the same [mean-field self-consistency equation](../../../../../../self-consistency-equation.md). First, the one-spin expectation in the effective field is

$$
m=\frac{\sum_{\sigma=\pm1}\sigma e^{\beta_T(h+cm)\sigma}}
{\sum_{\sigma=\pm1}e^{\beta_T(h+cm)\sigma}}
=\boxed{\tanh[\beta_T(h+cm)]}.
$$

Second, differentiating the [Ising auxiliary mean-field free energy](../../../../../../ising-auxiliary-mean-field-free-energy.md) gives

$$
\frac1N\frac{\partial A_{\mathrm{aux}}}{\partial m}
=c\{m-\tanh[\beta_T(h+cm)]\},
$$

whose stationary condition is precisely that [mean-field self-consistency equation](../../../../../../self-consistency-equation.md). Choose its stable, lowest-free-energy branch rather than every algebraic solution.

An equally useful [mean-field approximation](../../../../../../mean-field-approximation.md) parametrizes the trial distribution by its actual mean [Ising spin](../../../../../../ising-spin-variable.md). Its probabilities are $(1\pm m)/2$, giving the [Bragg-Williams free energy of the Ising model](../../../../../../bragg-williams-free-energy-of-the-ising-model.md)

$$
\frac{A_{\mathrm{BW}}(h,m)}N
=-\frac c2m^2-hm+k_BT\left[
\frac{1+m}{2}\log\frac{1+m}{2}
+\frac{1-m}{2}\log\frac{1-m}{2}\right],\qquad |m|\le1.
$$

This energy-minus-entropy function has expansion

$$
\boxed{\frac{A_{\mathrm{BW}}(h,m)}N
=-k_BT\log2-hm+\frac{k_BT-c}{2}m^2+\frac{k_BT}{12}m^4+O(m^6).}
$$

Its stationary equation is $h=k_BT\operatorname{arctanh}m-cm$, again equivalent to the [mean-field self-consistency equation](../../../../../../self-consistency-equation.md). The two functions differ away from equilibrium, but agree on stationary branches: for $z=\beta_T(h+cm)$ and $m=\tanh z$, the [entropy](../../../../../../entropy.md) bracket equals $mz-\log(2\cosh z)$. Their small-$m$ coefficients therefore need not agree at arbitrary temperature; at $T_c$ they have the same leading critical quartic coefficient $c/12$. This distinction prevents confusing the auxiliary-field expansion with the physical-magnetization variational expansion.

For the [order-parameter critical exponent](../../../../../../order-parameter-critical-exponent.md), expand the equation of state at $h=0$:

$$
0=(k_BT-c)m+\frac{k_BT}{3}m^3+O(m^5).
$$

On a nonzero stable branch,

$$
m^2=\frac{3(c-k_BT)}{k_BT}+O((T_c-T)^2)
\sim\frac{3(T_c-T)}{T_c}.
$$

Hence **$\beta=1/2$**. The [spontaneous magnetization](../../../../../../spontaneous-magnetization.md) is understood by selecting a branch with an infinitesimal field after the [thermodynamic limit](../../../../../../thermodynamic-limit.md); a finite symmetric sample has zero exact zero-field mean [Ising spin](../../../../../../ising-spin-variable.md).

For the [magnetic susceptibility](../../../../../../magnetic-susceptibility.md) per site, define $\chi=\partial m/\partial h$ with $h$ in energy units. Implicit differentiation gives

$$
\boxed{\chi=\frac{\beta_T(1-m^2)}{1-\beta_Tc(1-m^2)}
=\frac{1}{k_BT/(1-m^2)-c}.}
$$

Above $T_c$, $m=0$ and $\chi=1/[k_B(T-T_c)]$. Below $T_c$, evaluated on a selected ordered branch, the expansion of $m^2$ gives $\chi\sim1/[2k_B(T_c-T)]$. Thus the [magnetic-susceptibility critical exponent](../../../../../../magnetic-susceptibility-critical-exponent.md) is **$\gamma=1$ on both sides**, with different amplitudes. At $T=T_c$, the equation of state becomes

$$
h=\frac c3m^3+O(m^5),\qquad
m\sim\operatorname{sgn}(h)\left(\frac{3|h|}{c}\right)^{1/3},
$$

so the [critical-isotherm exponent](../../../../../../critical-isotherm-exponent.md) is **$\delta=3$**. These are [mean-field critical exponents](../../../../../../mean-field-critical-exponent.md), not a claim that neglecting fluctuations gives the exact Ising transition in every dimension.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 303](../../../paper-303-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
