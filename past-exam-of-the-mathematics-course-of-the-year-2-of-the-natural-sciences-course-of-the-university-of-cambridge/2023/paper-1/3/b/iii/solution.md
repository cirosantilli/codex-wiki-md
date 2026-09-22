<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $0<t<1$, split the [Green's function](../../../../../../green-s-function-split.md) integral where the absolute value changes sign:

$$
x(t)=-\frac14\left[e^{-2t}\int_0^t\tau e^{2\tau}\,d\tau+e^{2t}\int_t^1\tau e^{-2\tau}\,d\tau\right].
$$

The two terms inside the bracket are respectively

$$
\frac t2-\frac14+\frac14e^{-2t},\qquad\frac t2+\frac14-\frac34e^{2t-2}.
$$

Adding them yields

$$
\boxed{x(t)=-\frac t4-\frac1{16}e^{-2t}+\frac3{16}e^{2t-2},\qquad0<t<1.}
$$

The affine term gives $x''-4x=t$, while both exponential terms are homogeneous solutions. The values at the joins are $x(0)=(3e^{-2}-1)/16$ and $x(1)=-(1+e^{-2})/16$, agreeing with parts (i) and (ii). Their first [derivatives](../../../../../../derivative.md) also match: $x'(0)=(3e^{-2}-1)/8$ and $x'(1)=(1+e^{-2})/8$. Thus the pieces introduce no unwanted [Dirac delta distributions](../../../../../../dirac-delta-function.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
