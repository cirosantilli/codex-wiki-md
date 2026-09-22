<h1 id="28k/solution">Solution</h1>

↑ **Parent:** [28K](../28k.md)

The stochastic objective is interpreted as its [expectation](../../../../../expected-value.md); a literal pathwise minimization is generally impossible without knowing future noises. Let the value function from time $t$ be $V_t(x)=P_t x^2+d_t$, with $P_T=1,d_T=0$. Independence from past observations and zero contemporaneous [covariance](../../../../../covariance.md) give

$$
 \mathbb E[x_{t+1}^2\mid x_t=x,u_t=u]=V_\xi(Ax+u)^2+V_\epsilon.
$$

The [Bellman equation](../../../../../bellman-equation.md) is $V_t(x)=x^2+\min_u\{cu^2+P_{t+1}V_\xi(Ax+u)^2+P_{t+1}V_\epsilon+d_{t+1}\}$. Completing the square yields

$$
\boxed{u_t^*(x)=-\frac{A V_\xi P_{t+1}}{c+V_\xi P_{t+1}}x,\quad
 P_t=1+\frac{A^2c V_\xi P_{t+1}}{c+V_\xi P_{t+1}},\quad
 d_t=d_{t+1}+P_{t+1}V_\epsilon.}
$$

This feedback is optimal among all controls measurable from the specified past, not merely linear controls. It depends on $V_\xi$ and **does not depend on $V_\epsilon$**, though the minimal cost does. There is no cost-relevant $u_T$ in the displayed objective.

The backward [Riccati recurrence](../../../../../discrete-riccati-recurrence.md) iterates $F(P)=1+A^2cV_\xi P/(c+V_\xi P)$ from $1$. It is increasing, maps into $[1,1+A^2c]$, and has exactly one positive [fixed point](../../../../../fixed-point.md). Consequently it converges to

$$
\boxed{P=\frac{-b+\sqrt{b^2+4cV_\xi}}{2V_\xi},\quad
 b=c-V_\xi-A^2cV_\xi,\qquad
 u^*(x)=-\frac{A V_\xi P}{c+V_\xi P}x.}
$$

As $T\to\infty$, the finite-horizon feedback at any fixed time tends to this feedback. The closed-loop multiplier is $A c/(c+V_\xi P)$, and its squared-mean factor $\alpha=V_\xi A^2c^2/(c+V_\xi P)^2$ is less than one, since $(P-1)/P=A^2cV_\xi/(c+V_\xi P)$ and $\alpha=(P-1)c/[P(c+V_\xi P)]$. Thus the second moment tends to $V_\epsilon/(1-\alpha)$. The finite-horizon value has $d_1=V_\epsilon\sum_{t=1}^{T-1}P_{t+1}$; its average converges by Cesaro summation. For a fixed initial state of finite second moment,

$$
\boxed{\lim_{T\to\infty}\frac1T\inf\mathbb E[\text{total cost}]=P V_\epsilon.}
$$

The same average is attained by the stationary feedback, by the stationary [Bellman equation](../../../../../bellman-equation.md) and bounded second moments.

## ↑ Ancestors (10)

1. [28K](../28k.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
