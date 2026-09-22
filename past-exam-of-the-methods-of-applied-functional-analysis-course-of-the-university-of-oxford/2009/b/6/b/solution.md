<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [log-cosh energy on a Sobolev space](../../../../../log-cosh-energy-on-a-sobolev-space.md), the elementary inequalities $0\le\log\cosh t\le t^2/2$ follow by integrating $|\tanh t|\le|t|$ from zero. Thus

$$
0\le I(v)\le\tfrac12(\|\nabla v\|_2^2+\|v\|_2^2)<\infty,
$$

so the energy is well-defined on $H^1$. For a fixed $v$, its proposed [derivative](../../../../../derivative.md) is linear in the direction $h$ and [bounded](../../../../../boundedness.md), because $|\tanh v|\le|v|$ gives

$$
|\partial_h I(v)|\le\|\nabla v\|_2\|\nabla h\|_2+\|v\|_2\|h\|_2\le\|v\|_{H^1}\|h\|_{H^1}.
$$

To justify differentiation, use $(\log\cosh t)''=\operatorname{sech}^2t\in(0,1]$. Taylor's [integral](../../../../../integral-split.md) remainder [pointwise](../../../../../pointwise-convergence.md), combined with the exact quadratic [gradient](../../../../../gradient.md) expansion, gives

$$
0\le I(v+h)-I(v)-\int_\Omega(\nabla v\cdot\nabla h+\tanh(v)h)\,dx
\le\tfrac12\|h\|_{H^1}^2.
$$

Every term is integrable by the displayed bounds. The remainder is quadratic in the [norm](../../../../../norm.md), so the [functional](../../../../../functional.md) is even [Fréchet differentiable](../../../../../frechet-derivative.md), and in particular [Gâteaux differentiable](../../../../../gateaux-derivative.md) with the required [derivative](../../../../../derivative.md). This also proves that $A(v)$ belongs to the stated [dual space](../../../../../dual-space-split.md).

For $v,w\in H^1$,

$$
\langle A(v)-A(w),v-w\rangle=\|\nabla(v-w)\|_2^2+
\int_\Omega[\tanh v-\tanh w](v-w)\,dx.
$$

Both terms are nonnegative, and the integrand in the second is strictly positive wherever $v\ne w$, since $\tanh$ is strictly increasing. Distinct [Sobolev elements](../../../../../sobolev-space-split.md) differ on a [set](../../../../../set-split.md) of positive measure, so the expression is positive. Hence **$A$ is strictly monotone**.

This gives [strict monotonicity without coercivity on H1](../../../../../strict-monotonicity-without-coercivity-on-h1.md): it is **not coercive on $H^1$**. For [constant functions](../../../../../constant-function.md) $v_t=t$ with $t\to+\infty$, the [norm](../../../../../norm.md) is $t|\Omega|^{1/2}$ and

$$
\frac{\langle A(v_t),v_t\rangle}{\|v_t\|_{H^1}}=|\Omega|^{1/2}\tanh t\longrightarrow|\Omega|^{1/2},
$$

which is finite. In contrast it **is coercive on $H_0^1$**: if $\|v\|_2\le C_P\|\nabla v\|_2$, then

$$
\langle A(v),v\rangle=\|\nabla v\|_2^2+\int_\Omega v\tanh v\,dx
\ge\frac{\|v\|_{H^1}^2}{1+C_P^2}.
$$

Dividing by the [norm](../../../../../norm.md) proves growth to [infinity](../../../../../infinity.md). On this smaller space the operator is understood by restricting its [dual action](../../../../../dual-pairing.md) to [zero-trace](../../../../../zero-boundary-sobolev-space.md) [test functions](../../../../../test-function.md). Removing the constant directions by the [boundary condition](../../../../../boundary-condition.md) is what restores coercivity.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
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
