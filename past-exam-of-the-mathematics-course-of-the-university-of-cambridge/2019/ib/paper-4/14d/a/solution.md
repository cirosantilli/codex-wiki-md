<h1 id="14d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Bromwich inversion formula](../../../../../../bromwich-inversion-formula.md) gives

$$
f(t)=\frac1{2\pi i}\int_{\gamma-i\infty}^{\gamma+i\infty}\frac{e^{st}}{s^2}\,ds,
\qquad \gamma>0.
$$

For $t>0$, close the [Bromwich contour](../../../../../../bromwich-contour.md) in the left half-plane. The only enclosed singularity is the [double pole](../../../../../../double-pole.md) at $s=0$, whose [residue](../../../../../../residue.md) is

$$
\operatorname*{Res}_{s=0}\frac{e^{st}}{s^2}
=\left.\frac d{ds}e^{st}\right|_{s=0}=t.
$$

The [residue theorem](../../../../../../residue-theorem.md) therefore yields

$$
\boxed{\mathcal L^{-1}\{s^{-2}\}(t)=t}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14D](../../14d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
