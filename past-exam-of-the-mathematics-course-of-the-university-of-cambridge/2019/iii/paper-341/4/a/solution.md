<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Keep the [Courant number](../../../../../../courant-number.md) $\mu=\Delta t/\Delta x$ fixed and write $h=\Delta x$. An exact solution of $u_t=u_x$ is $u(x,t)=g(x+t)$. Substituting it into the update gives the defect

$$
g(s+\mu h)-(1-2\mu)\{g(s)-g(s+h)\}-g(s+(1-\mu)h)
=\frac{\mu(1-\mu)(1-2\mu)}6h^3g^{(3)} + O(h^4),
$$

where $s=x+t$ and $g^{(3)}$ is evaluated at $s$. The constant, first-derivative and second-derivative terms cancel. Dividing by $\Delta t=\mu h$ gives a second-order consistency error. Hence for fixed $0<\mu<1$, $\mu\ne1/2$, the scheme has **order two**.

At the special value $\mu=1/2$, the update reduces to $u_m^{n+1}=u_{m+1}^{n-1}$. This is exactly the transport over two time steps, since $2\Delta t=\Delta x$, so the defect vanishes identically. With exact data at both starting levels it transports their values exactly; errors in those starting levels are still present, and the even and odd time subsequences evolve separately.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
