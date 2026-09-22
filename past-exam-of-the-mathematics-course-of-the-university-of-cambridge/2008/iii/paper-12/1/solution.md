<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Choose $0<R<R_1$, $0<S<S_1$ and $0<T<T_1$. On this smaller closed [polydisc](../../../../../polydisc.md), the [holomorphic function](../../../../../holomorphic-function.md) $A$ and its $w$-[derivative](../../../../../derivative.md) are bounded; write $|A|\le M$ and $|\partial_w A|\le L$. Choose $0<r<R$ with $rM<S/2$ and $rL<1$, replacing a zero bound by any positive upper bound if necessary, and choose $0<\varepsilon<T$.

Consider functions $u(z,\alpha)$ continuous on $\overline{D(0,r)}\times\overline{D(0,\varepsilon)}$, jointly [holomorphic](../../../../../complex-differentiability-at-a-point.md) in the interior, with $u(0,\alpha)=0$ and $\|u\|_\infty\le S/2$. This is a closed subset of a [Banach space](../../../../../banach-space-split.md) in the supremum [norm](../../../../../norm.md). The integral operator

$$
(\mathcal Tu)(z,\alpha)=\int_0^z A(\zeta,u(\zeta,\alpha),\alpha)\,d\zeta
$$

is well defined on the straight segment and is jointly [holomorphic](../../../../../complex-differentiability-at-a-point.md). Indeed, it equals $z\int_0^1 A(tz,u(tz,\alpha),\alpha)\,dt$, an integral of jointly [holomorphic functions](../../../../../holomorphic-function.md) locally uniformly bounded in both variables. Convexity of the $w$-disc and the [derivative](../../../../../derivative.md) bound give

$$
\|\mathcal Tu\|_\infty\le rM<S/2,\qquad
\|\mathcal Tu-\mathcal Tv\|_\infty\le rL\|u-v\|_\infty.
$$

Thus the [Banach fixed-point theorem](../../../../../contraction-mapping-theorem.md) gives a fixed point $f(z,\alpha)$. More explicitly, the successive integral iterates starting from zero converge uniformly, and [locally uniform convergence of holomorphic functions](../../../../../locally-uniform-convergence-of-holomorphic-functions.md) makes their limit jointly [holomorphic](../../../../../complex-differentiability-at-a-point.md). Differentiating the integral equation gives the required [complex ordinary differential equation](../../../../../complex-ordinary-differential-equation.md) and initial value. This proves **local existence, uniqueness and joint holomorphic dependence on $(z,\alpha)$**. Uniqueness among arbitrary local solutions follows first on a small disc where their values stay within $|w|<S$, by the same [contraction mapping](../../../../../contraction-mapping.md) estimate, and then throughout their common connected domain by the [identity theorem](../../../../../identity-theorem.md).

For [holomorphic dependence of ordinary differential equations on parameters](../../../../../holomorphic-dependence-of-ordinary-differential-equations-on-parameters.md) in the initial value, fix an admissible initial value $w_*$ and put $u=f-w_0$. The equation becomes

$$
u'=A(z,u+w_0),\qquad u(0)=0.
$$

Its right-hand side is jointly [holomorphic](../../../../../complex-differentiability-at-a-point.md) in $(z,u,w_0)$ near $(0,0,w_*)$. The preceding construction supplies a common disc and a jointly [holomorphic](../../../../../complex-differentiability-at-a-point.md) solution for $w_0$ near $w_*$. Consequently $f=u+w_0$ is jointly [holomorphic](../../../../../complex-differentiability-at-a-point.md) in $z$ and its initial value $w_0$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
