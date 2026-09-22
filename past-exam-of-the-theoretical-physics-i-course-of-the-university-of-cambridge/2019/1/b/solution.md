<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There is a sign inconsistency in the original PDF: varying its action gives a plus sign for the spatially projected magnetic term, whereas its displayed target equation has a minus sign. The following [Lagrange multiplier for antisymmetry](../../../../lagrange-multiplier-for-antisymmetry.md) calculation derives the result of the action as printed.

Temporarily vary all sixteen entries $M^{\mu\nu}$ independently and add

$$
\mathcal L_{\lambda}=\frac12\lambda_{\mu\nu}(M^{\mu\nu}+M^{\nu\mu}),\qquad \lambda_{\mu\nu}=\lambda_{\nu\mu}.
$$

Variation of the symmetric [Lagrange multiplier](../../../../lagrange-multiplier.md) imposes $M^{\mu\nu}+M^{\nu\mu}=0$. Define

$$
w_\mu=u_\rho M^\rho{}_{\mu},\qquad C_{\mu\nu}=h_{\mu\rho}h_{\nu\sigma}M^{\rho\sigma}.
$$

On this constraint surface, $C_{\nu\mu}=-C_{\mu\nu}$. Differentiating the original contractions before imposing the constraint gives

$$
\left.\frac{\partial}{\partial M^{\mu\nu}}(u_\alpha u_\beta M^{\lambda\alpha}M^\beta{}_{\lambda})\right|_{M=-M^{\mathsf T}}
=u_\nu w_\mu-u_\mu w_\nu,
$$

and

$$
\left.\frac{\partial}{\partial M^{\mu\nu}}(h_{\alpha\rho}h_{\beta\sigma}M^{\alpha\beta}M^{\sigma\rho})\right|_{M=-M^{\mathsf T}}
=-2C_{\mu\nu}.
$$

In particular, the reversed order $\sigma\rho$ in the last factor of the action matters. The unrestricted [Euler-Lagrange field equation](../../../../euler-lagrange-field-equation.md), evaluated on the antisymmetry constraint, is

$$
0=\frac12F_{\mu\nu}-\frac1{2\kappa}(u_\nu w_\mu-u_\mu w_\nu)+\frac1{2\chi}C_{\mu\nu}+\lambda_{\mu\nu}.
$$

Subtract its index-transposed equation to eliminate the symmetric multiplier:

$$
\boxed{0=F_{\mu\nu}-\frac1\kappa\left(u_\nu u_\rho M^\rho{}_{\mu}-u_\mu u_\rho M^\rho{}_{\nu}\right)+\frac1\chi h_{\mu\rho}h_{\nu\sigma}M^{\rho\sigma}.}
$$

A direct check is to restrict the [action](../../../../action.md) to a rest-frame magnetic component $M^{12}=m$, $M^{21}=-m$: its quadratic contribution is $+m^2/(2\chi)$, whose derivative has a positive sign. To obtain the PDF's target equation instead, one must reverse the sign of that quadratic term in the action, or replace its last $M^{\sigma\rho}$ by $M^{\rho\sigma}$. These are alternative repairs; changing conventions cannot make the printed action and printed equation agree.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
