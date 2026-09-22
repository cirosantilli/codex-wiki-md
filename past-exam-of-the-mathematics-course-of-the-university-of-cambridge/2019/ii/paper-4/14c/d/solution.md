<h1 id="14c/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Uniform per-capita culling subtracts $kS$ and $kI$ from the two equations:

$$
\boxed{
\begin{aligned}
\dot S&=(S+I)-(S+I)S-\beta IS-kS,\\
\dot I&=-(S+I)I+\beta IS-kI.
\end{aligned}}
$$

Adding and again differentiating $\theta=I/N$ gives the [Uniform per-capita culling in the plant SI model](../../../../../../uniform-per-capita-culling-in-the-plant-si-model.md) equations

$$
\boxed{
\dot N=N(1-k-N),
\qquad
\dot\theta=\theta\{\beta N(1-\theta)-1\}.}
$$

The direct culling terms cancel from the prevalence equation because both classes are culled equally, but culling lowers the eventual total population. For $0\leq k<1$, $N(t)\to1-k$, and a rare infection grows precisely when

$$
\beta(1-k)>1.
$$

Therefore, when $\beta>1$, disease is eliminated while a positive plant population remains exactly for

$$
\boxed{1-\frac1\beta<k<1.}
$$

For $\beta\leq1$ the disease already dies out without culling. If $k\geq1$, culling drives the entire plant population to extinction, which removes the disease only by removing its host.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [14C](../../14c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
