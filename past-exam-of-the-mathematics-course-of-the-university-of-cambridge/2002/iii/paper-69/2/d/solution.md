<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $f=-V^{-1}\log\mathcal Z$ be the dimensionless [free-energy density](../../../../../../free-energy-density.md). The transformed volume is $V'=V/B$. Including the normalization from eliminated modes gives

$$
f(t,h)=g_b(t,h)+B^{-1}f(t',h'),
$$

where $g_b$ is an additive shell contribution. After subtraction of regular backgrounds, the leading singular part obeys the [scaling hypothesis for critical phenomena](../../../../../../scaling-hypothesis-for-critical-phenomena.md)

$$
f_s(t,h)=b^{-D_{\rm eff}}f_s(b^2t,b^{(d+5)/4}h),\qquad D_{\rm eff}=(d+1)/2.
$$

Choose $b=t^{-1/2}$ for the high-temperature side $t>0$. Then the nominal homogeneous form is

$$
\boxed{f_s(t,h)=t^{(d+1)/4}g_f\!\left(h/t^{(d+5)/8}\right),\quad
\alpha=(7-d)/4,\quad\Delta=(d+5)/8.}
$$

The volume exponent is $D_{\rm eff}$, so inserting $d$ in the isotropic hyperscaling formula would give the wrong answer.

There are two qualifications to interpreting this as the total [free energy](../../../../../../thermodynamic-free-energy.md). Completing the Gaussian square gives the source contribution exactly as $-h^2/(2t)$, and the zero-field [determinant](../../../../../../determinant.md) contributes

$$
f(t,h)=\frac12\int_q\log(Kq_\parallel^2+Lq_\perp^4+t)-\frac{h^2}{2t}+\text{normalization}.
$$

Rescaling $q_\parallel\sim t^{1/2}$ and $q_\perp\sim t^{1/4}$ gives the power $t^{(d+1)/4}$, while $2\Delta-1=(d+1)/4$ makes the source term consistent with it. Cutoff-dependent analytic terms need not obey the homogeneous law. Furthermore [Gaussian free-energy logarithms at integer singular powers](../../../../../../gaussian-free-energy-logarithms-at-integer-singular-powers.md) replace the pure zero-field power by $t^n\log t$ when $(d+1)/4=n$ is a positive integer, including $d=3,7$. This is the usual logarithmic qualification of the nominal exponents. The quadratic model also has no stable negative-$t$ phase unless a stabilizing interaction is added.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
