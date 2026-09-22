<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the counterclockwise rectangular [contour](../../../../../complex-integration-contour.md) with vertices $-R,R,R+i\pi,-R+i\pi$. It encloses just the [simple pole](../../../../../simple-pole.md) $i\pi/2$, whose [residue](../../../../../residue.md) is $e^{k\pi/2}/i$. Let $I_R=\int_{-R}^R e^{-ikx}/\cosh x\,dx$. The identity

$$
f(x+i\pi)=-e^{k\pi}f(x)
$$

makes the top edge, traversed right to left, contribute $e^{k\pi}I_R$. On either vertical edge,

$$
|\cosh(\pm R+iy)|^2=\sinh^2R+\cos^2y,\qquad |e^{-ik(\pm R+iy)}|=e^{ky}\leq e^{|k|\pi}.
$$

Thus the sum of the vertical integrals tends to zero, with absolute value at most $2\pi e^{|k|\pi}/\sinh R$. The [residue theorem](../../../../../residue-theorem.md) and $R\to\infty$ now give

$$
(1+e^{k\pi})I=2\pi e^{k\pi/2},\qquad
\boxed{I=\pi\operatorname{sech}\frac{k\pi}{2}.}
$$

The argument works for every fixed real $k$, including zero and negative values, and gives the [Fourier transform of the hyperbolic secant](../../../../../fourier-transform-of-the-hyperbolic-secant.md) with the convention $\widetilde f(k)=\int e^{-ikx}f(x)\,dx$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
