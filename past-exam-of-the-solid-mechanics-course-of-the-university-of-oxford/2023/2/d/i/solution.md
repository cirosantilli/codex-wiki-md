<h1 id="2/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [neo-Hookean solid](../../../../../neo-hookean-solid.md) corresponds to $\alpha=1$, with positive [shear modulus](../../../../../shear-modulus.md) $\mu$. Substitution of the [principal stretches](../../../../../principal-stretch.md) gives

$$
h(\lambda)=\frac\mu2(\lambda^{-4}+2\lambda^2-3),\qquad
h'(\lambda)=2\mu(\lambda-\lambda^{-5}).
$$

The identity $\lambda^6-1=(\lambda^3-1)(\lambda^3+1)$ simplifies the integrand:

$$
\frac{h'(\lambda)}{\lambda^3-1}
=2\mu\left(\lambda^{-2}+\lambda^{-5}\right).
$$

The two [improper integrals](../../../../../improper-integral.md) are elementary:

$$
\boxed{P_{\mathrm{crit}}
=-2\mu\left(\int_1^\infty\lambda^{-2}\,d\lambda
+\int_1^\infty\lambda^{-5}\,d\lambda\right)
=-2\mu\left(1+\frac14\right)=-\frac52\mu.}
$$

Thus the critical tensile [stress](../../../../../stress.md) magnitude is $5\mu/2$. As a check on the finite-sphere limit, part (c) gives

$$
P(a)=-2\mu\left(\lambda_b^{-1}+\frac14\lambda_b^{-4}\right),\qquad
\lambda_b=(1+a^3/B^3)^{1/3},
$$

which tends to $-5\mu/2$ as the cavity radius tends to zero.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
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
