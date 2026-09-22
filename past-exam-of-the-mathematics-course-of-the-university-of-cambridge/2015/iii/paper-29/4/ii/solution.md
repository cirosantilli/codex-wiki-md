<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The construction is well defined. Since $D$ is contained in a ball, its [Brownian exit time](../../../../../../brownian-exit-time.md) is finite [almost surely](../../../../../../almost-sure-convergence.md): at successive integer times there is a fixed positive probability that the next independent unit-time [Brownian motion](../../../../../../brownian-motion-split.md) increment has length greater than the ball's diameter, forcing an exit. The survival probability is therefore bounded by a geometric sequence. Path continuity gives $B_{\tau_D}\in\partial D$. Thus the bounded [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md) give a bounded Borel function $u$ on $D$.

For interior harmonicity, fix a ball with closure in $D$, centred at $x$, and let $\sigma$ be its [Brownian exit time](../../../../../../brownian-exit-time.md). The [Strong Markov property](../../../../../../strong-markov-property.md), followed by the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md), gives

$$
u(x)=\mathbb E_x[u(B_\sigma)].
$$

The [orthogonal invariance of Brownian motion](../../../../../../orthogonal-invariance-of-brownian-motion.md) makes $B_\sigma$ uniform on the boundary sphere. Hence $u$ has the spherical [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md) for every such ball. A locally bounded Borel function with this property is smooth and harmonic: integrating the spherical averages against any smooth radial [mollifier](../../../../../../mollifier.md) gives $u=u*\rho$ locally, which first proves smoothness; the [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md) then implies $\Delta u=0$.

For the boundary limit at $\xi$, choose the harmonic [barrier for the Dirichlet problem](../../../../../../barrier-for-the-dirichlet-problem.md) $h_\xi$ from (i). The [Itô formula](../../../../../../ito-s-lemma.md), localized inside $D$, makes $h_\xi(B_{t\wedge\tau_D})$ a bounded [martingale](../../../../../../martingale-split.md). Compact localization and the [bounded convergence theorem](../../../../../../bounded-convergence-theorem.md), first to the exit and then as $t\to\infty$, yield

$$
\mathbb E_x h_\xi(B_{\tau_D})=h_\xi(x).
$$

For $\varepsilon>0$, if $\partial D\setminus B(\xi,\varepsilon)$ is nonempty, [compactness](../../../../../../compact-space.md) and barrier positivity give

$$
c_\varepsilon=\min_{\eta\in\partial D,\ |\eta-\xi|\geq\varepsilon}h_\xi(\eta)>0,\qquad
\mathbb P_x(|B_{\tau_D}-\xi|\geq\varepsilon)\leq\frac{h_\xi(x)}{c_\varepsilon}\longrightarrow0\quad(x\to\xi).
$$

If that boundary subset is empty, the probability is already zero. Therefore

$$
|u(x)-f(\xi)|\leq\sup_{\eta\in\partial D,\ |\eta-\xi|<\varepsilon}|f(\eta)-f(\xi)|+2\|f\|_\infty\mathbb P_x(|B_{\tau_D}-\xi|\geq\varepsilon).
$$

First let $x\to\xi$ and then $\varepsilon\downarrow0$. The [continuity](../../../../../../continuous-function.md) of the [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md) proves $u(x)\to f(\xi)$.

Finally, the difference of two continuous solutions is a [harmonic function](../../../../../../harmonic-function.md) vanishing on the boundary. The [maximum principle for harmonic functions](../../../../../../maximum-principle-for-harmonic-functions.md) on the bounded domain gives that it is zero. Thus **the [Kakutani solution of the Dirichlet problem](../../../../../../kakutani-solution-of-the-dirichlet-problem.md) exists, attains every prescribed boundary value, and is unique**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
