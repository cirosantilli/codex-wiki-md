<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the corrected [piecewise-deterministic Markov process](../../../../../piecewise-deterministic-markov-process.md) from part (b). For a smooth [test function](../../../../../test-function.md) $f$, its time-dependent [infinitesimal generator](../../../../../infinitesimal-generator-stochastic-processes.md) is

$$
(L_tf)(x)=a(t,x)f'(x)+\alpha(x)\left[\int_{\mathbb R}f(y)m_t(x,y)\,dy-f(x)\right].
$$

Indeed, over an interval of length $h$, deterministic motion contributes $ha(t,x)f'(x)$, while a jump has [probability](../../../../../probability.md) $h\alpha(x)+o(h)$ and changes the conditional mean of $f$ by $K_tf(x)-f(x)$. Terms involving both drift and a jump contribute only to the remainder. Thus $P_{t,t+h}f=f+hL_tf+o(h)$.

The [Dynkin formula](../../../../../dynkin-s-formula.md), or this infinitesimal expansion integrated against the current [probability distribution](../../../../../probability-distribution-split.md), gives the weak evolution identity

$$
\frac d{dt}\int_{\mathbb R}f(x)p_t(x)\,dx
=\int_{\mathbb R}(L_tf)(x)p_t(x)\,dx.
$$

Take $f\in C_c^\infty(\mathbb R)$, so [integration by parts](../../../../../integration-by-parts.md) has no boundary contribution. Assuming the displayed jump integrals are finite, [Fubini's theorem](../../../../../fubini-s-theorem.md) gives

$$
\begin{aligned}
\int_{\mathbb R}a(t,x)f'(x)p_t(x)\,dx
&=-\int_{\mathbb R}f(x)\partial_x\bigl(a(t,x)p_t(x)\bigr)\,dx,\\
\int_{\mathbb R}\alpha(y)p_t(y)\int_{\mathbb R}f(x)m_t(y,x)\,dx\,dy
&=\int_{\mathbb R}f(x)\int_{\mathbb R}\alpha(y)m_t(y,x)p_t(y)\,dy\,dx.
\end{aligned}
$$

Consequently the [forward equation of a piecewise-deterministic Markov process](../../../../../forward-equation-of-a-piecewise-deterministic-markov-process.md) is

$$
\boxed{\begin{aligned}
\partial_tp_t(x)=(A_tp_t)(x)
&=-\partial_x\bigl(a(t,x)p_t(x)\bigr)-\alpha(x)p_t(x)\\
&\quad+\int_{\mathbb R}\alpha(y)m_t(y,x)p_t(y)\,dy.
\end{aligned}}
$$

Here $A_t=L_t^*$ is the formal [adjoint operator](../../../../../adjoint-operator.md) acting on [probability density functions](../../../../../probability-density-function.md). Its terms are transport, loss from $x$, and incoming mass from every $y$. In particular, the incoming rate is $\alpha(y)$, evaluated at the departure state. The operator denoted $A$ in the source is generally time-dependent. Because $\int m_t(y,x)\,dx=1$, the gain and loss integrals cancel; with vanishing transport flux at infinity, $\frac d{dt}\int p_t=0$.

**The deterministic initial state in part (b) does not actually yield an everywhere smooth full density.** For finite times the no-jump contribution is the positive measure

$$
\exp\left(-\int_0^t\alpha(\varphi(0,y_0,u))\,du\right)
\delta_{\varphi(0,y_0,t)},
$$

where $\delta_z$ is the [Dirac measure](../../../../../dirac-measure.md) at $z$. Smooth jump destination [probability density functions](../../../../../probability-density-function.md) cannot remove this positive atom. The density equation above is therefore conditional on the extra density hypothesis, for example with a suitable random initial [probability density function](../../../../../probability-density-function.md). For the specified fixed initial state, write $\nu_t$ for the whole [probability measure](../../../../../probability-measure.md) and use instead

$$
\boxed{\frac d{dt}\int f\,d\nu_t=\int L_tf\,d\nu_t,\qquad \nu_0=\delta_{y_0}.}
$$

This weak measure evolution includes both the atom and any continuous component. It becomes the displayed [partial differential equation](../../../../../partial-differential-equation-split.md) whenever $\nu_t(dx)=p_t(x)\,dx$ with the assumed regularity. It does not describe the literal hidden-reset construction without the correction in part (b).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic analysis and partial differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic analysis and partial differential equations course of the University of Oxford](../../../../../stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
