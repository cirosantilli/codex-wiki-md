<h1 id="a/2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In the [outer expansion](../../../../../outer-expansion.md), omit $\epsilon y''$ to get $y_0'=e^{y_0}$. Integrating and imposing the left boundary condition gives

$$
y_{\rm out}(x)=-\log(C-x),\qquad C=e^{-A}>1.
$$

This is regular throughout $[0,1]$. Its right-end value is $B=-\log(C-1)$, generally different from zero.

At $x=1$ set $X=(x-1)/\epsilon$. The equation is $Y''-Y'+\epsilon e^Y=0$, so the leading [inner expansion](../../../../../inner-expansion.md) is $Y=C_0+C_1e^X$. Matching as $X\to-\infty$ gives $C_0=B$, while $Y(0)=0$ gives $C_1=-B$. Thus

$$
y_{\rm in}(x)=B\left[1-\exp\left(\frac{x-1}{\epsilon}\right)\right].
$$

The common part is $B$. Subtract it once when forming the [additive composite expansion](../../../../../additive-composite-expansion.md):

$$
\boxed{y_c(x)=-\log(e^{-A}-x)+\log(e^{-A}-1)
\exp\left(\frac{x-1}{\epsilon}\right).}
$$

There is one generic boundary layer, at the right endpoint, of width $\epsilon$. A left-end exponential would grow into the interval and cannot supply a decaying matching correction. At $A=-\log2$ the displayed layer amplitude vanishes; the leading outer solution already meets the right condition, though a smaller correction can still be needed at higher order. The composite meets $y(1)=0$ exactly and $y(0)=A$ up to an exponentially small term.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
