<h1 id="13a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By [separation of variables](../../../../../../separation-of-variables.md), the axisymmetric [normal modes](../../../../../../normal-mode.md) satisfying regularity at $r=0$ and the fixed-edge condition at $r=1$ are

$$
J_0(\gamma_kr)\cos(\gamma_kt),
\qquad
J_0(\gamma_kr)\sin(\gamma_kt),
$$

where $J_0(\gamma_k)=0$. The zero initial displacement removes all cosine terms, so

$$
z(r,t)=\sum_{k=1}^{\infty}
C_kJ_0(\gamma_kr)\sin(\gamma_kt).
$$

Differentiating at $t=0$ gives the weighted Fourier-Bessel expansion

$$
U\mathbf1_{\{r<b\}}
=\sum_{k=1}^{\infty}\gamma_kC_kJ_0(\gamma_kr).
$$

Multiply by $rJ_0(\gamma_\ell r)$ and integrate from zero to one. The orthogonality and norm from part (i) give

$$
\frac12\gamma_\ell C_\ell J_0'(\gamma_\ell)^2
=U\int_0^b rJ_0(\gamma_\ell r)\,dr.
$$

Using

$$
\frac{d}{dr}\bigl[rJ_1(\gamma r)\bigr]
=\gamma rJ_0(\gamma r),
\qquad
J_1(x)=-J_0'(x),
$$

the remaining integral is

$$
\int_0^b rJ_0(\gamma_\ell r)\,dr
=-\frac b{\gamma_\ell}J_0'(\gamma_\ell b).
$$

Hence

$$
\boxed{
C_k=-\frac{2bU\,J_0'(\gamma_kb)}
{\gamma_k^2J_0'(\gamma_k)^2}},
$$

and therefore

$$
\boxed{
z(r,t)=\sum_{k=1}^{\infty}
C_kJ_0(\gamma_kr)\sin(\gamma_kt)}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [13A](../../13a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
