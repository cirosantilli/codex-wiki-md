<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [curvature form of a connection](../../../../../../curvature-form.md) is the endomorphism-valued [differential two-form](../../../../../../2-form.md) defined by

$$
R^\nabla(X,Y)s=\nabla_X\nabla_Ys-\nabla_Y\nabla_Xs-\nabla_{[X,Y]}s.
$$

It is alternating in $X,Y$. To see its [tensoriality](../../../../../../tensoriality.md), replacing $X$ by $fX$ produces an extra $-Y(f)\nabla_Xs$ from the second term and an extra $+Y(f)\nabla_Xs$ from $[fX,Y]=f[X,Y]-Y(f)X$, so these cancel. Alternation gives linearity over [smooth functions](../../../../../../smooth-function.md) in $Y$ too. Replacing $s$ by $fs$ produces the additional coefficient $(X(Yf)-Y(Xf)-[X,Y]f)s=0$; all terms involving one derivative of $s$ also cancel. Thus $R^\nabla$ belongs to $\Omega^2(M;\operatorname{End}E)$.

In the coefficient-column convention of part (b), expanding the definition gives

$$
R^\nabla(X,Y)(eu)=e\Bigl(
X(\Omega(Y))-Y(\Omega(X))-\Omega([X,Y])
+\Omega(X)\Omega(Y)-\Omega(Y)\Omega(X)\Bigr)u.
$$

The first three terms are $d\Omega(X,Y)$, and the last two are $(\Omega\wedge\Omega)(X,Y)$. This proves the [Cartan curvature matrix equation](../../../../../../cartan-curvature-matrix-equation.md) $F=d\Omega+\Omega\wedge\Omega$, with matrix multiplication combined with the [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md).

The [pullback connection](../../../../../../pullback-connection.md) has matrix $\Omega'=\phi^*\Omega$. Since the [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) commutes with the [exterior derivative](../../../../../../exterior-derivative.md) and the [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md), its [curvature form of a connection](../../../../../../curvature-form.md) has matrix

$$
F'=d(\phi^*\Omega)+(\phi^*\Omega)\wedge(\phi^*\Omega)
=\phi^*(d\Omega+\Omega\wedge\Omega)=\phi^*F.
$$

Changes of [frame of a vector bundle](../../../../../../frame-of-a-vector-bundle.md) conjugate both sides by the same pulled-back transition matrix, so this identity is intrinsic. In fibre notation the answer is

$$
\boxed{R^{\nabla'}_p(u,v)=R^\nabla_{\phi(p)}(d\phi_pu,d\phi_pv),
\qquad u,v\in T_pM'.}
$$

Both sides act on the same fibre $E_{\phi(p)}$. No claim that $d\phi$ preserves [Lie brackets of vector fields](../../../../../../lie-bracket-of-vector-fields.md) for an arbitrary map is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
