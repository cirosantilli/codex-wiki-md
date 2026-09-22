<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Start with $u\in H_s$ for some real $s$. The equation becomes

$$
(1+\Delta)u=f+(1-V)u.
$$

Smooth $f$ belongs to every [periodic Sobolev space](../../../../../../periodic-sobolev-space.md), and multiplication by the smooth coefficient preserves $H_s$ by part (c), so the right side lies in $H_s$. The Fourier multiplier $(1+\Delta)^{-1}$ has coefficient $(1+|m|^2)^{-1}$ and maps $H_s$ isometrically to $H_{s+2}$. Thus $u\in H_{s+2}$. Repeat this argument to get $u\in H_{s+2j}$ for every nonnegative integer $j$. For any derivative order $k$, choose $j$ with $s+2j>k+n/2$ and apply part (b). Therefore **$\boxed{u\in C^\infty(\mathbb T^n)}$**. This is elliptic bootstrapping directly from the Fourier multiplier, with no assumption that the solution initially has nonnegative Sobolev order.

## ↑ Ancestors (11)

1. [D](../d.md)
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
