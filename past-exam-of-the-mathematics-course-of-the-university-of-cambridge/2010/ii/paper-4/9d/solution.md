<h1 id="9d/solution">Solution</h1>

↑ **Parent:** [9D](../9d.md)

For an autonomous [Lagrangian](../../../../../lagrangian.md), the [canonical momentum](../../../../../canonical-momentum.md) and [energy](../../../../../energy.md) are

$$
p=L_{\dot q},\qquad E=p\dot q-L.
$$

Along a solution of the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md),

$$
\frac{dE}{dt}
=(\dot p-L_q)\dot q-L_t=0.
$$

The absence of explicit time dependence is essential to this conservation law.

The classical [action](../../../../../action.md) is $S_c(q_I,q_F,T)=\int_0^TL(q_c,\dot q_c)\,dt$. If the final endpoint is moved along one fixed classical trajectory, while the initial endpoint is held fixed, the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) gives

$$
\frac{dS_c}{dT}=L(q_c(T),\dot q_c(T)).
$$

This total derivative is different from the partial derivative with fixed final position.

For a family of nearby classical trajectories, integration by parts gives the endpoint variation

$$
\delta S_c=\int_0^T(L_q-\dot p)\delta q\,dt+
p_F\delta q_F-p_I\delta q_I+(L_F-p_F\dot q_F)\delta T.
$$

To obtain the final term, the endpoint change in the variation at fixed parameter time is $\delta q(T)=\delta q_F-\dot q_F\delta T$, while the changing upper integration limit contributes $L_F\delta T$. The interior integral vanishes by the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md). Therefore, on any smooth branch of classical boundary-value solutions,

$$
\boxed{\frac{\partial S_c}{\partial q_F}=p_F,\qquad
\frac{\partial S_c}{\partial q_I}=-p_I,\qquad
\frac{\partial S_c}{\partial T}=-E.}
$$

The chain rule along the endpoint trajectory now reads $dS_c/dT=p_F\dot q_F-E=L_F$, consistently with the direct calculation.

## ↑ Ancestors (10)

1. [9D](../9d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
