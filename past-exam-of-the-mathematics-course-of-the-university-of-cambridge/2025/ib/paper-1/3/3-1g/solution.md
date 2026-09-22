<h1 id="3/3-1g/solution">Solution</h1>

↑ **Parent:** [3.1G](../3-1g.md)

Jordan's lemma states that if $f$ is holomorphic in the upper half-plane apart from finitely many poles and $|f(z)|\le M/|z|$ on sufficiently large upper semicircles, then for $a>0$ the [integral](../../../../../../integral.md) of $e^{iaz}f(z)$ over those arcs tends to zero. Indeed, split the arc away from its endpoints, where exponential decay is uniform, and bound the two short endpoint arcs using $|e^{iaRe^{i\theta}}|=e^{-aR\sin\theta}$ and $\sin\theta\ge2\theta/\pi$ on $[0,\pi/2]$.

Apply the upper semicircle to $ze^{iz}/(1+z^2)$. The sole enclosed pole is $i$, with residue $e^{-1}/2$. Therefore the contour [integral](../../../../../../integral.md) is $\pi i/e$; taking imaginary parts gives

$$
\boxed{\int_{-\infty}^{\infty}\frac{x\sin x}{1+x^2}\,dx=\frac\pi e.}
$$

## ↑ Ancestors (11)

1. [3.1G](../3-1g.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
