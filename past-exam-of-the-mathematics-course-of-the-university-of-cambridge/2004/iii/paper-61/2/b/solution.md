<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $d=\ell/(2\sqrt3)$ and $a=e^{2\pi i/3}$. Consistent with the actual PDF vertices, parametrize the three oriented sides by

$$
z^{(j)}(s)=\beta_j(d+is),\qquad (\beta_1,\beta_2,\beta_3)=(1,\bar a,a),\qquad-\ell/2\leq s\leq\ell/2.
$$

They run counterclockwise, with unit tangent $i\beta_j$ and outward normal $\beta_j$. Consequently the [normal derivative](../../../../../../normal-derivative.md) and tangential derivative satisfy

$$
q_s=i\beta_jq_z-i\bar\beta_jq_{\bar z},\qquad q_N=\beta_jq_z+\bar\beta_jq_{\bar z},\qquad i\beta_jq_z=\frac{q_s+iq_N}{2}.
$$

Let $\kappa=k\beta_j$. On this side the exponential factor becomes

$$
\chi=E(-i\kappa)e^{(\kappa+\lambda/\kappa)s},\qquad E(k)=e^{(k+\lambda/k)d}.
$$

Pulling back the [closed differential one-form](../../../../../../closed-differential-one-form.md) therefore gives

$$
W|_j=E(-i\kappa)e^{(\kappa+\lambda/\kappa)s}\left[\frac12q_s^{(j)}+\frac\lambda\kappa q^{(j)}+\frac i2q_N^{(j)}\right]ds.
$$

Define $\Phi_j(\kappa)$ and $\Psi_j(\kappa)$ by integrating the Dirichlet terms and normal term in this expression. The [Generalized Stokes theorem](../../../../../../generalized-stokes-theorem.md) gives $\int_{\partial D}W=0$, so

$$
\boxed{E(-ik)\Psi_1(k)+E(-i\bar ak)\Psi_2(\bar ak)+E(-iak)\Psi_3(ak)=2i\bigl[E(-ik)\Phi_1(k)+E(-i\bar ak)\Phi_2(\bar ak)+E(-iak)\Phi_3(ak)\bigr].}
$$

The factor $2i$ follows by solving $\sum E\Phi+(i/2)\sum E\Psi=0$. The bars on the side-2 rotation are essential; replacing them with $a$ would use the wrong side orientation. The converted TeX also reverses the sign in the upper vertex's exponential, whereas the PDF puts that vertex above the real axis; the parametrization here follows the PDF.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
