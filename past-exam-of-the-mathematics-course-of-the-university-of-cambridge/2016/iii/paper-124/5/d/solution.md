<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $L=\log\log N$, $h=L^{-1/2}$, and let $F_N$ be the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) of $(\omega-L)/\sqrt L$. Since the [prime omega function](../../../../../../prime-omega-function.md) is integer-valued, $F_N$ is constant on every half-open interval between consecutive points of the lattice $(\mathbb Z-L)/\sqrt L$.

Choose $k=\lfloor L\rfloor$ and put $\alpha=(k-L)/\sqrt L$, $\beta=(k+1-L)/\sqrt L$. Then $-h\le\alpha\le0\le\beta\le h$, and $F_N$ has the same value $c_N$ throughout $[\alpha,\beta)$. The [standard normal distribution function](../../../../../../standard-normal-distribution-function.md) $\Phi$ is continuous, so the definition of the [Kolmogorov distance](../../../../../../kolmogorov-distance.md) gives

$$
E(N)\ge|c_N-\Phi(\alpha)|,\qquad E(N)\ge|c_N-\Phi(\beta)|,
$$

where the second inequality follows by taking a limit from below at $\beta$. The [triangle inequality](../../../../../../triangle-inequality.md) therefore yields

$$
2E(N)\ge\Phi(\beta)-\Phi(\alpha)=\int_\alpha^\beta\frac{e^{-t^2/2}}{\sqrt{2\pi}}\,dt\ge\frac{h e^{-h^2/2}}{\sqrt{2\pi}}.
$$

Thus **the integer lattice forces the lower bound**:

$$
\boxed{E(N)\ge\frac{e^{-1/(2\log\log N)}}{2\sqrt{2\pi\log\log N}}\gg\frac1{\sqrt{\log\log N}}.}
$$

This [lattice obstruction to normal approximation](../../../../../../lattice-obstruction-to-normal-approximation.md) does not require a quantitative [Erdős-Kac theorem](../../../../../../erdos-kac-theorem.md); it follows directly from discreteness and the positive [standard normal density](../../../../../../standard-normal-density.md) near zero.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
