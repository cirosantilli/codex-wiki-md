<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

The [Wronskian](../../../../../wronskian.md) satisfies [Abel identity](../../../../../abel-s-identity.md). Differentiating and substituting the homogeneous equations gives

$$
W'=y_1y_2''-y_1''y_2=-pW,\qquad W(0)=-1,
$$

so $W(x)=-\exp[-\int_0^xp(r)\,dr]\ne0$. The two homogeneous solutions are therefore independent.

Define the [variation of parameters](../../../../../variation-of-parameters.md) kernel

$$
K(x,s)=\frac{y_1(s)y_2(x)-y_1(x)y_2(s)}{W(s)}.
$$

For fixed $s$, it satisfies the homogeneous differential equation in $x$. Direct evaluation gives $K(s,s)=0$ and $K_x(s,s)=1$. For $y(x)=\int_0^xK(x,s)f(s)\,ds$, differentiation under the integral therefore yields

$$
y'=\int_0^xK_x(x,s)f(s)\,ds,\qquad
y''=f(x)+\int_0^xK_{xx}(x,s)f(s)\,ds.
$$

Combining these identities proves $y''+py'+qy=f$; both initial values vanish. Continuity of the coefficients gives uniqueness of this [initial value problem](../../../../../initial-value-problem.md), establishing the proposed formula rather than merely recognizing it as a standard method.

For the oscillator, $y_1=\sin x$, $y_2=\cos x$ and $W=-1$, so the kernel is $\sin(x-s)$. Hence

$$
y(x)=\int_0^x\sin(x-s)\sin s\,ds
=\sin x\int_0^x\cos s\sin s\,ds-\cos x\int_0^x\sin^2s\,ds.
$$

Using $\int_0^x\cos s\sin s\,ds=\sin^2x/2$ and $\int_0^x\sin^2s\,ds=x/2-\sin(2x)/4$ gives

$$
\boxed{y(x)=\frac12(\sin x-x\cos x).}
$$

The factor $x\cos x$ reflects [resonance](../../../../../resonance.md) with the homogeneous oscillator frequency.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
