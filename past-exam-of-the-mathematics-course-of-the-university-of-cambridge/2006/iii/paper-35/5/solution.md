<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use one $d$-dimensional [Brownian motion](../../../../../brownian-motion-split.md) $W$ to couple the [diffusion processes](../../../../../markov-diffusion.md)

$$
X_t^\varepsilon=x_0+\int_0^t b(X_s^\varepsilon)ds+\varepsilon W_t.
$$

The [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../../../global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients.md) supplies a unique nonexplosive [strong stochastic solution](../../../../../strong-solution-of-a-stochastic-differential-equation.md). Let $x$ be the deterministic drift trajectory. Subtraction and the [Gronwall inequality](../../../../../gronwall-inequality.md) give, on every finite horizon $t$,

$$
\boxed{\sup_{s\le t}|X_s^\varepsilon-x_s|
\le\varepsilon e^{Lt}\sup_{s\le t}|W_s|\longrightarrow0\quad\text{almost surely}.}
$$

This also follows directly from the integral equations with continuous forcing, so the coupling can be chosen simultaneously for all $\varepsilon$.

For completeness derive the needed [Feynman-Kac formula](../../../../../feynman-kac-formula.md) with its potential sign. For fixed $t$, apply the [Itô formula](../../../../../ito-s-lemma.md) and the [Itô product rule](../../../../../ito-product-rule.md) to

$$
Y_s=\exp\left(\int_0^s c(X_v^\varepsilon)dv\right)
 u^\varepsilon(t-s,X_s^\varepsilon),\qquad 0\le s\le t.
$$

Its drift is the exponential factor times $-u_t^\varepsilon+(\varepsilon^2\Delta/2+b\cdot\nabla)u^\varepsilon+c u^\varepsilon$, which vanishes by the [partial differential equation](../../../../../partial-differential-equation-split.md). It is a [local martingale](../../../../../local-martingale.md). Boundedness of $u^\varepsilon$ on the finite time slab and boundedness of $c$ make $Y$ bounded there, so it is a true [martingale](../../../../../martingale-split.md). Its endpoint expectations give

$$
u^\varepsilon(t,x_0)=\mathbb E\left[f(X_t^\varepsilon)
\exp\left(\int_0^t c(X_s^\varepsilon)ds\right)\right].
$$

The deterministic trajectory on $[0,t]$ is compact. Uniform pathwise convergence puts all sufficiently small-noise paths in a fixed compact neighbourhood of that trajectory. Continuity of $c$ therefore implies $\sup_{s\le t}|c(X_s^\varepsilon)-c(x_s)|\to0$; global [uniform continuity](../../../../../uniform-continuity.md) of $c$ is not required. Continuity of $f$ gives convergence of the terminal factor. Finally,

$$
\left|f(X_t^\varepsilon)\exp\left(\int_0^tc(X_s^\varepsilon)ds\right)\right|
\le\|f\|_\infty e^{t\|c\|_\infty}.
$$

The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) proves the [zero-noise limit with a bounded potential](../../../../../zero-noise-limit-with-a-bounded-potential.md):

$$
\boxed{u^\varepsilon(t,x_0)\longrightarrow
f(x_t)\exp\left(\int_0^t c(x_s)ds\right).}
$$

At $t=0$ this is the given initial condition. All boundedness arguments concern a fixed finite horizon; no uniform bound over infinite time is needed.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
