<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First establish the scalar [Leibniz rule](../../../../../../../leibniz-rule.md), since it is needed for an extension to all [tensor fields](../../../../../../../tensor-field.md). Suppose every component of $M$ has positive dimension. Computing $D(fgY)$ first with scalar $fg$ and then as $f(gY)$ gives

$$
\bigl(D(fg)-fDg-gDf\bigr)Y=0.
$$

At any point, a [smooth cutoff function](../../../../../../../smooth-cutoff-function.md) times a coordinate [vector field](../../../../../../../vector-field.md) can be chosen nonzero there. Evaluating the displayed identity proves

$$
D(fg)=fDg+gDf,\qquad D1=0.
$$

Thus the scalar operator is a [derivation of an algebra](../../../../../../../derivation-of-an-algebra.md). [Derivations of smooth functions are vector fields](../../../../../../../derivations-of-smooth-functions-are-vector-fields.md), so the scalar operator is differentiation along a unique [vector field](../../../../../../../vector-field.md) $Z$; no continuity assumption is needed. Indeed, if $h$ vanishes near $p$, take a [smooth cutoff function](../../../../../../../smooth-cutoff-function.md) $\chi$ equal to one near $p$ and supported where $h=0$. The identity $D(\chi h)=(D\chi)h+\chi Dh=0$ gives $Dh(p)=0$. Thus $D$ depends only on the local function germ, so local coordinate functions may be extended with cutoffs before applying it. The local identity $h(x)=h(p)+\sum_i(x^i-x^i(p))h_i(x)$ gives $Dh(p)=\sum_i D(x^i)(p)\partial_i h(p)$. Smooth local coefficients $D(x^i)$ define $Z$.

The vector-field operator is local as well. If $Y$ vanishes near $p$, choose a cutoff $h$ equal to one near $p$ with support where $Y=0$. Then $D(hY)=hDY+(Dh)Y$ gives $DY(p)=0$. We can therefore work with local frames without presuming a global frame.

For a [differential one-form](../../../../../../../one-form.md) $\omega$, the only possible contraction-compatible definition is

$$
\boxed{(D\omega)(Y)=D(\omega(Y))-\omega(DY).}
$$

The scalar product rule and the given vector-field rule show that this is linear over $C^\infty(M)$ in $Y$, so it defines a one-form. Its coefficients are smooth by evaluating the formula on local frame fields extended with cutoffs. It is real-linear in $\omega$, and direct substitution gives $D(f\omega)=fD\omega+(Df)\omega$.

The original PDF's hint has a transpose error. If $De_i=\sum_j a_{ij}e_j$ for $e_i=\partial/\partial x^i$, then evaluation on every $e_j$ forces

$$
\boxed{D(dx^i)=-\sum_j a_{ji}\,dx^j,}
$$

not the untransposed coefficient array printed in the hint. For example, take $Df=0$, $De_1=e_2$ and $De_2=0$ on $\mathbb R^2$. The correct values are $D(dx^1)=0$, $D(dx^2)=-dx^1$. The printed hint instead makes the derivative of $dx^1(e_2)=0$ equal to $-1$.

There is also a genuine zero-dimensional edge case in the hypotheses: on a one-point manifold the vector-field space is zero, so the printed rule imposes no condition on the scalar map. Taking $Df=f$ satisfies that rule but cannot extend to a [tensor derivation](../../../../../../../tensor-derivation.md), since the product rule requires $D1=0$. Thus the extension theorem is valid on positive-dimensional manifolds as above, or in every dimension if the scalar product rule is added explicitly. The next two parts use these precise hypotheses.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 115](../../../../paper-115-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
