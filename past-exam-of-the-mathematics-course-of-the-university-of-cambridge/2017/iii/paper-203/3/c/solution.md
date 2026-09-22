<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) $\partial_tg_t=2/(g_t-U_t)$ with $U_t=\sqrt\kappa B_t$. For a fixed $z\in\mathbb H$, let $T_z$ be its [Loewner swallowing time](../../../../../../interior-point-swallowing-time-for-a-loewner-chain.md), and write $Z_t=X_t+iY_t=g_t(z)-U_t$ and $J_t=|g_t'(z)|$ before that time. The [Loewner conformal radius](../../../../../../conformal-radius-under-a-chordal-loewner-flow.md) is $\Upsilon_t=Y_t/J_t$, half of the [conformal radius](../../../../../../conformal-radius.md) of $D_t=\mathbb H\setminus K_t$ at $z$. The [Koebe quarter theorem](../../../../../../koebe-quarter-theorem.md) bounds the [conformal radius](../../../../../../conformal-radius.md) above by four times the distance to the [boundary](../../../../../../boundary-of-a-set.md). For the reverse comparison, if $\phi:\mathbb D\to D_t$ maps zero to $z$, apply the [Schwarz lemma](../../../../../../schwarz-lemma.md) to $\phi^{-1}(z+dw)$ on the [unit disc](../../../../../../unit-disc.md), where $d=\operatorname{dist}(z,\partial D_t)$; it gives $d\leq|\phi'(0)|$. Thus

$$
\frac12\operatorname{dist}(z,\partial D_t)\leq\Upsilon_t\leq2\operatorname{dist}(z,\partial D_t).
$$

We use the basic trace theorems that, for $\kappa>8$, the [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) is continuous and [Transience of chordal SLE](../../../../../../transience-of-chordal-sle.md) gives $|\gamma(t)|\to\infty$. These facts make its image relatively closed in $\mathbb H$; they do not assume the space-filling conclusion. The [continuity](../../../../../../continuous-function.md) and transience statements are available in [Rohde and Schramm's basic trace theorems](https://annals.math.princeton.edu/wp-content/uploads/annals-v161-n2-p07.pdf).

Take $\rho=\kappa-8>0$ in the supplied [SLE interior-point martingale](../../../../../../sle-interior-point-martingale.md). The [derivative](../../../../../../derivative.md) exponent vanishes, leaving

$$
M_t=\Upsilon_t^{a}S_t^{-b},\qquad a=\frac{\kappa-8}{8}>0,\quad b=\frac{\kappa-8}{\kappa}>0,\quad S_t=\frac{Y_t}{|Z_t|}.
$$

A [nonnegative local martingale](../../../../../../nonnegative-local-martingale.md) is a [supermartingale](../../../../../../supermartingale.md). Applying the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) after localization at its first hit of a level $R$ gives the [maximal inequality for a nonnegative supermartingale](../../../../../../maximal-inequality-for-a-nonnegative-supermartingale.md)

$$
\mathbb P\!\left(\sup_{t<T_z}M_t\geq R\right)\leq\frac{M_0}{R}.
$$

Thus $C=\sup_{t<T_z}M_t<\infty$ almost surely.

Suppose the [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) avoids some [open ball](../../../../../../open-ball.md) $B(z,r)$ whose [closure](../../../../../../closure-topology.md) is inside $\mathbb H$. Before $T_z$, the whole [open ball](../../../../../../open-ball.md) is in $D_t$: a [connected](../../../../../../connected-space.md) [open ball](../../../../../../open-ball.md) disjoint from the trace cannot be partly in the unbounded [connected component](../../../../../../connected-component.md). Hence $\Upsilon_t\geq r/2$. The bound on $M$ forces $S_t\geq c>0$ throughout this interval, for a positive random constant $c$.

The [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) and its [derivative](../../../../../../derivative.md) yield

$$
\frac{d}{dt}Y_t^2=-4S_t^2,\qquad \frac{d}{dt}\log\Upsilon_t=-\frac{4Y_t^2}{|Z_t|^4},\qquad \frac{d\log\Upsilon_t}{d\log Y_t}=2S_t^2.
$$

The first identity forces $T_z<\infty$, since otherwise $Y_t^2\leq Y_0^2-4c^2t$ becomes negative. At a finite maximal lifetime, $Y_t\to0$; otherwise the continuous [Loewner driving function](../../../../../../loewner-driving-function.md) and the [ordinary differential equation](../../../../../../ordinary-differential-equation.md) continue past that time. Integrating the last identity, using $S_t\geq c$, gives

$$
\Upsilon_t\leq\Upsilon_0\left(\frac{Y_t}{Y_0}\right)^{2c^2}\longrightarrow0,
$$

contradicting $\Upsilon_t\geq r/2$. Thus every fixed rational ball inside $\mathbb H$ is hit almost surely. A countable intersection makes the trace a [dense subset](../../../../../../dense-set.md) almost surely, and its relatively closed image, established by [continuity](../../../../../../continuous-function.md) and transience, then contains all of $\mathbb H$:

$$
\boxed{\mathbb H\subseteq\gamma[0,\infty)\quad\text{almost surely for }\kappa>8.}
$$

This proves [space-filling SLE above parameter eight](../../../../../../space-filling-sle-above-parameter-eight.md). It rules out unvisited open regions, rather than inferring visits merely from membership in the filled [compact H-hulls](../../../../../../compact-h-hull.md). The choice $\rho=\kappa-8$ does not address the critical value eight.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
