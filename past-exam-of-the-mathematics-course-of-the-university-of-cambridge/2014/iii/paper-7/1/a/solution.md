<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [characteristic equations for a transport equation](../../../../../../characteristic-equations-for-a-transport-equation.md) are $\dot X=V$ and $\dot V=X$, so $\ddot X=X$. For an initial point $(x_0,v_0)$ their solution is

$$
 \binom{X(t)}{V(t)}=A_t\binom{x_0}{v_0},\qquad
 A_t=\begin{pmatrix}\cosh t&\sinh t\\\sinh t&\cosh t\end{pmatrix}.
$$

This is the [hyperbolic characteristic flow for an inverted oscillator](../../../../../../hyperbolic-characteristic-flow-for-an-inverted-oscillator.md). The addition formulas give $A_sA_t=A_{s+t}$ and $A_t^{-1}=A_{-t}$. In particular, the backward [characteristic flow map](../../../../../../characteristic-flow-map.md) from the point $(x,v)$ at time $t$ to time $s$ is

$$
 S_{s,t}(x,v)=\bigl(x\cosh(t-s)-v\sinh(t-s),\ v\cosh(t-s)-x\sinh(t-s)\bigr).
$$

Along this [characteristic curve](../../../../../../characteristic-curve.md), the [chain rule](../../../../../../chain-rule.md) changes the transport equation into $d[f(s,S_{s,t}(x,v))]/ds=h(s,S_{s,t}(x,v))$. Integrating from zero to $t$ gives

$$
 \boxed{f(t,x,v)=f_0(S_{0,t}(x,v))+\int_0^t h(s,S_{s,t}(x,v))\,ds.}
$$

The assumed $C^1$ regularity makes this a classical solution: on every compact set, the integrand and its needed derivatives are continuous, so differentiation under the finite-time [integral](../../../../../../integral.md) is justified. At $t=0$ it has the required initial value, and the characteristic calculation verifies the equation. Conversely every classical solution must satisfy the same integrated identity, proving uniqueness. This is the [Duhamel formula for Hamiltonian transport](../../../../../../duhamel-formula-for-hamiltonian-transport.md), with Hamiltonian $(v^2-x^2)/2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
