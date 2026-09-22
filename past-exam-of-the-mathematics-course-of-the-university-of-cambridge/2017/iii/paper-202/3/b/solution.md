<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Tanaka equation](../../../../../../tanaka-equation.md) is an example:

$$
\boxed{dX_t=s(X_t)\,dB_t,\quad X_0=0,\qquad s(x)=\begin{cases}1&x\geq0,\\-1&x<0.\end{cases}}
$$

It has [weak solutions](../../../../../../weak-solution.md) and [uniqueness in law](../../../../../../uniqueness-in-law.md), but lacks [pathwise uniqueness](../../../../../../pathwise-uniqueness.md). The value $s(0)=1$ is deliberate: using the [sign function](../../../../../../sign-function.md) with value zero at zero would admit the identically zero solution and would change the example.

For a quick verification, take a [Brownian motion](../../../../../../brownian-motion-split.md) $W$ and put $B=\int s(W)dW$. Its [quadratic variation](../../../../../../quadratic-variation.md) is $t$, so it is a [Brownian motion](../../../../../../brownian-motion-split.md) by the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md), and [associativity of stochastic integration](../../../../../../associativity-of-stochastic-integration.md) gives $W=\int s(W)dB$. Every [weak solution](../../../../../../weak-solution.md) likewise has [quadratic variation](../../../../../../quadratic-variation.md) $t$ and therefore the law of [Brownian motion](../../../../../../brownian-motion-split.md). On this same enlarged [filtration](../../../../../../filtration-probability-theory.md), both $W$ and $-W$ solve the equation driven by $B$: $s(-W)=-s(W)$ away from zero, and the [Brownian zero set](../../../../../../brownian-zero-set.md) has zero time measure, so the discrepancy at zero contributes nothing to the [Itô integral](../../../../../../ito-integral.md). These solutions differ with positive probability at any positive time. This proves the claimed distinction without relying on a choice of zero convention left unstated.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
