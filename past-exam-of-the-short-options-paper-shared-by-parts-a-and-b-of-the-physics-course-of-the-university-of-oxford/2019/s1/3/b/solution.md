<h1 id="s1/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $z=e^{i\theta}$, so $d\theta=dz/(iz)$, $\cos2\theta=(z^2+z^{-2})/2$ and $\cos^23\theta=(z^6+2+z^{-6})/4$. The [contour integral](../../../../../contour-integral.md) is

$$
\frac1{4i}\oint_{|z|=1}\frac{z^8+2z^2+z^{-4}}{z(5z^2-2z^4-2)}\,dz.
$$

The enclosed [poles](../../../../../pole.md) are $0$ and $\pm1/\sqrt2$. For the rational function displayed without the prefactor $1/(4i)$, the [residue](../../../../../residue.md) at zero is $-21/8$ and the two other [residues](../../../../../residue.md) sum to $27/8$. Therefore the [residue theorem](../../../../../residue-theorem.md) gives

$$
\boxed{\int_0^{2\pi}\frac{\cos^23\theta}{5-4\cos2\theta}\,d\theta=\frac1{4i}(2\pi i)\frac34=\frac{3\pi}{8}.}
$$

A useful independent check is the [Fourier series](../../../../../fourier-series-split.md) $(5-4\cos\phi)^{-1}=\frac13[1+2\sum_{k\ge1}2^{-k}\cos k\phi]$; only its constant and third [Fourier coefficients](../../../../../fourier-coefficient.md) survive.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [S1](../../../s1.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
