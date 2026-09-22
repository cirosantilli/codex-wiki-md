<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work over $\mathbb R$ or $\mathbb C$, in finite dimension and characteristic zero. The [Killing form](../../../../../killing-form.md) of a [Lie algebra](../../../../../lie-algebra-split.md) is the trace form of its [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md):

$$
\boxed{\kappa(x,y)=\operatorname{tr}(\operatorname{ad}_x\operatorname{ad}_y),\qquad\operatorname{ad}_x(z)=[x,z].}
$$

It is bilinear and symmetric by the [cyclic property of the trace](../../../../../cyclic-property-of-the-trace.md). It is an [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md), since the [Jacobi identity](../../../../../jacobi-identity.md) gives $\operatorname{ad}_{[x,y]}=[\operatorname{ad}_x,\operatorname{ad}_y]$ and hence

$$
\begin{aligned}
\kappa([x,y],z)
&=\operatorname{tr}([\operatorname{ad}_x,\operatorname{ad}_y]\operatorname{ad}_z)\\
&=\operatorname{tr}(\operatorname{ad}_x[\operatorname{ad}_y,\operatorname{ad}_z])
=\kappa(x,[y,z]).
\end{aligned}
$$

Equivalently, $\kappa([z,x],y)+\kappa(x,[z,y])=0$. A Lie algebra automorphism preserves the form, because it conjugates the adjoint matrices. Its [radical of a bilinear form](../../../../../radical-of-a-bilinear-form.md) $\mathfrak r_\kappa=\{x:\kappa(x,\mathfrak g)=0\}$ is an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md) by invariance. The [center of a Lie algebra](../../../../../center-of-a-lie-algebra.md) lies in this radical, so the form vanishes for an abelian algebra. On a direct sum of ideals the summands are orthogonal and the form restricts to their own Killing forms.

A short argument proves the requested implication without assuming the [Cartan criterion for semisimplicity](../../../../../cartan-criterion-for-semisimplicity.md). Let $\mathfrak a$ be an abelian [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md), $x\in\mathfrak a$, and $y\in\mathfrak g$. The map $\operatorname{ad}_x$ takes $\mathfrak g$ into $\mathfrak a$ and vanishes on $\mathfrak a$, while $\operatorname{ad}_y$ preserves $\mathfrak a$. Therefore $\operatorname{ad}_x\operatorname{ad}_y$ has image in $\mathfrak a$ and is zero on $\mathfrak a$. In a basis extending a basis of $\mathfrak a$, both diagonal blocks are zero, so its trace vanishes. This proves that [abelian ideals lie in the radical of the Killing form](../../../../../abelian-ideals-lie-in-the-radical-of-the-killing-form.md).

If the [solvable radical](../../../../../radical-of-a-lie-algebra.md) $\mathfrak r$ were nonzero, its [derived series of a Lie algebra](../../../../../derived-series-of-a-lie-algebra.md) would have a last nonzero term $\mathfrak a$. The [Jacobi identity](../../../../../jacobi-identity.md) makes every derived term an ideal of $\mathfrak g$, and the last one is abelian. Thus $0\ne\mathfrak a\subseteq\mathfrak r_\kappa$, contradicting nondegeneracy. We obtain

$$
\boxed{\kappa\text{ nondegenerate}\ \Longrightarrow\ \mathfrak r=0\ \Longrightarrow\ \mathfrak g\text{ is a semisimple Lie algebra}.}
$$

The converse holds as well in characteristic zero; together these implications are the [Cartan criterion for semisimplicity](../../../../../cartan-criterion-for-semisimplicity.md).

For a complex [simple Lie algebra](../../../../../simple-lie-algebra.md), that criterion gives nondegeneracy on $\mathfrak g$. Let $\mathfrak h$ be a [Cartan subalgebra](../../../../../cartan-subalgebra.md). Use the standard [root-space decomposition](../../../../../root-space-decomposition.md)

$$
\mathfrak g=\mathfrak h\oplus\bigoplus_{\alpha\in\Phi}\mathfrak g_\alpha,
\qquad[h,e_\alpha]=\alpha(h)e_\alpha.
$$

For $h,h'\in\mathfrak h$ and a [root vector](../../../../../root-vector.md) $e_\alpha$, choose $t\in\mathfrak h$ with $\alpha(t)\ne0$. Invariance gives

$$
\alpha(t)\kappa(h,e_\alpha)=\kappa(h,[t,e_\alpha])=\kappa([h,t],e_\alpha)=0.
$$

Thus $\mathfrak h$ is orthogonal to every nonzero [root space](../../../../../root-space.md). If $h\in\mathfrak h$ is also orthogonal to $\mathfrak h$, it is orthogonal to all of $\mathfrak g$ and hence is zero. This establishes [nondegeneracy of the Killing form on a Cartan subalgebra](../../../../../nondegeneracy-of-the-killing-form-on-a-cartan-subalgebra.md):

$$
\boxed{\kappa|_{\mathfrak h\times\mathfrak h}\text{ is nondegenerate}.}
$$

The same invariance calculation shows that $\kappa(\mathfrak g_\alpha,\mathfrak g_\beta)=0$ unless $\alpha+\beta=0$. Opposite root spaces are therefore paired nondegenerately. Tracing the adjoint action on the root-space decomposition yields

$$
\kappa(h,h')=\sum_{\alpha\in\Phi}\alpha(h)\alpha(h'),
$$

since the root spaces of a complex semisimple algebra are one-dimensional and its adjoint action on $\mathfrak h$ is zero.

The relevant [Euclidean subspace of a Cartan subalgebra](../../../../../euclidean-subspace-of-a-cartan-subalgebra.md) is

$$
\mathfrak h_{\mathbb R}=\operatorname{span}_{\mathbb R}\{h_{\alpha_1},\ldots,h_{\alpha_\ell}\}
=\{h\in\mathfrak h:\alpha(h)\in\mathbb R\text{ for all }\alpha\in\Phi\},
$$

where the $h_{\alpha_i}$ are the simple [coroots](../../../../../coroot.md), normalized by $\alpha_i(h_{\alpha_i})=2$. The standard Euclidean property is that $\kappa$ is real and positive definite on this space. The displayed trace formula explains it: $\kappa(h,h)$ is a sum of real squares, and the roots span $\mathfrak h^*$, so all squares vanish only for $h=0$. Via the nondegenerate form, the roots can consequently be regarded as vectors in a real [Euclidean normed vector space](../../../../../euclidean-norm.md). The induced dual [inner product](../../../../../inner-product.md) makes [root reflections](../../../../../root-reflection.md) orthogonal and allows root lengths and angles to be encoded by [Cartan integers](../../../../../cartan-integer.md) and the [Dynkin diagram](../../../../../dynkin-diagram.md).

This positivity is on a specified real subspace; the complex Killing form is a bilinear form, not a positive [Hermitian inner product](../../../../../hermitian-form.md). On a [compact real form](../../../../../compact-real-form-of-a-complex-semisimple-lie-algebra.md) the Killing form is instead negative definite. For example the [Killing form of the special linear Lie algebra](../../../../../killing-form-of-the-special-linear-lie-algebra.md) gives $\kappa(X,Y)=4\operatorname{tr}(XY)$ for $\mathfrak{sl}_2$, so $\kappa(L_0,L_0)=8$ but $\kappa(iL_0,iL_0)=-8$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
