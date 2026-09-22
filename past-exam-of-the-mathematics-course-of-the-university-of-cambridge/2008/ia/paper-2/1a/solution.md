<h1 id="1a/solution">Solution</h1>

↑ **Parent:** [1A](../1a.md)

The [complementary solution](../../../../../homogeneous-solution.md) comes from the characteristic equation $r^4-a^4=0$, whose roots are $a,-a,ia,-ia$. It is therefore

$$
y_h=C_1e^{ax}+C_2e^{-ax}+C_3\cos(ax)+C_4\sin(ax).
$$

For the [resonant exponential particular solution](../../../../../resonant-exponential-particular-solution.md), the forcing is already a homogeneous exponential, so the [method of undetermined coefficients](../../../../../method-of-undetermined-coefficients.md) needs the resonant trial $y_p=Kxe^{-ax}$. If $P(r)=r^4-a^4$, the identity $P(D)[xe^{rx}]=P'(r)e^{rx}$ when $P(r)=0$ gives $P'(-a)=-4a^3$. Hence $K=-1/(4a^3)$ and

$$
y=C_1e^{ax}+C_2e^{-ax}+C_3\cos(ax)+C_4\sin(ax)-\frac{x}{4a^3}e^{-ax}.
$$

The decay condition first eliminates the growing exponential, $C_1=0$. A nonzero combination of the sine and cosine has a fixed nonzero amplitude and cannot tend to zero, so $C_3=C_4=0$ as well. Both remaining exponential terms decay because $a>0$. Finally $y(0)=C_2=1$, giving the unique answer

$$
\boxed{y(x)=\left(1-\frac{x}{4a^3}\right)e^{-ax}.}
$$

This is an instance of [resonance in a differential equation](../../../../../resonance-in-a-differential-equation.md): multiplication by $x$ supplies the [particular solution](../../../../../particular-solution.md) when the forcing exponent is a simple characteristic root.

## ↑ Ancestors (10)

1. [1A](../1a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
