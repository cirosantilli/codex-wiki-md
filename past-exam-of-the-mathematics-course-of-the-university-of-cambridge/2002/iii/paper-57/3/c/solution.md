<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Both weights now equal farm size, giving the [farm-size stratified SIR model](../../../../../../farm-size-stratified-sir-model.md)

$$
\dot S_n=-\beta nS_nJ,\qquad \dot I_n=\beta nS_nJ-\gamma I_n,\qquad J=\sum_nnI_n.
$$

The next-generation [matrix](../../../../../../matrix.md) is $K_{nm}=(\beta/\gamma)nP_nm$, whose nonzero [eigenvalue](../../../../../../eigenvalue.md) is

$$
\boxed{\mathcal R_0=\frac{\beta\mu_2}{\gamma},\qquad
\mathcal R_{0,\rm hom}=\frac{\beta\mu^2}{\gamma},\qquad
\frac{\mathcal R_0}{\mathcal R_{0,\rm hom}}=1+\frac{\operatorname{Var}(n)}{\mu^2}.}
$$

The [variance](../../../../../../variance-split.md) matters because large farms are both more likely to acquire infection and more effective sources afterward. This positive correlation increases the [basic reproduction number](../../../../../../basic-reproduction-number.md) relative to the homogeneous [SIR model](../../../../../../sir-model.md). In particular the heterogeneous population can permit invasion when the homogeneous comparison is subcritical.

Put $\Lambda=\beta\int_0^tJ(u)\,du$. Apart from the negligible initial seed, $S_n=P_ne^{-n\Lambda}$. The susceptible [mean](../../../../../../expected-value.md) obeys $\dot\mu_S=-\beta J\operatorname{Var}_S(n)$. For infectives, the incidence [mean](../../../../../../expected-value.md) is again $\mu_{\rm inc}=\sum_nn^2S_n/\sum_nnS_n$, and

$$
\dot\mu_I=\frac{\beta J\sum_nnS_n}{I}(\mu_{\rm inc}-\mu_I).
$$

The growing mode $I_n\propto nP_n$ has [mean](../../../../../../expected-value.md) $\mu_2/\mu$, not $\mu$. As the larger susceptible farms are depleted, the [mean](../../../../../../expected-value.md) size of incoming infectives falls; the current infected [mean](../../../../../../expected-value.md) follows it with a delay. These equations give the direction of change for any initial condition without imposing false monotonicity of the infected [mean](../../../../../../expected-value.md).

The weighted infected total satisfies $\dot J=(\beta\sum_nn^2S_n-\gamma)J$, so the effective reproduction number declines from $\beta\mu_2/\gamma$ as the susceptible size distribution changes. The [final size relation for an epidemic](../../../../../../final-size-relation-for-an-epidemic.md) becomes

$$
\Lambda_\infty=\frac\beta\gamma\sum_nnP_n(1-e^{-n\Lambda_\infty}),\qquad
A=1-\sum_nP_ne^{-n\Lambda_\infty}.
$$

The right-column sketch illustrates the larger initial growth rate and preferential depletion of large farms. The homogeneous comparison has size $\mu$ in both transmission factors; it must not be assigned the heterogeneous second moment. **The general conclusions are enhanced invasion and selective removal of large susceptible farms.** The final unweighted fraction of farms infected has no universal ordering relative to the homogeneous comparison: higher transmission and stronger heterogeneity-induced depletion compete, and the displayed final-size equations determine the answer for a specified distribution. For example, with $P_1=P_3=1/2$, the infinitesimal-seed attack fractions are approximately $0.367$ versus $0.176$ when the homogeneous reproduction number is $1.1$, but $0.740$ versus $0.797$ when it is $2$; the two comparisons have opposite ordering.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
