<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $e=E'(1)>0$, $q_1=q'(1)>0$ and introduce perturbations $(H,U,C,S)e^{\lambda t+ikx}$ to [water depth](../../../../water-depth.md), [velocity](../../../../velocity.md), [concentration](../../../../concentration.md) and bed height. Take the leading [quasi-steady approximation](../../../../quasi-steady-approximation.md) $\epsilon=0$ for the fast [water](../../../../water.md) and suspension response, retaining the small [friction](../../../../friction.md) parameter $\delta$. For $k\ne0$, the linearized equations are

$$
\begin{aligned}
&H+U=0,\\
&[ik(F^2-1)+3\delta]U=-ikS,\\
&(\gamma+ik)C=\gamma eU,\\
&\lambda S+ikq_1U=\beta(C-eU).
\end{aligned}
$$

Here surface height is $H+S$, and [linearization](../../../../linearization.md) of $1-u^2/h$ gives $H-2U=-3U$. Eliminating $H,C,U$ gives the [dispersion relation](../../../../dispersion-relation-split.md)

$$
\boxed{\lambda(k)=-\frac{k^2\left(q_1+\dfrac{\beta e}{\gamma+ik}\right)}{3\delta+ik(F^2-1)}.}
$$

In particular, putting $B=F^2-1\ne0$ and expanding at large $|k|$,

$$
\boxed{\lambda(k)=i\frac{q_1}{B}k+\frac{\beta e}{B}-\frac{3\delta q_1}{B^2}+O(k^{-1}).}
$$

Thus the temporal growth rate tends to a finite constant, while the [phase velocity](../../../../phase-velocity.md) is

$$
\boxed{v_{\mathrm{ph}}=-\frac{\operatorname{Im}\lambda}{k}\longrightarrow-\frac{q_1}{F^2-1}.}
$$

For [supercritical flow](../../../../supercritical-flow.md) $F>1$, the waves propagate upstream. They grow if $\beta e(F^2-1)>3\delta q_1$; at leading order in small $\delta$, this holds for fixed positive $\beta,e$ away from critical flow. They are [antidunes](../../../../antidune.md), upstream-migrating bedforms coupled to the free surface. Indeed $H=-U$ and $S\simeq-(F^2-1)U$, so surface height $H+S\simeq-F^2U$ is in phase with the bed perturbation in this regime.

For clarity, neglecting $\delta$ completely gives the exact leading-order expressions

$$
\operatorname{Re}\lambda=\frac{\beta e}{F^2-1}\frac{k^2}{\gamma^2+k^2},\qquad v_{\mathrm{ph}}=-\frac1{F^2-1}\left(q_1+\frac{\beta e\gamma}{\gamma^2+k^2}\right).
$$

These also identify the missing qualification in the source: **the unstable upstream branch requires $F>1$.** For $F<1$ this leading model gives decay and downstream propagation. The near-critical case $F^2-1\simeq0$ needs a different balance; it is not covered by the expansion. Small nonzero $\epsilon$ perturbs the slow bedform branch and adds fast [water](../../../../water.md) modes, so the stated result concerns the leading slow morphodynamic branch. This is the [high-wavenumber antidune dispersion](../../../../high-wavenumber-antidune-dispersion.md) calculation.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the mathematics and the environment course of the University of Oxford](../../../split.md)
5. [Mathematics and the environment course of the University of Oxford](../../../../mathematics-and-the-environment-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
