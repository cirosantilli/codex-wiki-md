<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Uniqueness in law](../../../../../../uniqueness-in-law.md) means that, for a fixed initial value, every two [weak stochastic solutions](../../../../../../weak-solution-of-a-stochastic-differential-equation.md) of the [stochastic differential equation](../../../../../../stochastic-differential-equation.md) have the same distribution as entire solution paths, even if their filtered probability spaces and driving [Brownian motions](../../../../../../brownian-motion-split.md) differ. For an equation on $(0,\infty)$, initially consider the stopped path and lifetime at the boundary.

We first justify that the boundary cannot intervene when $\gamma\ge2$. For any solution of the displayed Bessel equation, let $\tau_{\varepsilon,L}$ be its first exit from $(\varepsilon,L)$, where $0<\varepsilon<r<L$. Applying Itô to $R^2$ gives

$$
\mathbb E R_{t\wedge\tau_{\varepsilon,L}}^2
=r^2+\gamma\mathbb E(t\wedge\tau_{\varepsilon,L})\le L^2.
$$

Thus the annulus exit has finite expectation and is almost surely finite. The one-dimensional generator is $\frac12\partial_{rr}+\frac{\gamma-1}{2r}\partial_r$. Its harmonic scale functions are $\log r$ for $\gamma=2$ and $r^{2-\gamma}$ for $\gamma>2$, as direct differentiation verifies. They are bounded on the stopped annulus, so optional sampling gives

$$
\mathbb P_r(\tau_\varepsilon<\tau_L)=
\begin{cases}
\dfrac{\log(L/r)}{\log(L/\varepsilon)},&\gamma=2,\\
\dfrac{r^{2-\gamma}-L^{2-\gamma}}{\varepsilon^{2-\gamma}-L^{2-\gamma}},&\gamma>2.
\end{cases}
$$

Both tend to zero as $\varepsilon\downarrow0$. A continuous path hitting zero before $\tau_L$ would hit every inner level first, so that event has probability zero. Exhausting the upper levels proves that zero is not hit at any finite time. Nor can an upper explosion occur: localization of $R^2$ gives $\mathbb P(\tau_L\le t)\le(r^2+\gamma t)/L^2\to0$. These are the [Hitting-zero classification for a Bessel process](../../../../../../hitting-zero-classification-for-a-bessel-process.md) arguments needed for the dimension-at-least-two case.

Now suppose $\gamma$ is an integer and take a $\gamma$-dimensional [Brownian motion](../../../../../../brownian-motion-split.md) $U$ from any deterministic vector $u$ with $|u|=r$. For $\rho=|U|>0$, differentiation of the [Euclidean norm](../../../../../../euclidean-norm.md) gives

$$
\partial_i|u|=u_i/|u|,\qquad \Delta|u|=(\gamma-1)/|u|.
$$

Define the radial noise $\beta=\sum_i\int U_i/\rho\,dW_i$, filling the integrand by a fixed unit vector on the zero set, as in part (b). It has bracket $t$ and is a [Brownian motion](../../../../../../brownian-motion-split.md). the [Itô formula](../../../../../../ito-s-lemma.md), initially before a possible zero, gives

$$
d\rho_t=d\beta_t+\frac{\gamma-1}{2\rho_t}dt,\qquad \rho_0=r.
$$

The boundary argument just given makes this a global positive [weak stochastic solution](../../../../../../weak-solution-of-a-stochastic-differential-equation.md). The assumed [uniqueness in law](../../../../../../uniqueness-in-law.md) therefore identifies every solution's path law with that of $|U|$. Orthogonal invariance of [Brownian motion](../../../../../../brownian-motion-split.md) makes this radial law independent of the selected point $u$ on the sphere. Consequently

$$
\boxed{(R_t)_{t\ge0}\ \stackrel{\mathrm{law}}=\ (|u+W_t|)_{t\ge0},\quad |u|=r.}
$$

This proves equality of process laws, not merely equality of one-time marginal distributions.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
