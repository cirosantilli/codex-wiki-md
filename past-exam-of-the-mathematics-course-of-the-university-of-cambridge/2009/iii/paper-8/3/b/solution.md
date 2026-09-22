<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\langle k\rangle=(1+|k|^2)^{1/2}$. There are $O(2^{jn})$ lattice points in the dyadic shell $2^j\leq|m|<2^{j+1}$, while each contributes at most a constant times $2^{-2js}$. The geometric series $\sum_j2^{j(n-2s)}$ converges when $2s>n$, proving $\sum_m\langle m\rangle^{-2s}<\infty$. For $|\alpha|\leq k$ and $u\in H_{s+k}$, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) yields

$$
\sum_m|m^\alpha\widehat u(m)|
\leq\left(\sum_m\langle m\rangle^{-2s}\right)^{1/2}
\left(\sum_m\langle m\rangle^{2s}|m^\alpha|^2|\widehat u(m)|^2\right)^{1/2}
\leq C_s\|u\|_{s+k}.
$$

Thus every derivative [Fourier series](../../../../../../fourier-series-split.md) through order $k$ converges absolutely and uniformly. Starting with the continuous sum for $u$, uniform convergence of successive derivative series justifies differentiation, so these are its continuous classical derivatives. **$\boxed{H_{s+k}(\mathbb T^n)\hookrightarrow C^k(\mathbb T^n),\ s>n/2}$**, with a continuous norm bound.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
