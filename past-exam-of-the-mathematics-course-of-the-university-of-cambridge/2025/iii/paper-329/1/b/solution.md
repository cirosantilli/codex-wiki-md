<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For two zero-body-force [Stokes flows](../../../../../../stokes-flow-split.md) $(\mathbf u,\boldsymbol\sigma)$ and $(\widehat{\mathbf u},\widehat{\boldsymbol\sigma})$ in the same domain, the [Lorentz reciprocal theorem for Stokes flow](../../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) states

$$
\int_{\partial D}\mathbf u\mathbin\cdot\widehat{\boldsymbol\sigma}\mathbf n\,dS
=\int_{\partial D}\widehat{\mathbf u}\mathbin\cdot\boldsymbol\sigma\mathbf n\,dS.
$$

Apply it first with the auxiliary translating-sphere solution and then with the auxiliary rotating-sphere solution. The swimmer is [force-free](../../../../../../force-free.md) and [torque-free](../../../../../../torque-free.md), while the auxiliary surface tractions are known. The resulting [surface slip velocity](../../../../../../surface-slip-velocity.md) formulas are

$$
\boxed{
\mathbf V=-\frac1{4\pi a^2}\int_{r=a}\mathbf u_s\,dS,
\qquad
\boldsymbol\omega=-\frac3{8\pi a^4}\int_{r=a}\mathbf x\times\mathbf u_s\,dS.}
$$

On $r=a$, the first part of the prescribed slip is

$$
\frac{(\mathbf A\times\mathbf x)\times\mathbf x}{a^2}
=\frac{\mathbf x(\mathbf A\mathbin\cdot\mathbf x)}{a^2}-\mathbf A.
$$

Its surface average is $-2\mathbf A/3$, whereas the $\mathbf B$ term has zero average by [oddness](../../../../../../odd-function.md). Thus

$$
\boxed{\mathbf V=\frac23\mathbf A.}
$$

The $\mathbf A$ term contributes no rotation. For the other term, the isotropic second and fourth surface moments give

$$
\int_{r=a}\mathbf x\times\mathbf u_s\,dS
=\frac{8\pi a^3}{15}|\mathbf B|^2\mathbf B,
$$

and hence

$$
\boxed{\boldsymbol\omega=-\frac{|\mathbf B|^2}{5a}\mathbf B.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
