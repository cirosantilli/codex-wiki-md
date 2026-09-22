<h1 id="30k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At the terminal time,

$$
F(W_T)=\mathbb E[x_T^2\mid W_T]
=\widehat x_T^2+V_T,
$$

so $P_T=1$ and $d_T=V_T=1/(T+1)$.

Assume $F(W_t)=P_t\widehat x_t^2+d_t$. Conditional on $W_{t-1}$, the random part of the next [Kalman filter](../../../../../../kalman-filter.md) estimate is $h_t$ times the innovation. Its variance is

$$
h_t^2(V_{t-1}+1)
=\frac{V_{t-1}^2}{V_{t-1}+1}
=V_{t-1}V_t.
$$

Therefore the [Bellman equation](../../../../../../bellman-equation.md) gives

$$
\begin{aligned}
F(W_{t-1})
&=\inf_{u_{t-1}}
\left\{u_{t-1}^2
+P_t\mathbb E[\widehat x_t^2\mid W_{t-1}]
+d_t\right\}\\
&=\inf_u\left\{
u^2+P_t(\widehat x_{t-1}+u)^2
+P_tV_{t-1}V_t+d_t\right\}.
\end{aligned}
$$

Completing the square gives

$$
P_{t-1}=\frac{P_t}{1+P_t},
\qquad
d_{t-1}=P_tV_{t-1}V_t+d_t.
$$

Starting from $P_T=1$ yields

$$
\boxed{P_t=\frac1{T-t+1}},
$$

and hence

$$
\boxed{F(W_t)=P_t\widehat x_t^2+d_t,\quad
d_T=\frac1{T+1},\quad
d_{t-1}=V_{t-1}V_tP_t+d_t.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30K](../../30k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
