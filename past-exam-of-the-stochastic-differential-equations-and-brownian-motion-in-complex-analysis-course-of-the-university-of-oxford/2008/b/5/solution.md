<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $Z=X+iY$, with $Y$ a real [Brownian motion](../../../../brownian-motion-split.md) started at one. For the nontrivial strip calculation assume $r>1$, so the starting point is in its interior. The first exit time is

$$
T_S=\inf\{t\geq0:Z_t\notin S\}.
$$

For a continuous Brownian path started inside, this equals the first hitting time of $Y=0$ or $Y=r$ almost surely: [Brownian motion](../../../../brownian-motion-split.md) started at a boundary immediately visits the exterior, so using the closed strip in the definition does not change the infimum.

If $T_S>n$, then $Y_n\in[0,r]$. Its normal density is bounded by $(2\pi n)^{-1/2}$, hence

$$
\mathbb P(T_S>n)\leq\mathbb P(0\leq Y_n\leq r)
\leq\frac r{\sqrt{2\pi n}}\longrightarrow0.
$$

Thus the exit time is finite almost surely.

The stopped harmonic coordinate $Y_{t\wedge T_S}$ is a [martingale](../../../../martingale-split.md) bounded between zero and $r$. [bounded convergence theorem](../../../../bounded-convergence-theorem.md) and [optional stopping theorem](../../../../optional-sampling-theorem-for-a-supermartingale.md) give $\mathbb EY_{T_S}=Y_0=1$. Since the exit coordinate is zero or $r$,

$$
\boxed{\mathbb P(Y_{T_S}=r)=\frac1r,\qquad
\mathbb P(Y_{T_S}=0)=1-\frac1r.}
$$

If $T$ is the first hit of the real axis, exit through the lower boundary implies $T<\infty$, so $\mathbb P(T<\infty)\geq1-1/r$ for every $r>1$. Letting $r\to\infty$ proves

$$
\boxed{\mathbb P(T<\infty)=1.}
$$

The strip assumption is worth making explicit: at $r=1$ the initial point is the upper boundary and exit is immediate; for $0<r<1$ it starts outside the strip and the displayed interior probabilities do not apply.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../split.md)
5. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
