<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the long filament, take the time-periodic solution of the dimensionless bending equation, after transients have decayed. Write $y=\operatorname{Re}[Y(x)e^{it}]$. Then $Y^{(4)}=-iY$, so the spatial exponents satisfy $\lambda^4=-i$. Define $C=\cos(\pi/8)$ and $S=\sin(\pi/8)$. The two roots with negative real part are $\lambda_1=-C+iS$ and $\lambda_2=-S-iC$; the other roots violate decay at infinity.

Hence $Y=Ae^{\lambda_1x}+Be^{\lambda_2x}$. The driven displacement gives $A+B=y_0$, while the zero bending moment gives $\lambda_1^2A+\lambda_2^2B=0$. Since $\lambda_2^2=-\lambda_1^2$, $A=B=y_0/2$. The [oscillatory bending of a moment-free semi-infinite filament](../../../../../../oscillatory-bending-of-a-moment-free-semi-infinite-filament.md) is

$$
\boxed{y(x,t)=\frac{y_0}{2}\left[e^{-Cx}\cos(t+Sx)+e^{-Sx}\cos(t-Cx)\right].}
$$

Holding each wave phase constant gives its dimensionless [phase velocity](../../../../../../phase-velocity.md):

$$
\boxed{v_1=-\frac1S\simeq-2.6131,\qquad v_2=\frac1C\simeq1.0824.}
$$

The first travels toward the actuator and attenuates over length $1/C$; the second travels away and attenuates over the longer length $1/S$. These are spatially damped phase patterns in an overdamped bending equation, not two undamped inertial beam waves. Their combination satisfies both displacement and zero-moment conditions at the driven end.

<a id="2/d/image-two-oppositely-traveling-damped-bending-waves"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-334-filament-waves.png)

**[Figure 2](#2/d/image-two-oppositely-traveling-damped-bending-waves). Two oppositely traveling damped bending waves**. The two components have different attenuation lengths and opposite phase velocities. Their sum gives the long-filament response to a periodically moved, moment-free endpoint.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 334](../../../paper-334-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
