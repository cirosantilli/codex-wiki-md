# Forward equation of a piecewise-deterministic Markov process

↑ **Parent:** [Piecewise-deterministic Markov process](piecewise-deterministic-markov-process.md)

If the destination [transition kernel](markov-kernel.md) has [probability density function](probability-density-function.md) $m_t(x,y)$, the formal [adjoint operator](adjoint-operator.md) of $L_tf=af'+\alpha(K_tf-f)$ is $(L_t^*p)(x)=-\partial_x(a(t,x)p(x))-\alpha(x)p(x)+\int\alpha(y)m_t(y,x)p(y)dy$. Multiply by a smooth compactly supported [test function](test-function.md), use [integration by parts](integration-by-parts.md) on transport and [Fubini's theorem](fubini-s-theorem.md) on the jump gain to prove the formula when the integrals are finite. The general formulation is $\frac d{dt}\int f\,d\nu_t=\int L_tf\,d\nu_t$ for [probability measures](probability-measure.md) $\nu_t$. A deterministic initial value leaves positive no-jump atomic mass at finite times, so a full smooth density cannot be assumed for that initialization.

## ↑ Ancestors (7)

1. [Piecewise-deterministic Markov process](piecewise-deterministic-markov-process.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford/2025/1/c/ii/solution.md)
