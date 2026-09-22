<h1 id="1a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Multiplying

$$
y'+P(x)y=Q(x)y^n
$$

by $y^{-n}$ and setting $z=y^{1-n}$ gives

$$
\frac1{1-n}z'+Pz=Q.
$$

Therefore the [Bernoulli differential equation](../../../../../../bernoulli-differential-equation.md) becomes

$$
\boxed{z'+(1-n)Pz=(1-n)Q}.
$$

For the stated equation,

$$
\dot x+6t^2x=2te^{-t^3}x^{1/2}.
$$

Set $z=\sqrt x$. Then

$$
\dot z+3t^2z=te^{-t^3}.
$$

The integrating factor is $e^{t^3}$, so

$$
\frac d{dt}(e^{t^3}z)=t.
$$

Hence

$$
e^{t^3}\sqrt{x}=\frac{t^2}{2}+C.
$$

The condition $x(1)=4$ gives $C=2e-\tfrac12$. Consequently

$$
\boxed{x(t)=e^{-2t^3}
\left(\frac{t^2}{2}+2e-\frac12\right)^2}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1A](../../1a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
