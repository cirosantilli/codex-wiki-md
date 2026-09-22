<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix a compact $K\subset\Omega$ and choose $\delta>0$ such that a closed $3\delta$-neighbourhood of $K$ is compactly contained in $\Omega$. The hypothesis gives a common bound $M$ on that neighbourhood. Choose a smooth radial [mollifier](../../../../../../mollifier.md) $\rho_\delta$ supported in $B_\delta(0)$ with integral one. The [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md), integrated against its radial weights, gives

$$
u_j(x)=\int\rho_\delta(x-y)u_j(y)\,dy
$$

in a neighbourhood of $K$. Differentiating this fixed-radius convolution gives the uniform interior estimate

$$
|\nabla u_j(x)|\leq M\|\nabla\rho_\delta\|_1\leq C_\rho M/\delta.
$$

Thus the sequence is equicontinuous there; taking its pointwise limit gives the same local modulus of continuity for $u$. A finite small-ball cover of $K$ now proves [uniform convergence](../../../../../../uniform-convergence.md) directly: choose the cover so both $u_j$ and $u$ vary by less than $\varepsilon$ inside each ball, then use convergence at its finitely many centres to make $|u_j-u|<\varepsilon$ there. The [triangle inequality](../../../../../../triangle-inequality.md) gives $\sup_K|u_j-u|<3\varepsilon$ for large $j$.

Finally, pass to the limit in the reproducing convolution identity on smaller compact sets. It yields $u=u*\rho_\delta$, so $u$ is smooth locally. Also, for each compactly supported smooth [test function](../../../../../../test-function.md) $\phi$, uniform convergence on its support gives

$$
\int_\Omega u\Delta\phi=\lim_j\int_\Omega u_j\Delta\phi=0.
$$

Hence its smooth Laplacian is zero. We have proved **$u_j\to u$ uniformly on every compact subset and $u$ is harmonic**. Using the continuous representatives in the pointwise hypothesis makes this conclusion pointwise, rather than only almost everywhere. This is [compact convergence of locally bounded harmonic functions](../../../../../../compact-convergence-of-locally-bounded-harmonic-functions.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
