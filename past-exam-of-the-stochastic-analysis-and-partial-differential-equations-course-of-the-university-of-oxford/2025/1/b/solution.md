<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The displayed identity requires a correction to the process construction in the source.** In a [piecewise-deterministic Markov process](../../../../piecewise-deterministic-markov-process.md), the instantaneous [hazard function](../../../../hazard-function.md) is evaluated at the current flowing state $X_{u-}$, and the destination is sampled from $K_u(X_{u-},dy)$. Keeping the jump times and destinations of the original [Markov jump process](../../../../markov-jump-process.md) $Y$ instead evaluates both quantities at its last reset state $Y_{u-}$, which generally differs from $X_{u-}$. The source PDF confirms that these original jump times and destinations were retained. Consequently its definition does not in general produce the asserted [transition kernel](../../../../markov-kernel.md), or even a [Markov process](../../../../markov-process-split.md) in the state variable $X$ alone.

For an explicit counterexample, take $a(t,x)=1$, $\alpha(x)=2+\tanh x$, $y_0=0$, and let every $K_t(x,dy)$ be the [standard normal distribution](../../../../standard-normal-distribution.md), independently of $t,x$. These are smooth coefficients with bounded positive jump rate, so [nonexplosion](../../../../nonexplosion-of-a-continuous-time-markov-chain.md) holds. In the literal construction, the first holding time has the [exponential distribution](../../../../exponential-distribution.md) of rate $2$. Thus the [probability distribution](../../../../probability-distribution-split.md) of $X_t$ has an atom of mass $e^{-2t}$ at $t$. Paths with at least one jump contribute no atom there, because the reset has a [normal density](../../../../normal-density.md). The asserted identity instead assigns to this no-jump atom the mass

$$
\exp\left(-\int_0^t(2+\tanh u)\,du\right)=\frac{e^{-2t}}{\cosh t},
$$

which differs for every $t>0$.

Here is the full derivation for the intended [piecewise-deterministic Markov process](../../../../piecewise-deterministic-markov-process.md). Assume [nonexplosion](../../../../nonexplosion-of-a-continuous-time-markov-chain.md); smoothness alone does not guarantee it. Start at $(s,x)$, let $\tau$ be the first jump after $s$, and set

$$
z(u)=\varphi(s,x,u),\qquad H(u)=\int_s^u\alpha(z(r))\,dr.
$$

One precise construction draws an independent unit-rate [exponential random variable](../../../../exponential-distribution.md) $E$ and takes $\tau=\inf\{u\geq s:H(u)\geq E\}$, with $\inf\varnothing=\infty$. This implements a [hazard function](../../../../hazard-function.md) along the [flow of a vector field](../../../../flow-of-a-vector-field.md), rather than a fixed exponential holding time at the last reset. Its [survival probability](../../../../survival-probability.md) and jump-time [probability density function](../../../../probability-density-function.md) are

$$
S(u)=\mathbb P_{s,x}(\tau>u)=e^{-H(u)},\qquad
-\partial_u S(u)=\alpha(z(u))e^{-H(u)}.
$$

Equivalently, $S'=-\alpha(z)S$ with $S(s)=1$. On $\{\tau>t\}$, the terminal state is $z(t)$. Conditional on $\tau=u$, draw the new state $y$ from $K_u(z(u),dy)$ and restart the same construction from $(u,y)$. The [Markov property](../../../../markov-property.md) and the [tower property of conditional expectation](../../../../law-of-total-expectation.md) therefore give the [first-jump decomposition of a piecewise-deterministic Markov process](../../../../first-jump-decomposition-of-a-piecewise-deterministic-markov-process.md)

$$
\boxed{\begin{aligned}
(P_{s,t}f)(x)
&=e^{-H(t)}f(z(t))\\
&\quad+\int_s^t\alpha(z(u))e^{-H(u)}
\int_{\mathbb R}(P_{u,t}f)(y)K_u(z(u),dy)\,du.
\end{aligned}}
$$

This proves the requested identity under the corrected construction, for every bounded [Borel measurable function](../../../../borel-measurable-function.md) $f$. The two contributions partition according to whether the first jump occurs before $t$; later jumps are already contained in $P_{u,t}$.

For comparison, the literal construction does have a different renewal identity when started at a reset with $X_s=Y_s=x$. If $Q_{s,t}$ denotes only these reset-start operators, the same [conditional expectation](../../../../conditional-expectation.md) argument gives

$$
(Q_{s,t}f)(x)=e^{-\alpha(x)(t-s)}f(\varphi(s,x,t))
+\int_s^t\alpha(x)e^{-\alpha(x)(u-s)}(K_uQ_{u,t}f)(x)\,du.
$$

These $Q_{s,t}$ need not be the [transition operators](../../../../transition-operator.md) conditional on $X_s=x$ at an arbitrary time: that observation does not specify the hidden reset state. This distinction explains exactly why replacing only the between-jump paths is insufficient.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the stochastic analysis and partial differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic analysis and partial differential equations course of the University of Oxford](../../../../stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
