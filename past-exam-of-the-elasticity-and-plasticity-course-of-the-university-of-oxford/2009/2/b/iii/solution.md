<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Multiplication of the preceding [displacement](../../../../../displacement.md) formula by $-ik$ gives

$$
\boxed{2\mu\widehat{v_x}=\widehat P\left[-ikye^{-qy}-2i(1-\nu)\frac{k}{q}e^{-qy}\right].}
$$

For the supplied kernels, $\widehat{f_{1,x}}=-ike^{-qy}$ and $\widehat f_2=i(k/q)e^{-qy}$. The [convolution theorem](../../../../../convolution-theorem.md) therefore gives

$$
2\mu v_x=P*\left[yf_{1,x}-2(1-\nu)f_2\right].
$$

Since $f_{1,x}(s,y)=-2ys/[\pi(s^2+y^2)^2]$ and $f_2(s,y)=s/[\pi(s^2+y^2)]$, combine the two fractions and divide by two:

$$
\boxed{\mu v_x(x,y)=-\frac1\pi\int_{-\infty}^\infty\frac{(1-\nu)s^2+(2-\nu)y^2}{(s^2+y^2)^2}\,P(x-s)s\,ds.}
$$

The sign is tied to the positive forward Fourier phase used here. This is a [displacement](../../../../../displacement.md) derivative, so an additive [displacement](../../../../../displacement.md) reference drops out. At $y>0$ the kernel is regular near $s=0$; the usual decay/integrability of the applied load controls the tails. A boundary-limit singular integral, if wanted at $y=0$, would require its own principal-value interpretation.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../../split.md)
6. [Elasticity and plasticity course of the University of Oxford](../../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
