<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the causal [convolution](../../../../../convolution.md) $(f_0*f_1)(x)=\int_0^x f_0(t)f_1(x-t)\,dt$. The [convolution theorem for Laplace transforms](../../../../../convolution-theorem-for-laplace-transforms.md) and (i) give

$$
\mathcal L(f_0*f_1)(p)=F_0(p)F_1(p)=\frac1{\sqrt{p^2+1}}-\frac p{p^2+1}.
$$

Since $\mathcal L(\cos x)=p/(p^2+1)$, uniqueness of the [Laplace transform](../../../../../laplace-transform.md) yields

$$
\boxed{(f_0*f_1)(x)=f_0(x)-\cos x,\qquad x\ge0.}
$$

At $x=0$ the right side is $1-1=0$, agreeing with the empty [convolution](../../../../../convolution.md) integral. Identification of $f_0$ as a [Bessel function](../../../../../bessel-function-split.md) is unnecessary.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
