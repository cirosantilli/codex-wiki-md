<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The identity for the [killed deterministic flow](../../../../../killed-deterministic-flow.md) follows directly from the [chain rule](../../../../../chain-rule.md) and the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md), independently of the construction issue in part (b). For a continuously differentiable $f$, put $z(t)=\varphi(s,x,t)$ and $H(t)=\int_s^t\alpha(\varphi(s,x,u))\,du$. Then

$$
\begin{aligned}
\partial_t(P^\alpha_{s,t}f)(x)
&=e^{-H(t)}\bigl[f'(z(t))\partial_tz(t)-\alpha(z(t))f(z(t))\bigr]\\
&=e^{-H(t)}\bigl[a(t,z(t))f'(z(t))-\alpha(z(t))f(z(t))\bigr]\\
&=(P^\alpha_{s,t}L_t^\alpha f)(x).
\end{aligned}
$$

Hence, on such [test functions](../../../../../test-function.md),

$$
\boxed{\partial_tP^\alpha_{s,t}=P^\alpha_{s,t}L_t^\alpha,\qquad
L_t^\alpha f=a(t,\cdot)f'-\alpha f.}
$$

The time subscript on $L_t^\alpha$ is necessary because the [vector field](../../../../../vector-field.md) may depend on time; it is suppressed on the right-hand side of the source's displayed operator identity. The [killed deterministic flow](../../../../../killed-deterministic-flow.md) transports an observable along the [flow of a vector field](../../../../../flow-of-a-vector-field.md) and multiplies it by the no-jump [survival probability](../../../../../survival-probability.md).

## ↑ Ancestors (13)

1. [I](../i.md)
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
