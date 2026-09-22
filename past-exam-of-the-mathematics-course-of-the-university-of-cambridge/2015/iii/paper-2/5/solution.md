<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a complex [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) $\mathfrak g$, a [Cartan subalgebra](../../../../../cartan-subalgebra.md) $\mathfrak h$ is a maximal abelian subalgebra consisting of elements whose [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) matrices are diagonalizable. Equivalently it is a nilpotent self-normalizing [Lie subalgebra](../../../../../lie-subalgebra.md). The [root-space decomposition](../../../../../root-space-decomposition.md) is

$$
\mathfrak g=\mathfrak h\oplus\bigoplus_{\alpha\in R}\mathfrak g_\alpha,\qquad\mathfrak g_\alpha=\{x:[h,x]=\alpha(h)x\text{ for every }h\in\mathfrak h\},
$$

where the roots are the nonzero weights of that [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md).

We use these properties of the [Killing form](../../../../../killing-form.md) $B$: it is nondegenerate on $\mathfrak g$ and on $\mathfrak h$, it is invariant, distinct [root spaces](../../../../../root-space.md) are orthogonal unless their roots sum to zero, and $B$ pairs $\mathfrak g_\alpha$ nondegenerately with $\mathfrak g_{-\alpha}$. Define $t_\alpha$ by $B(t_\alpha,h)=\alpha(h)$, and choose $e\in\mathfrak g_\alpha$, $f\in\mathfrak g_{-\alpha}$ with $B(e,f)=1$. Since weights add, $[e,f]\in\mathfrak h$, and invariance gives

$$
B([e,f],h)=B(e,[f,h])=\alpha(h),\qquad[e,f]=t_\alpha.
$$

The [nonisotropic root lemma](../../../../../nonisotropic-root-lemma.md) shows $\alpha(t_\alpha)\ne0$. Here is its short proof: if this number were zero, the span of $e,f,t_\alpha$ would be a [solvable Lie algebra](../../../../../solvable-lie-algebra.md) with $t_\alpha$ central. Apply the [Lie theorem](../../../../../lie-s-theorem.md) to its action on $\mathfrak g$. The commutator $\operatorname{ad}t_\alpha=[\operatorname{ad}e,\operatorname{ad}f]$ would be strictly upper triangular and hence nilpotent. But $t_\alpha\in\mathfrak h$ makes it diagonalizable. It would therefore be zero, putting $t_\alpha$ in the zero [center of a Lie algebra](../../../../../center-of-a-lie-algebra.md) of $\mathfrak g$, contrary to its definition. Set

$$
H_\alpha=\frac{2t_\alpha}{\alpha(t_\alpha)},\qquad X_\alpha=e,\qquad Y_\alpha=\frac{2f}{\alpha(t_\alpha)}.
$$

Then

$$
\boxed{[H_\alpha,X_\alpha]=2X_\alpha,\quad[H_\alpha,Y_\alpha]=-2Y_\alpha,\quad[X_\alpha,Y_\alpha]=H_\alpha,}
$$

so their span is the [sl2 subalgebra associated with a root](../../../../../sl2-subalgebra-associated-with-a-root.md).

The abstract reduced [crystallographic root system](../../../../../crystallographic-root-system.md) axioms are as follows. In a finite-dimensional real [inner product space](../../../../../inner-product-space.md) $E$, the set $R$ is finite, consists of nonzero vectors and spans $E$; for every $\alpha\in R$, one has $R\cap\mathbb R\alpha=\{\alpha,-\alpha\}$; the [root reflection](../../../../../root-reflection.md) $s_\alpha(\beta)=\beta-2(\beta,\alpha)\alpha/(\alpha,\alpha)$ preserves $R$; and $2(\beta,\alpha)/(\alpha,\alpha)$ is an [integer](../../../../../integer.md) for every pair of roots. We verify the [positive-definite](../../../../../positive-definite-bilinear-form.md) real form as well as these axioms, rather than assuming the complex [Killing form](../../../../../killing-form.md) is already positive.

