<h1 id="b/6/i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the standard canonical [Wiener-Hopf factorization](../../../../../../wiener-hopf-factorization.md), first assume the nonzero kernel has [Index of a Wiener-Hopf kernel](../../../../../../index-of-a-wiener-hopf-kernel.md) zero and a continuous analytic logarithm $\ell=\log F$ tending to zero at both ends of the strip, with sufficient decay for the Cauchy projections. Choose $\alpha<a<b<\beta$. Let $\Gamma_+$ be the line $\operatorname{Im}\zeta=a$ oriented left to right, with its factor used above that line; let $\Gamma_-$ be the line $\operatorname{Im}\zeta=b$ oriented left to right, with its factor used below that line.

For $a<\operatorname{Im}z<b$, closing the rectangle between the two lines and using the [Cauchy integral formula](../../../../../../cauchy-integral-formula.md) gives

$$
\log F_+(z)-\log F_-(z)
=\frac1{2\pi i}\left(\int_{\Gamma_+}-\int_{\Gamma_-}\right)\frac{\ell(\zeta)}{\zeta-z}d\zeta
=\ell(z).
$$

Thus $F=F_+/F_-$. Multiplying $Fw_+=w_-$ gives $F_+w_+=F_-w_-$ in the overlap. The canonical factors are analytic, nonzero, and normalized at infinity in their respective half-planes, so part (a) yields

$$
\boxed{F_+w_+=F_-w_-=\text{constant}.}
$$

Contours may be shifted within the strip without changing their factors on the appropriate side. When necessary, a subtracted Cauchy kernel fixes convergence and the common normalization constant.

The printed hypotheses omit the index and factor-growth qualifications; $F\to1$ alone does not ensure them. An explicit counterexample is $F(z)=(z+i)/(z-i)$ on $-1/2<\operatorname{Im}z<1/2$, with $w_+=(z-i)/(z+i)$ and $w_-=1$. Both $w$ functions are analytic and bounded at infinity in their prescribed half-planes, and the relation holds. If admissible analytic factors made their common product a nonzero constant, $w_-=1$ would force $F_-$ constant and hence $F_+$ proportional to $F$, impossible because $F$ has a [pole](../../../../../../pole.md) at $i$ in the plus half-plane. The natural factors $F_+=z+i$, $F_-=z-i$ instead give the nonconstant common polynomial $z-i$. Thus the boxed constant conclusion is the intended index-zero result, not a consequence of the literal assumptions alone.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [I](../../i.md)
3. [6](../../../6.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../../split.md)
7. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
