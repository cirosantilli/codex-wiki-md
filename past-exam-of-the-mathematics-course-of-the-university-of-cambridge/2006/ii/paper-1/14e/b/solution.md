<h1 id="14e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $y=\dot x$ and $E=(x^2+y^2)/2$. Along a trajectory,

$$
\dot E=-\epsilon(\alpha x^2+\beta y^2-\gamma)y^2.
$$

Use the unperturbed orbit $x=R\sin t,y=R\cos t$ to compute the leading energy change over one period:

$$
\Delta E=-\epsilon\pi\left[\frac{\alpha+3\beta}{4}R^4-2\gamma R^2\right]+O(\epsilon^2).
$$

Zero averaged energy change gives the nonzero amplitude

$$
\boxed{R=2\sqrt{\frac{\gamma}{\alpha+3\beta}}+O(\epsilon).}
$$

The supplied sign condition makes this real and nonzero. The averaged [amplitude equation](../../../../../../amplitude-equation.md) is $\dot R=\epsilon[\gamma R/2-(\alpha+3\beta)R^3/8]+O(\epsilon^2)$, whose [derivative](../../../../../../derivative.md) at that root is $-\epsilon\gamma+O(\epsilon^2)$. Its nonzero [derivative](../../../../../../derivative.md) also makes the root persist as an isolated [periodic orbit](../../../../../../periodic-orbit.md) for sufficiently small positive $\epsilon$.

Directly, the planar [divergence](../../../../../../divergence.md) is $-\epsilon(\alpha x^2+3\beta y^2-\gamma)$. On the leading orbit its integral over $2\pi$ is $-\epsilon[\pi R^2(\alpha+3\beta)-2\pi\gamma]=-2\pi\epsilon\gamma$. Thus

$$
\boxed{\mu=\exp[-2\pi\epsilon\gamma+O(\epsilon^2)].}
$$

**The cycle is attracting for $\gamma>0$ and repelling for $\gamma<0$**. Both sign possibilities are allowed by $(\alpha+3\beta)\gamma>0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
