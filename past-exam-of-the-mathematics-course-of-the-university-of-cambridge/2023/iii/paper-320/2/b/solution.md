<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [relative energy](../../../../../../relative-energy.md) $\mathcal E=-E=\Psi-v^2/2$. At fixed $r$, write velocity-space spherical coordinates with polar angle $\alpha$ from the radial direction, so $L=rv\sin\alpha$. Then

$$
\rho=2\pi f_0r^{-2\beta}
\int_0^{\sqrt{2\Psi}}v^{2-2\beta}
(\Psi-v^2/2)^n,dv
\int_0^\pi\sin^{1-2\beta}\alpha\,d\alpha.
$$

The [beta function](../../../../../../beta-function.md) integrals give

$$
\boxed{
\rho(r)=A r^{-2\beta}\Psi^{n+3/2-\beta}},
$$

where

$$
\boxed{
A=f_0,2^{3/2-\beta}\pi^{3/2}
\frac{\Gamma(1-\beta)\Gamma(n+1)}
{\Gamma(n+5/2-\beta)}}.
$$

Thus $\gamma=2\beta$ and $p=n+3/2-\beta$, with convergence for $\beta<1$ and $n>-1$.

Comparison with part a gives

$$
(\beta_1,n_1)=\left(\frac34,\frac54\right),
\qquad
(\beta_2,n_2)=\left(\frac12,2\right).
$$

Hence the model has the [constant-anisotropy distribution function](../../../../../../constant-anisotropy-distribution-function.md)

$$
\boxed{
f(\mathcal E,L)=f_{01}L^{-3/2}\mathcal E^{5/4}
+f_{02}L^{-1}\mathcal E^2},
$$

where matching the two density coefficients gives

$$
\boxed{
f_{01}=\frac{3\,2^{5/4}\sqrt b}
{5\pi^{5/2}G^2M\Gamma(1/4)^2},
\qquad
f_{02}=\frac{3b}{4\pi^3G^3M^2}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
