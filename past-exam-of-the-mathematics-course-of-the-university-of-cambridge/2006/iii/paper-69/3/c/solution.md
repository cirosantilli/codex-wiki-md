<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Multiply the [Fokker-Planck equation](../../../../../../fokker-planck-equation.md) by $B^n$ and integrate over $B>0$ and all $\sigma$, assuming the required boundary terms vanish. [Integration by parts](../../../../../../integration-by-parts.md) gives

$$
\frac{d}{dt}\mathbb E[B^n]=n\mathbb E[\sigma B^n].
$$

The mixed [moment](../../../../../../moment.md) is not determined by $\mathbb E[B^n]$: the current strain and the accumulated [magnetic field](../../../../../../magnetic-field.md) are correlated. Zero mean strain does not imply $\mathbb E[\sigma B^n]=0$, so this is an unclosed [moment equation](../../../../../../moment-equation.md).

Keep the strain dependence by defining $P_n(\sigma,t)=\int_0^\infty B^nP(B,\sigma,t)\,dB$. The magnetic drift term satisfies

$$
-\int_0^\infty B^n\partial_B(\sigma BP)\,dB=n\sigma P_n.
$$

The strain derivatives commute with the $B$ integral. Hence

$$
\boxed{\partial_tP_n=\frac\kappa2\partial_\sigma^2P_n+\frac1\tau\partial_\sigma(\sigma P_n)+n\sigma P_n.}
$$

This weighted density obeys a tilted [Ornstein-Uhlenbeck Fokker-Planck equation](../../../../../../ornstein-uhlenbeck-fokker-planck-equation.md). Its integral over $\sigma$ is the desired [moment](../../../../../../moment.md), while retaining $\sigma$ makes the evolution closed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
