<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [Matrix Lie group](../../../../../matrix-lie-group.md) $G$, the left [Maurer-Cartan form](../../../../../maurer-cartan-form.md) identifies tangent vectors with the [Lie algebra](../../../../../lie-algebra-split.md) by translating them to the identity:

$$
\boxed{\rho_g(v)=(dL_{g^{-1}})_g v=g^{-1}v,\qquad \rho=g^{-1}dg.}
$$

It is a [Lie algebra](../../../../../lie-algebra-split.md)-valued [differential form](../../../../../differential-form-split.md) of degree one. For a fixed $h\in G$, replacing $g$ by $hg$ gives $(hg)^{-1}d(hg)=g^{-1}dg$, so it is a [left-invariant differential form](../../../../../left-invariant-differential-form.md).

Differentiate $g^{-1}g=I$ to get $d(g^{-1})=-g^{-1}(dg)g^{-1}$. The [exterior derivative](../../../../../exterior-derivative.md) then gives

$$
d\rho=d(g^{-1})\wedge dg+g^{-1}d^2g=-g^{-1}dg\wedge g^{-1}dg=-\rho\wedge\rho.
$$

Here the [exterior product](../../../../../exterior-product.md) of matrix-valued [differential forms](../../../../../differential-form-split.md) includes matrix multiplication; the order of the matrices matters. Hence **the Maurer-Cartan equation is**

$$
\boxed{d\rho+\rho\wedge\rho=0.}
$$

Write $\rho=\sigma^\alpha T_\alpha$. Antisymmetry of the [exterior product](../../../../../exterior-product.md) implies

$$
\rho\wedge\rho=\frac12\sum_{\alpha,\beta}\sigma^\alpha\wedge\sigma^\beta[T_\alpha,T_\beta]
=\frac12\sum_{\alpha,\beta,\gamma}c^\gamma{}_{\alpha\beta}\sigma^\alpha\wedge\sigma^\beta T_\gamma.
$$

Comparison of the [Lie algebra](../../../../../lie-algebra-split.md) components yields the [Maurer-Cartan equation in a Lie-algebra basis](../../../../../maurer-cartan-equation-in-a-lie-algebra-basis.md):

$$
\boxed{d\sigma^\gamma=-\frac12\sum_{\alpha,\beta}c^\gamma{}_{\alpha\beta}\sigma^\alpha\wedge\sigma^\beta.}
$$

Thus **the canonical antisymmetric choice is $f^\gamma{}_{\alpha\beta}=-\tfrac12c^\gamma{}_{\alpha\beta}$**. The factor one half is required because the sum includes both ordered pairs $(\alpha,\beta)$ and $(\beta,\alpha)$. If only $\alpha<\beta$ is summed, its coefficient is $-c^\gamma{}_{\alpha\beta}$. Strictly, the equality of [differential forms](../../../../../differential-form-split.md) determines only the antisymmetric part of $f$: one may add any tensor symmetric in $\alpha,\beta$ without changing it. This is the [symmetric-part ambiguity in Maurer-Cartan coefficients](../../../../../symmetric-part-ambiguity-in-maurer-cartan-coefficients.md).

A faithful [matrix representation](../../../../../matrix-representation.md) of the orientation-preserving [real affine group](../../../../../orientation-preserving-affine-group-of-the-real-line.md) is

$$
\boxed{g(a,b)=\begin{pmatrix}a&b\\0&1\end{pmatrix},\qquad a>0,\ b\in\mathbb R.}
$$

Its action on $(x,1)^T$ has first component $ax+b$. The [group operation](../../../../../group-operation.md) and inverse are

$$
g(a,b)g(a',b')=g(aa',b+ab'),\qquad g(a,b)^{-1}=g(a^{-1},-b/a).
$$

Different transformations have different matrix entries, proving faithfulness. With the [Lie algebra](../../../../../lie-algebra-split.md) basis

$$
D=\begin{pmatrix}1&0\\0&0\end{pmatrix},\qquad T=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad [D,T]=T,
$$

the left [Maurer-Cartan form](../../../../../maurer-cartan-form.md) is

$$
g^{-1}dg=\begin{pmatrix}da/a&db/a\\0&0\end{pmatrix}=\sigma^D D+\sigma^T T.
$$

The requested [left-invariant differential forms](../../../../../left-invariant-differential-form.md) therefore form the [Maurer-Cartan coframe of the real affine group](../../../../../maurer-cartan-coframe-of-the-real-affine-group.md):

$$
\boxed{\sigma^D=\frac{da}{a},\qquad\sigma^T=\frac{db}{a},\qquad d\sigma^D=0,\quad d\sigma^T=-\sigma^D\wedge\sigma^T.}
$$

For a direct invariance check, left translation by $(a_0,b_0)$ sends $(a,b)$ to $(a_0a,b_0+a_0b)$, and the pullbacks of the two displayed [differential forms](../../../../../differential-form-split.md) are unchanged. Their dual [left-invariant vector fields](../../../../../left-invariant-vector-field.md) are $a\partial_a$ and $a\partial_b$, whose bracket is $a\partial_b$, in agreement with $[D,T]=T$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
