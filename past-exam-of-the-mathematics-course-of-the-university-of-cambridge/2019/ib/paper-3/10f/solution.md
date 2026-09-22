<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

The [symmetric bilinear form associated with a quadratic form](../../../../../polarization-identity.md) is obtained by polarization:

$$
\boxed{\phi(u,v)=\frac12\bigl(q(u+v)-q(u)-q(v)\bigr)},
\qquad q(v)=\phi(v,v).
$$

To diagonalize it, argue by induction on $\dim V$. If $\phi(v,v)=0$ for every $v$, polarization gives $\phi=0$, so every basis works. Otherwise choose $e$ with $\phi(e,e)\ne0$. Then

$$
V=\operatorname{span}(e)\oplus e^\perp,
\qquad
v=\frac{\phi(v,e)}{\phi(e,e)}e+\left(v-\frac{\phi(v,e)}{\phi(e,e)}e\right),
$$

and diagonalize the restriction to $e^\perp$ inductively. Thus some basis gives a diagonal matrix with positive, negative, and zero entries. By [Sylvester's law of inertia](../../../../../sylvester-s-law-of-inertia.md), their counts $n_+,n_-,n_0$ are basis-independent. In the convention relevant here, the [signature of a quadratic form](../../../../../signature-of-a-quadratic-form.md) is

$$
\boxed{\operatorname{sig}(q)=n_+-n_-}.
$$

Suppose $R$ lies in the [radical of a bilinear form](../../../../../radical-of-a-bilinear-form.md), so $\phi(r,v)=0$ for all $r\in R,v\in V$. Then $q(r)=0$ and

$$
q(v+r)=q(v)+2\phi(v,r)+q(r)=q(v).
$$

Hence $q'(v+R)=q(v)$ is a well-defined quadratic form on the [quotient vector space](../../../../../quotient-vector-space.md) $V/R$. In an adapted diagonal basis, quotienting by $R$ merely removes zero diagonal directions, so $n_+$ and $n_-$, and therefore the signature, are unchanged.

Now let $W=\operatorname{span}(e,f)$. Its Gram matrix is

$$
\begin{pmatrix}0&1\\1&\phi(f,f)\end{pmatrix},
$$

which has determinant $-1$. Thus $W$ is nondegenerate and has one positive and one negative square: it is a [hyperbolic plane](../../../../../hyperbolic-plane-quadratic-form.md) and has signature zero. Nondegeneracy gives the orthogonal direct sum

$$
\boxed{V=W\oplus U,\qquad U=W^\perp}.
$$

Signature is additive under orthogonal direct sums, so

$$
\boxed{\operatorname{sig}(q|_U)=\operatorname{sig}(q)-\operatorname{sig}(q|_W)=\operatorname{sig}(q).}
$$

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
