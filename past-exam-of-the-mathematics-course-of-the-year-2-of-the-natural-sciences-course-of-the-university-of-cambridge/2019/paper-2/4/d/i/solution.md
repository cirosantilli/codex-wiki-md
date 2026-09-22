<h1 id="4/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Close the real segment $[-R,R]$ by an anticlockwise semicircle in the upper half-plane. For $F(z)=1/[(z^2+1)(z^2+4)]$, the [contour integral](../../../../../../contour-integral.md) over the arc is $O(R^{-3})$: its length is $\pi R$, whereas $|z^2+1|\geq R^2-1$ and $|z^2+4|\geq R^2-4$. The enclosed [simple poles](../../../../../../simple-pole.md) are $i$ and $2i$, with [residues](../../../../../../residue.md)

$$
\operatorname{Res}_{i}F=\frac1{(2i)(i^2+4)}=\frac1{6i},\qquad
\operatorname{Res}_{2i}F=\frac1{(4i)((2i)^2+1)}=-\frac1{12i}.
$$

Letting $R\to\infty$ in the [residue theorem](../../../../../../residue-theorem.md) yields

$$
\boxed{\int_{-\infty}^{\infty}\frac{dx}{(x^2+1)(x^2+4)}
=2\pi i\left(\frac1{6i}-\frac1{12i}\right)=\frac\pi6}.
$$

## ↑ Ancestors (14)

1. [I](../i.md)
2. [D](../../d.md)
3. [4](../../../4.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
