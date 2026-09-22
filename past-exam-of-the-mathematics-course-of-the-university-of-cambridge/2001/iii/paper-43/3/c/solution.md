<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The ratio $\lambda=H/z_s$ compares the reference constant-stratification rise length with the height at which the actual [buoyancy frequency](../../../../../../buoyancy-frequency.md) equals $N_s$. Equivalently, the actual gradient sampled around that reference height is $N^2(H)/N_s^2=\lambda^\beta$. Positive $\beta$ means stratification strengthens upwards; negative $\beta$ means it weakens upwards.

For a finite-rise branch at fixed $\beta>0$, increasing $\lambda$ makes the gradient stronger at each fixed normalized height $z/H$, so $H'/H$ decreases. A small $\lambda$ means a larger region of weaker-than-reference stratification and permits relatively greater rise. For $\beta<0$, the same comparison reverses: increasing $\lambda$ weakens the sampled stratification, increases $H'/H$, and can permit escape when the upper stratification decays sufficiently fast. At $\beta=0$ the ratio is one. Comparison at $\lambda=1$ is not an exact equality for nonzero $\beta$, because the plume samples a whole range of heights, not only $z=H$.

Using the [pure plume](../../../../../../pure-plume.md) as a scaling estimate before appreciable buoyancy loss,

$$
B_0\sim N_s^2z_s^{-\beta}B_0^{1/3}(H')^{\beta+8/3},\qquad
\boxed{\frac{H'}H\sim C(\beta,\alpha)\lambda^{-3\beta/(8+3\beta)}}
$$

when $\beta>-8/3$ and the lower integral is regular. This gives the preceding monotonic trends, but not a universal numerical height. In particular, sufficiently negative powers are singular at a literal point source at $z=0$. A finite source elevation or a regularized near-source stratification must then be specified, as in part (d); no finite positive source buoyancy can absorb an infinite near-source buoyancy loss. Once such a finite source is used, $N^2Q\sim z^{\beta+5/3}$ has an integrable far-field tail for $\beta<-8/3$. A sufficiently buoyant plume can then retain positive buoyancy and rise without bound. The exact decaying-buoyancy infinite-rise branch in part (d) is another, specially matched possibility.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
