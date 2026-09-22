<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With susceptibility independent of size and infectivity proportional to size, define $J=\sum_nnI_n$. The [farm-size stratified SIR model](../../../../../../farm-size-stratified-sir-model.md) is

$$
\dot S_n=-\beta S_nJ,\qquad \dot I_n=\beta S_nJ-\gamma I_n,\qquad \dot R_n=\gamma I_n.
$$

An infectious size-$m$ farm has next-generation column $K_{nm}=(\beta/\gamma)P_nm$. Its sole nonzero [eigenvalue](../../../../../../eigenvalue.md) gives the [basic reproduction number](../../../../../../basic-reproduction-number.md)

$$
\boxed{\mathcal R_0=\beta\mu/\gamma,}
$$

again equal to the comparison [SIR model](../../../../../../sir-model.md).

Since every susceptible farm experiences the same [force of infection](../../../../../../force-of-infection.md), all ratios $S_n/S_m$ remain fixed. For a representative initial seed, $S_n(0)=(1-i_0)P_n$ and $I_n(0)=i_0P_n$, uniqueness of the [differential equations](../../../../../../differential-equation-split.md) gives $S_n=P_nS$, $I_n=P_nI$, $R_n=P_nR$ for all time. Consequently $J=\mu I$ and

$$
\dot S=-\beta\mu SI,\qquad \dot I=\beta\mu SI-\gamma I,\qquad \dot R=\gamma I.
$$

**For this representative seed, the heterogeneous and homogeneous [epidemics](../../../../../../epidemic.md) coincide exactly, and both susceptible and infected farm [means](../../../../../../expected-value.md) stay at $\mu$.** This is the overlapping middle-column sketch above, not merely an approximation based on equal reproduction numbers.

With a nonrepresentative seed the susceptible [mean](../../../../../../expected-value.md) remains its initial value, but the infected [mean](../../../../../../expected-value.md) need not. The influx of new infectives has the constant susceptible [mean](../../../../../../expected-value.md), so

$$
\dot\mu_I=\frac{\beta SJ}{I}(\mu_S-\mu_I).
$$

Thus it is pulled toward $\mu_S$ while incidence continues. Infectivity variation alone does not selectively remove large susceptible farms. The exact homogeneous reduction depends on the representative initial condition; specifying only $P_n$ and $\mathcal R_0$ does not determine a trajectory for every possible seed.

## ↑ Ancestors (11)

1. [B](../b.md)
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
