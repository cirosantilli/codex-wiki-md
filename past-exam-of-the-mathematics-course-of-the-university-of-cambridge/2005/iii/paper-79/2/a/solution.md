<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The factorial tail provides the connection with the supplied [Borel summation](../../../../../../borel-summation.md) formula. Near the first switching line choose $\lambda=-z^3$ with $\arg\lambda=3(\arg z-\pi/3)$, so $\lambda$ is near the positive real axis and $\lambda^{-1/3}=e^{i\pi/3}/z$. The endpoint contribution through $N-1$ terms is

$$
P_N(z)=\frac{e^\lambda}{3\lambda\Gamma(2/3)}\sum_{r=0}^{N-1}\frac{\Gamma(r+2/3)}{\lambda^r}.
$$

Writing $r=N+p$ in its formal remainder, with $\gamma=N+2/3$, gives

$$
\frac{\lambda^{-1/3}}{3\Gamma(2/3)}\sum_{p\geq0}\frac{\Gamma(\gamma+p)e^\lambda}{\lambda^{p+\gamma}}.
$$

Thus the [Borel remainder for a cubic exponential integral](../../../../../../borel-remainder-for-a-cubic-exponential-integral.md), using the contour just above the pole specified in the paper, is

$$
\boxed{G(z)-P_N(z)=\frac C z+\frac{e^{i\pi/3}}{3\Gamma(2/3)z}I(\lambda,\gamma).}
$$

The continuation is chosen from the sector below the switching line. The term $C/z$ fixes that continuation; an alternative lateral pole contour would shift it by the corresponding residue. This is why the contour prescription must accompany the divergent factorial series.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

## ← Incoming links (2)

- [Solution](../b/solution.md)
- [Solution](../solution.md)
