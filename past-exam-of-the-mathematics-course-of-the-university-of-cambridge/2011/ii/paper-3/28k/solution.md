<h1 id="28k/solution">Solution</h1>

↑ **Parent:** [28K](../28k.md)

The stage cost is $(x+u)^2+6u^2\geq0$. The finite-horizon [Bellman equation](../../../../../bellman-equation.md) is

$$
C_s(x)=\inf_u\{x^2+2xu+7u^2+C_{s-1}(x+u)\},\qquad C_0(x)=0.
$$

Inductively write $C_{s-1}(x)=\Pi_{s-1}x^2$. Completing the square in $u$ gives the unique optimal first control

$$
u=-\frac{1+\Pi_{s-1}}{7+\Pi_{s-1}}x,
$$

and

$$
\boxed{C_s(x)=\Pi_sx^2,\qquad \Pi_s=\frac{6(1+\Pi_{s-1})}{7+\Pi_{s-1}},\quad\Pi_0=0.}
$$

For $0\leq q<2$, the recurrence map $F(q)$ satisfies $F(q)<2$ and

$$
F(q)-q=\frac{(2-q)(q+3)}{q+7}>0.
$$

Thus $\Pi_s$ increases and is bounded above by two. Its limit solves $L=6(1+L)/(7+L)$, or $(L-2)(L+3)=0$; nonnegativity forces $L=2$. In particular $C_\infty(x_0)\geq2x_0^2$, and indeed this recurrence already identifies the limit.

For the proposed policy, induction on the state equation gives $x_t=(2/3)^tx_0$ and $u_t=-x_t/3$. The stage cost is $(10/9)x_t^2$, so the infinite [geometric series](../../../../../geometric-series.md) gives

$$
\sum_{t=0}^\infty\frac{10}{9}\left(\frac49\right)^tx_0^2=2x_0^2.
$$

This supplies an admissible policy attaining the lower bound:

$$
\boxed{C_\infty(x_0)=2x_0^2,\qquad u_t=-x_t/3.}
$$

The last formula is the requested [closed-loop control](../../../../../closed-loop-control.md): it uses the observed current state rather than an initial-state schedule.

## ↑ Ancestors (10)

1. [28K](../28k.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
