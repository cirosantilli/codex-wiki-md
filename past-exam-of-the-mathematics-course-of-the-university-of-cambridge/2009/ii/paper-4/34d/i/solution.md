<h1 id="34d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take the floor at $z=0$, gas-particle mass $m$, $N$ atoms and box side $L$. The one-particle [Hamiltonian](../../../../../../hamiltonian.md) is $p^2/(2m)+mgz$. With $\beta=1/(k_BT)$ and horizontal area $A=L^2$, the [partition function](../../../../../../canonical-partition-function.md) is

$$
Z_N=\frac1{N!h^{3N}}\left[A\left(\frac{2\pi m}{\beta}\right)^{3/2}\frac{1-e^{-\beta mgL}}{\beta mg}\right]^N.
$$

This follows by independent Gaussian momentum integrals and the elementary height integral. Taking $E=-\partial_\beta\log Z_N$ gives

$$
\boxed{E=N\left(\frac5{2\beta}-\frac{mgL}{e^{\beta mgL}-1}\right).}
$$

For an arbitrarily tall box compared with the gravitational scale height, $L\gg k_BT/(mg)$, the upper-wall correction is negligible and

$$
\boxed{E=\frac52Nk_BT.}
$$

The energy includes gravitational potential relative to the floor; the kinetic part alone is $3Nk_BT/2$. Retaining the finite-height correction also gives the ordinary ideal-gas limit as $g\to0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [34D](../../34d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
