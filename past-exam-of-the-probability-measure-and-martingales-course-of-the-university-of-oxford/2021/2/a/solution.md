<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $m=\mathbb EX$. First, $m$ lies in the open [interval](../../../../interval-mathematics.md) $I$. For example, if $I$ has a finite lower endpoint $\ell$, then $X-\ell>0$ [almost surely](../../../../almost-sure-convergence.md), and its [expected value](../../../../expected-value-split.md) is strictly positive; hence $m>\ell$. The corresponding argument at a finite upper endpoint gives the other strict inequality. [Integrability](../../../../integrability.md) ensures $m$ is finite when either endpoint is infinite.

The tangent [affine function](../../../../affine-function.md) at $m$ gives the [supporting inequality for a differentiable convex function](../../../../supporting-inequality-for-a-differentiable-convex-function.md). Under the stipulated condition $f''>0$, contact with that tangent occurs only at $m$: define

$$
h(t)=f(t)-f(m)-f'(m)(t-m).
$$

Then $h(m)=0$, and $h(t)>0$ for every $t\ne m$. One direct proof uses $h'(t)=f'(t)-f'(m)$: $f'$ is strictly increasing, so $h$ decreases towards $m$ on the left and increases away from $m$ on the right. Therefore

$$
\mathbb E[f(X)]=f(m)+\mathbb E[h(X)]\geq f(m),
$$

with equality exactly when $h(X)=0$ [almost surely](../../../../almost-sure-convergence.md), equivalently when $X=m$ [almost surely](../../../../almost-sure-convergence.md). Conversely, an [almost surely](../../../../almost-sure-convergence.md) constant $X=m$ plainly gives equality. This proves the [strict Jensen equality criterion](../../../../strict-jensen-equality-criterion.md).

No extra assumption that $f(X)$ is an [integrable random variable](../../../../integrable-random-variable.md) is needed to interpret this argument. Its [negative part](../../../../negative-part-of-a-real-valued-function.md) is bounded by the absolute value of the [integrable random variable](../../../../integrable-random-variable.md) $f(m)+f'(m)(X-m)$, since $h(X)\geq0$. Thus its [expected value](../../../../expected-value-split.md) is defined in $(-\infty,+\infty]$; if it equals the finite number $f(m)$, then $\mathbb E[h(X)]=0$ and the required [integrability](../../../../integrability.md) follows automatically. **Equality holds if and only if $X=\mathbb EX$ almost surely.**

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../split.md)
5. [Probability, measure and martingales course of the University of Oxford](../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
