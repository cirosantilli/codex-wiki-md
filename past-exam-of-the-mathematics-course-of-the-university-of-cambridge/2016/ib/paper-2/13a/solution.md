<h1 id="13a/solution">Solution</h1>

↑ **Parent:** [13A](../13a.md)

Let $a=N+\tfrac12$. The useful identity on the square contour is

$$
|\sin\pi(x+iy)|^2=\sin^2\pi x+\sinh^2\pi y.
$$

On the vertical edges the first term equals one; on the horizontal edges $|y|=a$ and $\sinh\pi a>1$. Thus $|1/\sin\pi z|\le1$ on every edge. Also $|z|\ge a$ and the contour has length $8a$, so the [estimation lemma](../../../../../estimation-lemma.md) gives

$$
\left|\oint\frac{dz}{z^2\sin\pi z}\right|\le\frac{8}{a}\longrightarrow0.
$$

At every nonzero integer $k$, the [residue](../../../../../residue.md) is $(-1)^k/(\pi k^2)$. At zero the [Laurent series](../../../../../laurent-series.md) is

$$
\frac1{z^2\sin\pi z}=\frac1{\pi z^3}+\frac{\pi}{6z}+O(z),
$$

so the [residue](../../../../../residue.md) there is $\pi/6$. The positive orientation and the [residue theorem](../../../../../residue-theorem.md) therefore give

$$
\oint\frac{dz}{z^2\sin\pi z}=2\pi i\left(\frac\pi6+\frac2\pi\sum_{k=1}^N\frac{(-1)^k}{k^2}\right).
$$

Letting $N\to\infty$ yields **the alternating reciprocal-square sum**

$$
\boxed{\sum_{k=1}^{\infty}\frac{(-1)^{k-1}}{k^2}=\frac{\pi^2}{12}.}
$$

## ↑ Ancestors (10)

1. [13A](../13a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
