<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

For $s>n/2$ and $u\in H^s(\mathbb R^n)$, Fourier inversion and Cauchy--Schwarz give

$$
|u(x)|\leq C\int|\widehat u(\xi)|\,d\xi
\leq C\left(\int(1+|\xi|^2)^s|\widehat u|^2d\xi\right)^{1/2}
\left(\int(1+|\xi|^2)^{-s}d\xi\right)^{1/2}.
$$

The last [integral](../../../../../integral.md) is finite exactly when $s>n/2$. Thus the [sobolev embedding theorem](../../../../../sobolev-embedding-theorem.md) gives

$$
\|u\|_\infty\leq C_{n,s}\|u\|_{H^s}.
$$

To see why the endpoint relevant to $H^1(\mathbb R^3)$ fails, choose a smooth cutoff $\chi$ supported near the origin and equal to one there, and set

$$
u(x)=\chi(x)|x|^{-1/4}.
$$

Near zero, $|u|^2$ contributes $\int_0^1r^{3/2}dr$, while $|\nabla u|^2$ contributes a constant multiple of $\int_0^1r^{-1/2}dr$. Both are finite, so $u\in H^1(\mathbb R^3)$, but $u$ is unbounded.

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
