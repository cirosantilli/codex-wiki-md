<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove the [symmetric derivative criterion for monotonicity](../../../../../../../symmetric-derivative-criterion-for-monotonicity.md) using an [antiderivative](../../../../../../../antiderivative.md). Fix $a<u<v<b$ and define

$$
F(t)=\int_u^t f(s)\,ds.
$$

The [fundamental theorem of calculus](../../../../../../../fundamental-theorem-of-calculus.md) gives $F'=f$ because $f$ is [continuous](../../../../../../../continuous-function.md). For each interior $x$,

$$
F(x+h)-2F(x)+F(x-h)=\int_0^h\bigl(f(x+t)-f(x-t)\bigr)\,dt.
$$

Since $f^s(x)>0$, the definition of [symmetric derivative](../../../../../../../symmetric-derivative.md) gives $\delta>0$ such that $f(x+t)-f(x-t)>t f^s(x)$ for $0<t<\delta$. Therefore, for $0<h<\delta$,

$$
F(x+h)-2F(x)+F(x-h)>\frac12 f^s(x)h^2>0.
$$

We next show that $F$ is a [convex function](../../../../../../../convex-function.md). On any closed [interval](../../../../../../../interval-mathematics.md) $[r,s]\subset(a,b)$ let $\ell$ be the [affine function](../../../../../../../affine-function.md) joining $(r,F(r))$ to $(s,F(s))$. If $F-\ell$ were positive anywhere, the [extreme value theorem](../../../../../../../extreme-value-theorem.md) would give a positive [maximum](../../../../../../../maximum-of-a-subset-of-a-total-order.md) at an interior point $x$. For every sufficiently small $h>0$, that [maximum](../../../../../../../maximum-of-a-subset-of-a-total-order.md) would imply

$$
(F-\ell)(x+h)-2(F-\ell)(x)+(F-\ell)(x-h)\leq0.
$$

The [affine function](../../../../../../../affine-function.md) contributes zero to this symmetric difference, contradicting the strict positive [inequality](../../../../../../../inequality-mathematics.md) above. Thus $F\leq\ell$ on every such [interval](../../../../../../../interval-mathematics.md), exactly [convexity](../../../../../../../convex-function.md).

For a [differentiable](../../../../../../../differentiable-function.md) [convex function](../../../../../../../convex-function.md), secant slopes bound endpoint [derivatives](../../../../../../../derivative.md). Explicitly, the chord [inequality](../../../../../../../inequality-mathematics.md) at $u+h$ and at $v-h$, followed by $h\downarrow0$, gives

$$
f(u)=F'(u)\leq\frac{F(v)-F(u)}{v-u}\leq F'(v)=f(v).
$$

So $f$ is [nondecreasing](../../../../../../../nondecreasing-function.md). If $f(u)=f(v)$ for some $u<v$, [monotonicity](../../../../../../../monotonic-function.md) would make $f$ constant on $[u,v]$, forcing $f^s(x)=0$ for $u<x<v$, a contradiction. Consequently $\boxed{f(u)<f(v)\text{ for every }u<v}$: $f$ is [strictly increasing](../../../../../../../strictly-increasing-function.md). This proof requires no [continuity](../../../../../../../continuous-function.md) of $f^s$ and never applies the ordinary [mean value theorem](../../../../../../../mean-value-theorem.md) to a merely symmetrically [differentiable](../../../../../../../differentiable-function.md) [function](../../../../../../../function-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
