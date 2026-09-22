<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [random walk](../../../../../../random-walk.md) interpretation and [optimal stopping value function](../../../../../../optimal-stopping-value-function.md) recursion specified in part (b). If $h$ is [convex](../../../../../../convex-function.md), translating and integrating its [convexity](../../../../../../convex-function.md) inequality gives, for $0<\theta<1$,

$$
\begin{aligned}
(Ph)(\theta x+(1-\theta)y)
&=\int h\big(\theta(x+z)+(1-\theta)(y+z)\big)\,\nu(dz)\\
&\leq\theta(Ph)(x)+(1-\theta)(Ph)(y).
\end{aligned}
$$

Thus the [transition operator](../../../../../../transition-operator.md) preserves [convex functions](../../../../../../convex-function.md). Also the [pointwise maximum of convex functions](../../../../../../pointwise-maximum-of-convex-functions.md) is [convex](../../../../../../convex-function.md): each of two [convex functions](../../../../../../convex-function.md) at an intermediate point is bounded by the same convex combination of their pointwise maximum at the endpoints. Starting with $V(T,\cdot)=f$, backward induction in

$$
V(t,\cdot)=\max\{f,PV(t+1,\cdot)\}
$$

therefore proves **the asserted convexity in the intended model**:

$$
\boxed{V(t,\cdot)\text{ is convex for every }0\leq t\leq T.}
$$

The statewise integrability convention in part (b) gives finite [convex functions](../../../../../../convex-function.md) on all real states. The same inequality holds for the canonical extended value function wherever the expectations are well-defined. Integrability only along one started process need not make that canonical function finite at unused states: for $T=1$, $S_0=0$, $f(s)=e^{s^2}$ and increment density proportional to $e^{-y^2-|y|}$, $\mathbb E f(S_1)<\infty$, but $\mathbb E f(s+Y_1)=\infty$ for $s>1/2$. This concerns the canonical recursion away from visited states, rather than the almost-sure identity for $U$. Arbitrary off-state versions of $V$ need not be [convex](../../../../../../convex-function.md); the recursive version is the one meant here. No zero-mean assumption on the increments was used, and [convexity](../../../../../../convex-function.md) alone does not make $f(S_t)$ a [submartingale](../../../../../../submartingale.md) for an arbitrary drift.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
