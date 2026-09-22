<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

Put $\theta=T-T_r$ and $u=U-T_r$. The term $-a\theta$ models oven cooling to the room, $Q$ is heater input, and $-bu=b\theta-bu$ makes the pizza relax toward the oven temperature. Both protocols supply unit total heat because $\int\delta(t)\,dt=1$ and the rectangular pulse has height $1/\tau$ and width $\tau$.

For the impulse, $\theta$ jumps by one at zero while $u$ remains continuous:

$$
\boxed{\theta_1(t)=e^{-at},\qquad
u_1(t)=\frac{b}{b-a}(e^{-at}-e^{-bt})}
$$

for $a\ne b$; when $a=b$, $u_1=bte^{-bt}$.

Define causal functions

$$
G_a(t)=H(t)\frac{1-e^{-at}}a,\qquad
K(t)=H(t)\frac{b}{b-a}\left(\frac{1-e^{-at}}a-\frac{1-e^{-bt}}b\right).
$$

The rectangular-pulse solutions are

$$
\boxed{\theta_2(t)=\frac{G_a(t)-G_a(t-\tau)}{\tau},\qquad
u_2(t)=\frac{K(t)-K(t-\tau)}{\tau}.}
$$

Finally $T_i=T_r+\theta_i$, $U_i=T_r+u_i$. These formulas make $T_2,U_2$ continuous at $0,\tau$; only $T_1$ jumps at the delta impulse. As $\tau\to0$, the difference quotients tend to $G_a'=\theta_1$ and $K'=u_1$, because the rectangular pulse is an [approximate identity](../../../../../approximate-identity.md).

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
