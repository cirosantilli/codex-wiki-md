<h1 id="7/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a circle in the right half-plane use $0<\lambda<1$. Its centre and radius from part (ii) satisfy $d^2-R^2=a^2$. Hence choose

$$
\boxed{a=\sqrt{d^2-R^2}.}
$$

Put $\tau_0=\operatorname{arcosh}(d/R)$. Then $\sinh\tau_0=a/R$ and

$$
\lambda=e^{-\tau_0}=\frac{d-a}{R}=\frac{R}{d+a}.
$$

Indeed the [Apollonius circle](../../../../../circles-of-apollonius.md) has centre $a\coth\tau_0=d$ and radius $a/\sinh\tau_0=R$. Its logarithmic modulus is therefore $-\tau_0$, while on $x=0$ the modulus is one. The [logarithmic Dirichlet potential between a circle and a line](../../../../../logarithmic-dirichlet-potential-between-a-circle-and-a-line.md) is

$$
\boxed{V(x,y)=\frac{V_0}{\operatorname{arcosh}(d/R)}\log\left|\frac{z-a}{z+a}\right|.}
$$

The logarithmic singularity at $a$ lies inside the excluded disk, since $d-a<R$. The other singularity, at $-a$, lies outside the right half-plane. Thus the real logarithmic modulus is harmonic throughout the required region and has exactly the two specified boundary values.

Local branches of the complex logarithm justify harmonicity; its real part is globally single-valued even though the complex logarithm need not be single-valued around the excluded disk. The displayed solution is bounded and tends to zero at infinity. A boundedness or corresponding far-field condition supplies uniqueness in this unbounded domain; finite boundary values alone do not rule out unbounded additional harmonic solutions. The same geometry appears in [cylinder-plane image charges](../../../../../cylinder-plane-image-charges.md).

<a id="7/iii/image-apollonius-circles-and-a-bounded-harmonic-potential-outside-a-circle-beside-a-line"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1-q7-circle-line-potential.png)

**[Figure 2](#7/iii/image-apollonius-circles-and-a-bounded-harmonic-potential-outside-a-circle-beside-a-line). Apollonius circles and a bounded harmonic potential outside a circle beside a line**.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
