<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use a real [Lie algebra](../../../../../lie-algebra-split.md) convention $[T_a,T_b]=f_{ab}{}^cT_c$. Its [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md) acts on $\mathfrak g$ itself:

$$
\boxed{\operatorname{ad}_X(Y)=[X,Y].}
$$

Linearity is immediate. The [Jacobi identity](../../../../../jacobi-identity.md) gives

$$
[\operatorname{ad}_X,\operatorname{ad}_Y]Z
=[X,[Y,Z]]-[Y,[X,Z]]=[[X,Y],Z],
$$

so $[\operatorname{ad}_X,\operatorname{ad}_Y]=\operatorname{ad}_{[X,Y]}$, the defining [Lie algebra representation](../../../../../lie-algebra-representation.md) condition. In the basis $T_b$, its [matrix](../../../../../matrix.md) entries are

$$
\boxed{(T_a^{\rm ad})^c{}_b=f_{ab}{}^c.}
$$

Thus the adjoint generators are the [structure constants](../../../../../structure-constant.md) arranged as [matrices](../../../../../matrix.md). The representation has kernel equal to the [center of a Lie algebra](../../../../../center-of-a-lie-algebra.md); it need not be faithful for an arbitrary algebra.

The [Adjoint representation of a Lie group](../../../../../adjoint-representation-of-a-lie-group.md) is $\operatorname{Ad}_g(Y)=gYg^{-1}$. It satisfies $\operatorname{Ad}_{gh}=\operatorname{Ad}_g\operatorname{Ad}_h$, preserves the identity, and sends inverses to inverse [matrices](../../../../../matrix.md). Differentiating $e^{tX}Ye^{-tX}$ gives $[X,e^{tX}Ye^{-tX}]$, so

$$
\boxed{\operatorname{Ad}_{e^X}=e^{\operatorname{ad}_X},\qquad e^{-X}Ye^X=e^{-\operatorname{ad}_X}Y.}
$$

Consequently the positive adjoint exponentials furnish the representation on elements $g=e^X$ and their products, and the intrinsic conjugation action defines it globally.

**The inverse-conjugation formula in the PDF needs a minus adjoint exponent with this standard definition.** Its first-order term is $Y-[X,Y]$, whereas $e^{+\operatorname{ad}_X}Y$ has first-order term $Y+[X,Y]$. For example $X=T_1,Y=T_2$ in a nonabelian algebra with $[T_1,T_2]\neq0$ already distinguishes the two. The [inverse conjugation and adjoint antirepresentations](../../../../../inverse-conjugation-and-adjoint-antirepresentations.md) identity explains the group-order issue as well: $F(g)=\operatorname{Ad}_{g^{-1}}$ satisfies $F(gh)=F(h)F(g)$. Retaining the printed inverse conjugation as a left action without this order reversal would not give an ordinary [group representation](../../../../../group-representation.md).

The [Killing form](../../../../../killing-form.md) is the symmetric [bilinear form](../../../../../bilinear-form.md)

$$
\boxed{B(X,Y)=\operatorname{tr}(\operatorname{ad}_X\operatorname{ad}_Y).}
$$

To prove degeneracy for a non-[semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), take its nonzero [solvable radical](../../../../../radical-of-a-lie-algebra.md) and the last nonzero member $\mathfrak a$ of its [derived series of a Lie algebra](../../../../../derived-series-of-a-lie-algebra.md). This is a nonzero abelian [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md). For $x\in\mathfrak a$, $\operatorname{ad}_x$ maps $\mathfrak g$ into $\mathfrak a$ and kills $\mathfrak a$. Every $\operatorname{ad}_y$ preserves $\mathfrak a$. Hence $\operatorname{ad}_x\operatorname{ad}_y$ maps the full space into $\mathfrak a$ and has zero restriction there, so its trace is zero. Thus $B(x,y)=0$ for every $y$. This is the [abelian ideals lie in the radical of the Killing form](../../../../../abelian-ideals-lie-in-the-radical-of-the-killing-form.md) argument, and establishes a nonzero kernel and vanishing [determinant](../../../../../determinant.md).

For a compact real [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), the adjoint action is unitary in an invariant positive [inner product](../../../../../inner-product.md). Its infinitesimal generators are skew-Hermitian, giving

$$
B(X,X)=-\operatorname{tr}(\operatorname{ad}_X^\dagger\operatorname{ad}_X)<0\qquad(X\neq0).
$$

Strictness follows because the adjoint kernel is the zero center. This explains the [compactness criterion from the Killing form](../../../../../compactness-criterion-from-the-killing-form.md): “strictly negative” means negative-definite, not that every entry of its [matrix](../../../../../matrix.md) is negative.

In the first three-generator example, take columns to be images of the basis $(X,Y,H)$. Direct use of the brackets gives

$$
\boxed{\operatorname{ad}_X=\begin{pmatrix}0&0&0\\0&0&2\\0&2&0\end{pmatrix},\quad
\operatorname{ad}_Y=\begin{pmatrix}0&0&2\\0&0&0\\-2&0&0\end{pmatrix},\quad
\operatorname{ad}_H=\begin{pmatrix}0&-2&0\\-2&0&0\\0&0&0\end{pmatrix}.}
$$

Taking traces of products yields the [Killing form for cyclic three-generator brackets](../../../../../killing-form-for-cyclic-three-generator-brackets.md)

$$
\boxed{[B]_{(X,Y,H)}=\operatorname{diag}(8,-8,8).}
$$

It is nondegenerate, hence semisimple by the preceding degeneracy result, but it has mixed signature and is not compact. An explicit realization is

$$
X=\begin{pmatrix}0&1\\1&0\end{pmatrix},\quad
Y=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\quad
H=\begin{pmatrix}-1&0\\0&1\end{pmatrix},
$$

which span the real traceless two-by-two [matrices](../../../../../matrix.md) and satisfy exactly these brackets.

Changing the sign of $[X,H]$ changes the first and third adjoint [matrices](../../../../../matrix.md) to

$$
\operatorname{ad}_X=\begin{pmatrix}0&0&0\\0&0&-2\\0&2&0\end{pmatrix},\qquad
\operatorname{ad}_H=\begin{pmatrix}0&-2&0\\2&0&0\\0&0&0\end{pmatrix},
$$

while $\operatorname{ad}_Y$ is unchanged. Now

$$
\boxed{[B]=-8I_3,}
$$

the negative-definite compact case. The basis $X=-i\sigma_1$, $Y=-i\sigma_2$, $H=-i\sigma_3$ realizes it as the real [special unitary Lie algebra](../../../../../special-unitary-lie-algebra.md) $\mathfrak{su}(2)$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
