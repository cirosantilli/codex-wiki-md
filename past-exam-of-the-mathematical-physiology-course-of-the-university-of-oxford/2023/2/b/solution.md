<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the three standard reduction assumptions: $m$ relaxes much faster than $V,n,h$ and can be replaced by $m_\infty(V)$; the two slower gates have the same [time constant](../../../../time-constant.md), $\tau_n(V)=\tau_h(V)=\tau(V)$; and their limiting open fractions have a voltage-independent sum, $n_\infty(V)+h_\infty(V)=K$. The constant-sum assumption is essential: equality of two [time constants](../../../../time-constant.md) by itself does not preserve a moving voltage-dependent sum.

For $q=n+h$, addition of the two gate [ordinary differential equations](../../../../ordinary-differential-equation.md) gives

$$
\tau(V)\dot q=K-q.
$$

The specified initial condition is $q(0)=K$. Uniqueness for this [first-order linear differential equation](../../../../first-order-linear-differential-equation.md) gives $q(t)=K$, hence $h=K-n$ for all time. The remaining two [ordinary differential equations](../../../../ordinary-differential-equation.md) are

$$
\boxed{\begin{aligned}
C_m\dot V={}&I_{\mathrm{app}}
-g_{\mathrm{Na}}m_\infty(V)^3(K-n)(V-V_{\mathrm{Na}})
-g_{\mathrm K}n^4(V-V_{\mathrm K})-g_{\mathrm L}(V-V_{\mathrm L}),\\
\tau(V)\dot n={}&n_\infty(V)-n.
\end{aligned}}
$$

These assumptions give a [planar reduction of the Hodgkin-Huxley model](../../../../planar-reduction-of-the-hodgkin-huxley-model.md). The [FitzHugh-Nagumo model](../../../../fitzhugh-nagumo-model.md) keeps its fast activation and slow [recovery variable](../../../../recovery-variable.md) geometry, approximating the voltage response by a [cubic polynomial](../../../../cubic-polynomial.md) and the recovery response by a [linear function](../../../../linear-function.md) after [nondimensionalization](../../../../nondimensionalization.md). The [polynomial](../../../../polynomial-split.md) equations in part (c) are a further model simplification; they are not an exact algebraic consequence of arbitrary original gate functions.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematical physiology course of the University of Oxford](../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
