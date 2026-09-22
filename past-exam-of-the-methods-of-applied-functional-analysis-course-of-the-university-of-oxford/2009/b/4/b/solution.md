<h1 id="b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [weak solution](../../../../../weak-solution.md) belongs to $V=H_0^1(\Omega)$ and satisfies

$$
\boxed{\int_\Omega\nabla u\cdot\nabla h\,dx=\int_\Omega f(u)h\,dx\qquad(h\in V),}
$$

with the nonlinear right-hand side defining a [bounded](../../../../../boundedness.md) [functional](../../../../../functional.md) on $V$. Under the stated global [Lipschitz](../../../../../lipschitz-continuity.md) hypothesis this requirement is automatic: $|f(s)|\le|f(0)|+\epsilon|s|$ and boundedness of $\Omega$ give $f(u)\in L^2$ whenever $u\in V$. [Continuity](../../../../../continuous-function.md) of $f$ alone, without growth control, would not guarantee this for an arbitrary [Sobolev function](../../../../../sobolev-space-split.md).

For the [semilinear Poisson contraction threshold](../../../../../semilinear-poisson-contraction-threshold.md), use the [gradient norm](../../../../../sobolev-norm.md) on $V$, and let $C_P$ satisfy the [Poincaré inequality](../../../../../poincare-inequality.md) $\|v\|_2\le C_P\|\nabla v\|_2$. For $g\in L^2$, Lax-Milgram gives the [zero-Dirichlet](../../../../../dirichlet-boundary-condition.md) Poisson solution $Pg\in V$. Testing with $Pg$ yields $\|\nabla Pg\|_2\le C_P\|g\|_2$. Define $T(v)=P(f(v))$, a self-map of the complete space $V$. For $v,w\in V$,

$$
\|T(v)-T(w)\|_V\le C_P\|f(v)-f(w)\|_2
\le\epsilon C_P^2\|v-w\|_V.
$$

Therefore **$\epsilon C_P^2<1$ is a sufficient condition** for [Banach's theorem](../../../../../contraction-mapping-theorem.md) to give a unique [fixed point](../../../../../fixed-point.md) and hence a unique [weak solution](../../../../../weak-solution.md). There is no need to assume $f(0)=0$ or to restrict to a small ball: the [Lipschitz](../../../../../lipschitz-continuity.md) bound makes the map defined on all of $V$. The same estimates give

$$
\|\nabla u\|_2\le\frac{C_P|\Omega|^{1/2}|f(0)|}{1-\epsilon C_P^2}.
$$

With the optimal [Poincaré](../../../../../poincare-inequality.md) constant, the threshold is $\epsilon<\lambda_1$ for the [First Dirichlet eigenvalue](../../../../../first-dirichlet-eigenvalue.md); the stated sufficient condition does not depend on knowing that optimal constant.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../split.md)
6. [Methods of applied functional analysis course of the University of Oxford](../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