First $R$ is finite and has no zero element by its definition. The roots span $\mathfrak h^*$ over $\mathbb C$: any $h\in\mathfrak h$ annihilated by all roots commutes with the whole [root-space decomposition](../../../../../root-space-decomposition.md) and is central, hence zero. Therefore the $t_\alpha$, and also the $H_\alpha$, span $\mathfrak h$ over $\mathbb C$. For every root $\beta$, the [classification of finite-dimensional sl2 representations](../../../../../classification-of-finite-dimensional-sl2-representations.md) applied to the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) of the root subalgebra gives $\beta(H_\alpha)\in\mathbb Z$. Put $\mathfrak h_{\mathbb R}=\operatorname{span}_{\mathbb R}\{H_\alpha:\alpha\in R\}$. Every root takes real values on this space, and

$$
B(h,h)=\operatorname{tr}((\operatorname{ad}h)^2)=\sum_{\beta\in R}(\dim\mathfrak g_\beta)\beta(h)^2>0\qquad(0\ne h\in\mathfrak h_{\mathbb R}).
$$

The strict inequality follows because the roots span $\mathfrak h^*$. This also shows that the complexification of $\mathfrak h_{\mathbb R}$ injects into $\mathfrak h$: an equality $h_1+ih_2=0$ with real $h_j$ would contradict positivity of $B(h_1,h_1)$ and $B(h_2,h_2)$. Since its complex span is all of $\mathfrak h$, it is a real form. Moreover $B(H_\alpha,H_\alpha)=4/\alpha(t_\alpha)>0$, so $t_\alpha$ is a real scalar multiple of $H_\alpha$. The dual [inner product](../../../../../inner-product.md) thus makes $E=\operatorname{span}_{\mathbb R}R$ a Euclidean space, as in the [Euclidean subspace of a Cartan subalgebra](../../../../../euclidean-subspace-of-a-cartan-subalgebra.md).

To prove reducedness without assuming it, consider the root-subalgebra module

$$
M_\alpha=\mathfrak h\oplus\bigoplus_{j\in\mathbb Z\setminus\{0\}}\mathfrak g_{j\alpha},
$$

with absent [root spaces](../../../../../root-space.md) understood to be zero. Its $H_\alpha$ weights are even, so every nontrivial [Irreducible Lie algebra representation](../../../../../irreducible-lie-algebra-representation.md) in it has even positive [highest weight](../../../../../highest-weight-of-a-representation.md) and one-dimensional weight-zero space. The action of $X_\alpha$ on its weight-zero space $\mathfrak h$ has image exactly $\mathbb C X_\alpha$, of dimension one. Therefore there is precisely one nontrivial irreducible summand, the already embedded adjoint $\mathfrak{sl}_2$ module of highest weight $2$. Thus $\dim\mathfrak g_\alpha=1$ and $2\alpha\notin R$. If $\beta=c\alpha$ is any root on the same real line, the integral numbers $\beta(H_\alpha)=2c$ and $\alpha(H_\beta)=2/c$ have product $4$. Hence $c$ is one of $\pm\tfrac12,\pm1,\pm2$; the half and double cases are excluded by applying the preceding argument to the appropriate root. This proves the [root-space reducedness lemma](../../../../../root-space-reducedness-lemma.md) and $R\cap\mathbb R\alpha=\{\pm\alpha\}$.

For a root $\beta$ not parallel to $\alpha$, the sum of [root spaces](../../../../../root-space.md) $\bigoplus_{j\in\mathbb Z}\mathfrak g_{\beta+j\alpha}$ is stable under the root $\mathfrak{sl}_2$. Its integer $H_\alpha$ weights are symmetric under sign in each irreducible summand. Therefore the weight $-\beta(H_\alpha)$ also occurs, at the root $\beta-\beta(H_\alpha)\alpha$. The [Killing form](../../../../../killing-form.md) normalization gives

$$
\beta(H_\alpha)=\frac{2(\beta,\alpha)}{(\alpha,\alpha)},
$$

so this root is exactly $s_\alpha(\beta)$. For $\beta=\pm\alpha$ the reflection just swaps the two roots. This proves reflection invariance and the [Cartan integer](../../../../../cartan-integer.md) condition. All axioms of the reduced [crystallographic root system](../../../../../crystallographic-root-system.md) have now been verified.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
