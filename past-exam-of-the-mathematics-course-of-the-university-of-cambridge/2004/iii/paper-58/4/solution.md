<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use ambient [quadratic form](../../../../../quadratic-form.md) $Q=-(X^0)^2-(X^4)^2+(X^1)^2+(X^2)^2$. The printed sine coordinate has a duplicated superscript: it must be $X^2$, not another $X^1$. With that correction the embedding lies on $Q=-1$. Put $s=\sqrt{1+r^2}$. Differentiating the two timelike coordinates gives

$$
(dX^0)^2+(dX^4)^2=\frac{r^2}{1+r^2}\,dr^2+(1+r^2)\,dt^2,
$$

whereas the two spatial coordinates give $(dX^1)^2+(dX^2)^2=dr^2+r^2d\theta^2$. Their difference is the induced [Lorentzian metric](../../../../../lorentzian-metric.md)

$$
g=-(1+r^2)\,dt^2+\frac{dr^2}{1+r^2}+r^2d\theta^2.
$$

The polar coordinate $\theta$ collapses at $r=0$; this is a coordinate degeneracy, not a degeneracy of the metric.

For the [matrix model of anti-de Sitter three-space](../../../../../matrix-model-of-anti-de-sitter-three-space.md), define

$$
M(X)=\begin{pmatrix}X^4+X^1&X^2+X^0\\X^2-X^0&X^4-X^1\end{pmatrix}.
$$

Then $\det M=-Q$. This linear identification of ambient space with real two-by-two matrices identifies $Q=-1$ with $SL(2,\mathbb R)$. Its inverse recovers each $X$ by sums and differences of matrix entries, so the identification is global. The identity corresponds to $X^4=1$ and the other coordinates zero. For a traceless tangent matrix $U$, the induced squared norm is

$$
g_I(U,U)=-\det U=\tfrac12\operatorname{tr}(U^2).
$$

Polarization gives $g_I(U,V)=\tfrac12\operatorname{tr}(UV)$.

The [Killing form](../../../../../killing-form.md) of $\mathfrak{sl}_2(\mathbb R)$ is $B(U,V)=4\operatorname{tr}(UV)$. This normalization can be checked without assuming it: for $H=\operatorname{diag}(1,-1)$, $E=\left(\begin{smallmatrix}0&1\\0&0\end{smallmatrix}\right)$ and $F=\left(\begin{smallmatrix}0&0\\1&0\end{smallmatrix}\right)$, the brackets are $[H,E]=2E$, $[H,F]=-2F$, $[E,F]=H$. Taking traces of their three-dimensional adjoint matrices gives $B(H,H)=8$, $B(E,F)=B(F,E)=4$, and all other basis pairings zero. These agree with $4\operatorname{tr}(UV)$.

Both left and right multiplication by matrices in $SL(2,\mathbb R)$ preserve $-\det M$, hence its polarized ambient [bilinear form](../../../../../bilinear-form.md) and the induced metric. Equality at the identity therefore propagates throughout the group:

$$
\boxed{g=\tfrac18 B.}
$$

In particular the [Killing-form Einstein metric](../../../../../killing-form-einstein-metric.md) calculation gives $\operatorname{Ric}=-2g$, consistent with unit-radius three-dimensional [Anti-de Sitter spacetime](../../../../../anti-de-sitter-spacetime.md).

Every element of $SO(2,2)$ preserves the ambient [quadratic form](../../../../../quadratic-form.md), hence the hyperboloid and its induced metric, and so acts by [isometries](../../../../../isometry.md). Define the [left-right double cover of SO0(2,2)](../../../../../left-right-double-cover-of-so0-2-2.md) by

$$
\Phi(A,B)(M)=AMB^{-1},\qquad A,B\in SL(2,\mathbb R).
$$

This is a [group homomorphism](../../../../../group-homomorphism.md), since successive actions multiply the two factors in the same order. It preserves $\det M$; as a transformation of the four-dimensional matrix space it has determinant $(\det A)^2(\det B^{-1})^2=1$. Thus it takes values in $SO(2,2)$.

If its action is the identity, applying it to $M=I$ gives $A=B$. Commuting with every matrix then forces $A$ to be scalar. The condition $\det A=1$ leaves only $A=I$ or $A=-I$. Hence

$$
\ker\Phi=\{(I,I),(-I,-I)\}.
$$

The differential is $(a,b):M\mapsto aM-Mb$. A zero differential implies $a=b$ and that $a$ is scalar; tracelessness makes $a=b=0$. It is therefore an isomorphism onto the target [Lie algebra](../../../../../lie-algebra-split.md), since both dimensions are six. The image is an open subgroup. Since $SL(2,\mathbb R)$ is connected, the image is connected and is exactly the [identity component](../../../../../identity-component.md) $SO_0(2,2)$: an open subgroup of a connected group is also closed and must be the whole group. Thus the precise covering statement is

$$
\boxed{SO_0(2,2)\cong\big(SL(2,\mathbb R)\times SL(2,\mathbb R)\big)/\{\pm(I,I)\}.}
$$

It is not onto the disconnected full $SO(2,2)$. For example, conjugation $M\mapsto DMD^{-1}$, $D=\operatorname{diag}(1,-1)$, sends $(X^0,X^4,X^1,X^2)$ to $(-X^0,X^4,X^1,-X^2)$ and belongs to the other component of $SO(2,2)$. It reverses the orientation of the negative two-plane and is not in the image of the connected source.

The [Adjoint representation of a Lie group](../../../../../adjoint-representation-of-a-lie-group.md) of $SL(2,\mathbb R)$ preserves its [Killing form](../../../../../killing-form.md) of [metric signature](../../../../../metric-signature.md) $(2,1)$ and gives a second double cover,

$$
\boxed{SL(2,\mathbb R)/\{\pm I\}\cong SO_0(2,1).}
$$

Its kernel is the scalar centre; its differential is injective and both dimensions are three, so the same connected-image argument proves surjectivity onto the identity component. The full $SO(2,1)$ again has an additional component. Thus $SO_0(2,1)$ is locally the same [Lie group](../../../../../lie-group.md) geometry as $SL(2,\mathbb R)$, with its [Killing metric](../../../../../killing-form-einstein-metric.md), and globally is its central quotient.

With the printed periodic time, the group model has topology $S^1\times\mathbb R^2$ and closed timelike curves, since varying $t$ at fixed spatial position gives a timelike circle. The causally unwrapped version of [Anti-de Sitter spacetime](../../../../../anti-de-sitter-spacetime.md) instead has $t\in\mathbb R$ and is the [universal covering Lie group](../../../../../universal-covering-lie-group.md). It must not be substituted silently for the periodic spacetime specified here.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
