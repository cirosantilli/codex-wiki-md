# Strict Jensen equality criterion

↑ **Parent:** [Jensen's inequality](jensen-s-inequality.md)

Let $X$ be an [integrable random variable](integrable-random-variable.md) taking values in an open [interval](interval-mathematics.md) $I$. Suppose $f:I\to\mathbb R$ is a differentiable [strictly convex function](strictly-convex-function.md). Then its [expected value](expected-value-split.md) has equality in [Jensen's inequality](jensen-s-inequality.md) exactly when $X$ is constant [almost surely](almost-sure-convergence.md).

First $m=\mathbb EX$ lies in $I$: at each finite endpoint, taking the [expected value](expected-value-split.md) of the strictly positive distance to that endpoint gives a strictly positive distance for $m$. A tangent [affine function](affine-function.md) supports $f$ at $m$, so

$$
h(t)=f(t)-f(m)-f'(m)(t-m)\geq0.
$$

Strict [convexity](convex-function.md) forces $h(t)>0$ for $t\ne m$. Indeed, equality at another point would force the graph to coincide with its supporting line on the connecting [line segment](line-segment.md), contradicting strict [convexity](convex-function.md). Therefore

$$
\mathbb E[f(X)]-f(m)=\mathbb E[h(X)]\geq0,
$$

and the right side is zero exactly when $X=m$ [almost surely](almost-sure-convergence.md).

The tangent [affine function](affine-function.md) of $X$ is an [integrable random variable](integrable-random-variable.md), so $f(X)$ has an [integrable](integrability.md) [negative part](negative-part-of-a-real-valued-function.md). Thus $\mathbb E[f(X)]$ is well defined, possibly $+\infty$, even if absolute [integrability](integrability.md) was not assumed. Equality to $f(m)$ automatically excludes that infinite case.

## ↑ Ancestors (7)

1. [Jensen's inequality](jensen-s-inequality.md)
2. [Convex function](convex-function.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-probability-measure-and-martingales-course-of-the-university-of-oxford/2021/2/a/solution.md)
- [Solution](past-exam-of-the-probability-measure-and-martingales-course-of-the-university-of-oxford/2021/2/c/i/solution.md)
