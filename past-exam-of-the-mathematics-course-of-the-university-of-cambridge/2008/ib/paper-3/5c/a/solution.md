<h1 id="5c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $t>0$, use the [Bromwich inversion formula](../../../../../../bromwich-inversion-formula.md) with a vertical contour $\operatorname{Re}s=c>0$:

$$
f(t)=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}e^{st}\frac{s}{s^2+a^2}\,ds.
$$

Close the contour to the left, where the exponential decays. The large-arc contribution tends to zero by the usual exponential arc estimate, and the two simple [poles](../../../../../../pole.md) are at $s=ia$ and $s=-ia$. The [residues](../../../../../../residue.md) of the complete integrand are $e^{iat}/2$ and $e^{-iat}/2$. The [residue theorem](../../../../../../residue-theorem.md) therefore gives

$$
\boxed{\mathcal L^{-1}\!\left[\frac{s}{s^2+a^2}\right](t)=\cos(at)\quad(t>0).}
$$

The right limit at zero is one. The sign of nonzero real $a$ has no effect on the answer.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5C](../../5c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
