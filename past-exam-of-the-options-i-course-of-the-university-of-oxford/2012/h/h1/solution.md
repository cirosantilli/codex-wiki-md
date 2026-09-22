<h1 id="h/h1/solution">Solution</h1>

↑ **Parent:** [H1](../h1.md)

Away from a collision, let $r=q_1-q_2$ and $D=|r|>0$. The [Lagrangian](../../../../lagrangian.md) is

$$
\boxed{L=\frac12m_1|\dot q_1|^2+\frac12m_2|\dot q_2|^2-V(D).}
$$

Differentiating $D^2=r\cdot r$ with respect to $x_1$ and $x_2$ gives $2D\partial_{x_1}D=2(x_1-x_2)$ and $2D\partial_{x_2}D=-2(x_1-x_2)$. Therefore

$$
\boxed{\partial_{x_1}D=-\partial_{x_2}D=\frac{x_1-x_2}{D}.}
$$

The other coordinates give $\nabla_{q_1}D=r/D$ and $\nabla_{q_2}D=-r/D$. Substituting these into the [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) yields equal and opposite central forces:

$$
\boxed{m_1\ddot q_1=-\frac{V'(D)}D r,\qquad
m_2\ddot q_2=\frac{V'(D)}D r.}
$$

Adding the equations shows that the [derivative](../../../../derivative.md) of the total [linear momentum](../../../../momentum-split.md) is zero, so $P=m_1\dot q_1+m_2\dot q_2$ is constant. For the total [angular momentum](../../../../angular-momentum.md), the terms $\dot q_i\times\dot q_i$ vanish, giving

$$
\begin{aligned}
\frac d{dt}(m_1q_1\times\dot q_1+m_2q_2\times\dot q_2)
&=q_1\times\left(-\frac{V'}D r\right)+q_2\times\left(\frac{V'}D r\right)\\
&=-\frac{V'}D(q_1-q_2)\times r=0.
\end{aligned}
$$

Thus both stated vectors are [conserved quantities](../../../../conserved-quantity.md).

**The total energy is also constant.** Define $E=\tfrac12m_1|\dot q_1|^2+\tfrac12m_2|\dot q_2|^2+V(D)$. Since $\dot D=r\cdot(\dot q_1-\dot q_2)/D$,

$$
\begin{aligned}
\dot E&=m_1\dot q_1\cdot\ddot q_1+m_2\dot q_2\cdot\ddot q_2+V'\dot D\\
&=-\frac{V'}D r\cdot(\dot q_1-\dot q_2)+V'\frac{r\cdot(\dot q_1-\dot q_2)}D=0.
\end{aligned}
$$

Hence $\boxed{E=T+V(D)\text{ is conserved}}$. The explicit cancellation establishes energy conservation for an arbitrary smooth separation-dependent potential, throughout any collision-free trajectory.

## ↑ Ancestors (12)

1. [H1](../h1.md)
2. [H](../../h.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
