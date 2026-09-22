<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For this real integral choose $0<\arg z<2\pi$, so the upper bank of the positive real axis has $z^{1/4}=x^{1/4}>0$. Use a counterclockwise [keyhole contour](../../../../../../keyhole-contour.md) with inner radius $\varepsilon$ and outer radius $R$, enclosing $\pm i$. The upper-bank contribution tends to $J$. On the lower bank, $z^{-1/4}=e^{-i\pi/2}x^{-1/4}=-ix^{-1/4}$, and the reversed orientation makes its contribution $+iJ$.

The large arc is $O(R^{-5/4})$ because $g=O(R^{-9/4})$, while the small arc is $O(\varepsilon^{3/4})$. Both vanish, giving

$$
\oint g(z)\,dz\longrightarrow(1+i)J.
$$

The [residues](../../../../../../residue.md) on this branch are

$$
\operatorname{Res}(g,i)=\frac{e^{-i\pi/8}}{2i},\qquad
\operatorname{Res}(g,-i)=-\frac{e^{-3i\pi/8}}{2i}.
$$

The [residue theorem](../../../../../../residue-theorem.md) yields

$$
(1+i)J=\pi\left(e^{-i\pi/8}-e^{-3i\pi/8}\right)
=2\pi i e^{-i\pi/4}\sin\frac\pi8.
$$

Therefore

$$
\boxed{J=\pi\sqrt2\sin\frac\pi8=\frac{\pi}{2\sin(3\pi/8)}=\frac{\pi}{\sqrt{2+\sqrt2}}.}
$$

The branch cut in (a) was arbitrary; here placing it on the integration axis makes the bank contributions directly proportional to the desired positive-real integral.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
