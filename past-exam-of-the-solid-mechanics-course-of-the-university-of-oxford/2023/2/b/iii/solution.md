<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take the inner surface to be free of [traction](../../../../../traction.md), as appropriate to an empty cavity with no [surface tension](../../../../../surface-tension-split.md). At the outer surface the imposed [pressure](../../../../../pressure-split.md) is compressive when positive. The outward [normal vectors](../../../../../normal-vector.md) are $-\mathbf e_r$ at $r=a$ and $+\mathbf e_r$ at $r=b$, giving

$$
t_r(a)=0,\qquad t_r(b)=-P.
$$

Integrating the [ordinary differential equation](../../../../../ordinary-differential-equation.md) from part (ii) between the two surfaces gives

$$
-P=\int_{\lambda_a}^{\lambda_b}\frac{h'(\lambda)}{1-\lambda^3}\,d\lambda.
$$

The outer stretch follows from [incompressibility](../../../../../incompressible-flow.md):

$$
\lambda_b^3=\frac{b^3}{B^3}
=1+\frac{A^3}{B^3}(\lambda_a^3-1).
$$

Hence an expression entirely in terms of the inner stretch and the reference radii is

$$
\boxed{P(\lambda_a)=
\int_{\lambda_a}^{[1+(A/B)^3(\lambda_a^3-1)]^{1/3}}
\frac{h'(\lambda)}{\lambda^3-1}\,d\lambda.}
$$

Equivalently $P=-\int_{\lambda_b}^{\lambda_a}h'(\lambda)/(\lambda^3-1)\,d\lambda$. For an expanding shell, $1<\lambda_b<\lambda_a$; when $h'>0$ on this range, $P<0$, correctly describing an outward tensile loading. If an inner [pressure](../../../../../pressure-split.md) $P_i$ were present, the same derivation would give $P-P_i$ on the left. Thus the empty-cavity condition specifies the pressure reference needed for the requested answer.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the solid mechanics course of the University of Oxford](../../../../split.md)
6. [Solid mechanics course of the University of Oxford](../../../../../solid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
