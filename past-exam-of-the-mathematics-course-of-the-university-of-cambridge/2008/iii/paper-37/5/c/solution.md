<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed $\varepsilon>0$, the derivative of $\sigma_\varepsilon$ is zero on $(-\infty,\varepsilon/2]$, bounded on the compact transition interval $[\varepsilon/2,\varepsilon]$, and equals $1/(2\sqrt x)\leq1/(2\sqrt\varepsilon)$ for $x\geq\varepsilon$. Thus $\sigma_\varepsilon$ is globally Lipschitz, with at most linear growth. The [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../../../../global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients.md) supplies a global [strong stochastic solution](../../../../../../strong-solution-of-a-stochastic-differential-equation.md) and [pathwise uniqueness](../../../../../../pathwise-uniqueness.md) for the modified equation.

The solution stays nonnegative. More precisely, if $z>\varepsilon/2$, it cannot cross $\varepsilon/2$: on reaching this level the constant continuation solves the equation, and [pathwise uniqueness](../../../../../../pathwise-uniqueness.md) forces that continuation. If $z\leq\varepsilon/2$, it is constant from the outset. In either case $Z^\varepsilon$ is a [nonnegative local martingale](../../../../../../nonnegative-local-martingale.md), so $\mathbb E Z^\varepsilon_s\leq z$.

For $\varepsilon'<\varepsilon<z$, both coefficients agree with $\sqrt x$ on $[\varepsilon,\infty)$. Stop the two solutions when either first reaches $\varepsilon$, and also at a common upper bound. On the resulting compact state interval, the coefficient is Lipschitz. The [Itô isometry](../../../../../../ito-isometry.md) applied to their difference, followed by the [Gronwall inequality](../../../../../../gronwall-inequality.md), gives zero expected squared difference. Remove the upper bound using the nonexplosion of each modified solution. The two solutions agree until the first of these lower exits, and by continuity both have value $\varepsilon$ there, so their exits at that level coincide. In particular,

$$
\boxed{Z^{\varepsilon'}_t=Z^\varepsilon_t\quad(0\leq t\leq T_\varepsilon),}
$$

up to indistinguishability. If $\varepsilon\geq z$, the first exit time is zero and the same assertion is immediate from their initial values.

Now take a decreasing sequence $0<\varepsilon_n<z$ with $\varepsilon_n\downarrow0$. Write $Z^n=Z^{\varepsilon_n}$ and $\tau_n=T_{\varepsilon_n}$. Compatibility gives $\tau_n\leq\tau_{n+1}$; indeed, a continuous path cannot reach the smaller level before reaching the larger one. Let $\tau=\lim_n\tau_n$, a [stopping time](../../../../../../stopping-time.md). On $[0,\tau)$ the compatible solutions define an adapted continuous process $Z$ by setting $Z_t=Z^n_t$ whenever $t\leq\tau_n$. We still need to justify the finite limiting endpoint and the integral equation there, rather than assume they exist.

For this purpose use the compatible predictable integrands

$$
H^n_s=\mathbf1_{\{s\leq\tau_n\}}\sqrt{Z^n_s}.
$$

Their squares increase pointwise with $n$: on the smaller interval compatibility makes the values equal, and outside it the old integrand is zero. Their limit $H$ is predictable and equals $\sqrt{Z_s}$ before $\tau$, and zero after $\tau$, apart from irrelevant single-time endpoints. For every finite $t$,

$$
\mathbb E\int_0^t(H^n_s)^2ds
=\int_0^t\mathbb E\bigl[\mathbf1_{\{s\leq\tau_n\}}Z^n_s\bigr]ds\leq zt.
$$

The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) gives $\mathbb E\int_0^tH_s^2ds\leq zt$. Moreover, compatibility makes $(H-H^n)^2=H^2-(H^n)^2$ away from endpoints, so its expected time-integral tends to zero. The [Itô isometry](../../../../../../ito-isometry.md), and the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) if uniform convergence on a finite time interval is desired, therefore give a continuous stochastic-integral limit

$$
L_t=z+\int_0^tH_s\,dB_s.
$$

Before $\tau_n$, the integrand agrees with $\sqrt{Z^n}$, which is the original square-root coefficient there. Locality of the [stochastic integral](../../../../../../stochastic-integral.md) yields $L_{t\wedge\tau_n}=Z^n_{t\wedge\tau_n}$. A countable intersection in $n$ and path continuity give this equality simultaneously for all times.

On $\{\tau<\infty\}$, every $\tau_n$ is finite and $L_{\tau_n}=\varepsilon_n$. Continuity of $L$ thus gives $L_\tau=0$. The limiting integrand is zero after $\tau$, so $L$ remains zero afterward. On $\{\tau=\infty\}$, every finite time is covered by one of the compatible positive solutions. Consequently $L$ is nonnegative everywhere and $H_s=\sqrt{L_s}$ for almost every $s$, including after absorption. The [cutoff construction of an absorbed square-root diffusion](../../../../../../cutoff-construction-of-an-absorbed-square-root-diffusion.md) has produced

$$
\boxed{Z_t=L_t=z+\int_0^t\sqrt{Z_s}\,dB_s,\qquad Z_t=0\text{ for }t\geq\tau\text{ if }\tau<\infty.}
$$

All modified solutions, [stopping times](../../../../../../stopping-time.md) and integrands were constructed from the same prescribed [Brownian motion](../../../../../../brownian-motion-split.md); hence this is a [strong stochastic solution](../../../../../../strong-solution-of-a-stochastic-differential-equation.md). The integral is square-integrable on every finite horizon by the bound $zt$, which also rules out a hidden finite-time explosion in the patching argument.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
