<h1 id="6c/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On times $\tau\gg\epsilon$, the [quasi-steady-state approximation](../../../../../../quasi-steady-state-approximation.md) sets

$$
g_1=g_2=0.
$$

The second equation gives

$$
v_2=\frac{\beta}{\gamma}uv_1.
$$

In the first equation the terms $-\beta uv_1+\gamma v_2$ then cancel, leaving

$$
u(1-v_1-v_2)=\alpha v_1.
$$

Solving these two equations gives

$$
v_1=\frac{u}{\alpha+u+(\beta/\gamma)u^2},
\qquad
v_2=\frac{(\beta/\gamma)u^2}
{\alpha+u+(\beta/\gamma)u^2}.
$$

Since $\dot p=k_3c_2=k_3e_0v_2$,

$$
\boxed{
\frac{dp}{dt}
=A\frac{u^2}{\alpha+u+(\beta/\gamma)u^2},
\qquad
A=\frac{k_3e_0\beta}{\gamma}=k_2e_0s_0
}.
$$

At small substrate concentration this allosteric rate is quadratic, $dp/dt\sim(A/\alpha)u^2$, so its graph leaves the origin with zero slope. At large $u$ it saturates at $A\gamma/\beta=k_3e_0$. A [Michaelis-Menten equation](../../../../../../michaelis-menten-equation.md) also saturates, but its rate $V_{\max}u/(K_M+u)$ is linear near the origin. The allosteric curve is therefore more sigmoidal:

$$
\begin{array}{c|cc}
&u\to0&u\to\infty\\ \hline
\text{allosteric}&O(u^2)&k_3e_0\\
\text{Michaelis--Menten}&O(u)&V_{\max}
\end{array}
$$

This is the [quasi-steady rate law for a two-substrate allosteric enzyme](../../../../../../quasi-steady-rate-law-for-a-two-substrate-allosteric-enzyme.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6C](../../6c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
