<h1 id="3/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $X(t,a)=X(t;0,a)$ and $A(t,x)=X(0;t,x)$. If $u_0\in C^1(\mathbb R^d)$, the unique global [classical solution](../../../../../../../classical-solution.md) is

$$
\boxed{u(t,x)=u_0(A(t,x)).}
$$

It is $C^1$, and the [chain rule](../../../../../../../chain-rule.md) makes its value constant along every [characteristic curve](../../../../../../../characteristic-curve.md). The same calculation proves classical uniqueness. No boundedness of $u_0$ is needed for this classical statement.

For $u_0\in L^\infty$, a bounded [weak solution](../../../../../../../weak-solution.md) on the positive half-line is defined by

$$
\int_0^\infty\!\int_{\mathbb R^d}u\bigl[\varphi_t+\operatorname{div}_x(F\varphi)\bigr]dx\,dt+\int_{\mathbb R^d}u_0(x)\varphi(0,x)dx=0
$$

for every compactly supported $C^1$ [test function](../../../../../../../test-function.md) on $[0,\infty)\times\mathbb R^d$. The analogous backward-time identity defines the solution on all real time. The $u\operatorname{div}F$ term is essential: this is transport, not the conservative equation $u_t+\operatorname{div}(Fu)=0$.

The same inverse-flow formula defines the unique weak solution, with $\|u(t)\|_\infty=\|u_0\|_\infty$, equality almost everywhere, and a representative continuous into $L^1$ on each compact spatial set. For a direct uniqueness argument, change variables $x=X(t,a)$ in the weak identity and put $w(t,a)=u(t,X(t,a))$. Using $J_t=(\operatorname{div}F)(t,X)J$ gives

$$
\int w\partial_t(J\zeta)\,da\,dt+\int u_0(a)\zeta(0,a)da=0,
$$

initially for $C^1$ compactly supported $\zeta$. Since $J>0$ and $J,J_t$ are continuous on compact sets, approximation in the spatial parameter permits $\zeta=\eta/J$: both $\zeta$ and $\zeta_t$ are uniformly approximable there, which are the only [derivatives](../../../../../../../derivative.md) left in this identity. Hence $\int w\eta_t+\int u_0\eta(0)=0$ and $w=u_0$ almost everywhere. This also verifies existence by reversing the argument, and avoids assuming second [derivatives](../../../../../../../derivative.md) of the $C^1$ field. Local $L^1$ continuity follows by approximating $u_0$ by continuous functions on compact flow tubes.

This is the [weak transport solution under characteristic coordinates](../../../../../../../weak-transport-solution-under-characteristic-coordinates.md). The [weak-strong uniqueness principle](../../../../../../../weak-strong-uniqueness-principle.md) says that a weak solution in the specified class agrees with a classical solution having the same data for as long as that classical solution exists. Here it holds globally in the bounded class whenever the classical initial data are also bounded.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [3](../../../3.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
