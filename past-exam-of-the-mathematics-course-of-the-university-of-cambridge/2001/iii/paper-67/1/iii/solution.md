<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the same conserved-source interpretation, [comoving number density](../../../../../../comoving-number-density.md) $n_0$ and normalization $a_0=1$ as in the preceding part. Define

$$
u=\sqrt{-k}\,\tau,\qquad
C=\frac{\Omega_0}{2(1-\Omega_0)},\qquad
\kappa=H_0\sqrt{1-\Omega_0}.
$$

The [open matter-dominated Friedmann solution](../../../../../../open-matter-dominated-friedmann-solution.md) then has $a=C(\cosh u-1)$, $t=(C/\kappa)(\sinh u-u)$ and $dt=(C/\kappa)(\cosh u-1)du$. The present parameter satisfies

$$
\cosh u_0=\frac{2}{\Omega_0}-1.
$$

The [cosmological bolometric background from conserved sources](../../../../../../cosmological-bolometric-background-from-conserved-sources.md) is therefore

$$
\mathcal F_{\rm open}
=\frac{Ln_0C^2}{\kappa}\int_0^{u_0}(\cosh u-1)^2du.
$$

Since $\cosh^2u=(1+\cosh2u)/2$, the [open dust bolometric background integral](../../../../../../open-dust-bolometric-background-integral.md) is

$$
\boxed{\mathcal F_{\rm open}
=\frac{Ln_0\Omega_0^2}{4H_0(1-\Omega_0)^{5/2}}
\left[\frac14\sinh(2u_0)-2\sinh u_0+\frac32u_0\right].}
$$

This leaves the answer in the requested parameter form and makes no use of a radial-distance approximation. For arbitrary proper [number density](../../../../../../number-density.md) instead, the same calculation gives

$$
\mathcal F_{\rm open}
=\frac{LC^5}{\kappa}\int_0^{u_0}
n\!\left(\frac C\kappa(\sinh u-u)\right)(\cosh u-1)^5du.
$$

For the conserved population, compare models with the same present $n_0,L,H_0$. As $\Omega_0\to0$, $u_0\to\infty$ and $\cosh u_0\sim2/\Omega_0$. The leading term in the square bracket is $\sinh(2u_0)/4\sim2/\Omega_0^2$; the terms linear in $\sinh u_0$ and $u_0$ vanish after multiplication by $\Omega_0^2$. Hence

$$
\boxed{\mathcal F_{\Omega_0\to0}=\frac{Ln_0}{2H_0}
=\frac54\mathcal F_{\rm flat}\quad\text{at fixed }H_0.}
$$

This is also immediate in the [Milne model](../../../../../../milne-model.md), for which $a=t/t_0$ and $t_0=H_0^{-1}$. If one compares at fixed cosmic age instead, the results are $Ln_0t_0/2$ and $3Ln_0t_0/5$, so the empty open model gives $5/6$ of the flat-model flux. Specifying what is held fixed is necessary because the two expansion histories have different ages at the same [Hubble constant](../../../../../../hubble-constant.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
