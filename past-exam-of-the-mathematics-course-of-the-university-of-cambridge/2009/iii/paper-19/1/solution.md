<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [almost complex structure](../../../../../almost-complex-manifold.md) is a smooth real [bundle endomorphism](../../../../../vector-bundle-endomorphism.md) $J:TM\to TM$ satisfying $J^2=-I$. In particular the real dimension is even, say $2m$. After complexifying, the [type decomposition of the complexified tangent bundle](../../../../../type-decomposition-of-the-complexified-tangent-bundle.md) is

$$
T_{\mathbb C}M=T^{1,0}M\oplus T^{0,1}M,
\qquad T^{1,0}M=\ker(J-i),\quad T^{0,1}M=\ker(J+i).
$$

The corresponding [differential forms of type (p, q)](../../../../../differential-form-of-type-p-q.md) are smooth sections of $\Lambda^p(T^{1,0}M)^*\otimes\Lambda^q(T^{0,1}M)^*$, regarded as alternating forms by the [wedge product of differential forms](../../../../../wedge-product-of-differential-forms.md). A form of type $(p,q)$ vanishes unless its arguments include $p$ vectors of type $(1,0)$ and $q$ of type $(0,1)$.

Besides vanishing of the [Nijenhuis tensor](../../../../../nijenhuis-tensor.md), two equivalent descriptions of an [integrable almost complex structure](../../../../../integrable-almost-complex-structure.md) are: the smooth sections of $T^{0,1}M$ are closed under [Lie bracket](../../../../../lie-bracket.md); and every point has complex coordinates in which $J$ is multiplication by $i$, with [holomorphic](../../../../../complex-differentiability-at-a-point.md) changes of coordinates. The equivalence with existence of these coordinates is the [Newlander-Nirenberg theorem](../../../../../newlander-nirenberg-theorem.md) for smooth $J$. A further equivalent condition is that the [exterior derivative](../../../../../exterior-derivative.md) has only the two type components $d=\partial+\bar\partial$, with no components of bidegree $(2,-1)$ or $(-1,2)$. Indeed evaluation of $d$ of a $(1,0)$-form on two $(0,1)$ vector fields detects the $(1,0)$ component of their bracket; [complex conjugation](../../../../../complex-conjugation.md) detects the other component.

For the [almost complex structure induced by a complex atlas](../../../../../almost-complex-structure-induced-by-a-complex-atlas.md), write $z^j=x^j+iy^j$ and put $J\partial_{x^j}=\partial_{y^j}$, $J\partial_{y^j}=-\partial_{x^j}$. The differentials of [holomorphic](../../../../../complex-differentiability-at-a-point.md) transition maps are complex linear, so these local definitions agree. In these coordinates $J$ has constant coefficients and all coordinate vector fields commute. The expression defining the [Nijenhuis tensor](../../../../../nijenhuis-tensor.md) is tensorial, so evaluating it on this frame proves it is zero everywhere. Thus the induced structure is integrable.

Here is a direct proof for the [smooth submanifolds with invariant complex tangent spaces are complex](../../../../../smooth-submanifolds-with-invariant-complex-tangent-spaces-are-complex.md) assertion. At a point of $Y$, its [tangent space](../../../../../tangent-space.md) is a complex-linear subspace, of real dimension $2k$. Make a complex-linear change of ambient [holomorphic coordinates](../../../../../holomorphic-coordinate.md) so that this [tangent space](../../../../../tangent-space.md) is $\mathbb C^k\times0$. Projection onto the first $k$ coordinates has invertible real differential on $Y$. The real [inverse function theorem](../../../../../inverse-function-theorem.md) states that a smooth map between equal-dimensional manifolds with invertible differential is a [diffeomorphism](../../../../../diffeomorphism.md) on sufficiently small neighbourhoods. It therefore writes $Y$ locally as a smooth graph $w=F(z)$ over an open set in $\mathbb C^k$.

A tangent vector to this graph is $(v,dF(v))$. Its image under $J$ is $(iv,i\,dF(v))$. Tangent-space invariance implies

$$
dF(iv)=i\,dF(v),
$$

so $F$ satisfies the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md). Smooth functions satisfying these equations are [holomorphic](../../../../../complex-differentiability-at-a-point.md): restrict to each coordinate complex line, use the one-variable criterion, and apply the iterated Cauchy integral formula on a small polydisc to get jointly [holomorphic](../../../../../complex-differentiability-at-a-point.md) coefficients. Hence the graph parametrization is [holomorphic](../../../../../complex-differentiability-at-a-point.md). Restrictions of ambient [holomorphic coordinates](../../../../../holomorphic-coordinate.md) supply [holomorphic](../../../../../complex-differentiability-at-a-point.md) transition maps between these graph charts. **The restricted structure on $Y$ is an integrable [complex structure](../../../../../complex-structure.md).** This also proves the induced structure agrees with the original restriction, rather than merely producing some [complex structure](../../../../../complex-structure.md) on $Y$.

A [nonsingular analytic subvariety](../../../../../nonsingular-analytic-subvariety.md) is a closed analytic subset which near each of its points is the zero set of a [holomorphic](../../../../../complex-differentiability-at-a-point.md) submersion of constant rank; equivalently, it is locally a coordinate subspace in [holomorphic coordinates](../../../../../holomorphic-coordinate.md). The [holomorphic implicit function theorem](../../../../../holomorphic-implicit-function-theorem.md) says that if a [holomorphic map](../../../../../holomorphic-map.md) to $\mathbb C^r$ has differential of rank $r$ at a zero, its nearby zero set is a complex submanifold of codimension $r$.

The homogeneous equation defines a subset of [Complex projective space](../../../../../complex-projective-space.md) because multiplying a vector by $\lambda\ne0$ multiplies its quadratic value by $\lambda^2$. Its gradient on $\mathbb C^4$ is $2Qz$, which is nonzero for $z\ne0$. More explicitly, in an affine chart set $z_i=1$. If all derivatives of the restricted equation vanished at one of its zeros, all components of $2Qz$ except possibly the $i$th would vanish. The [Euler homogeneous function theorem](../../../../../euler-theorem-for-homogeneous-functions.md) gives $\sum_j z_j\partial_jp=2p=0$, forcing the remaining component to vanish as well. This contradicts invertibility of $Q$. The [holomorphic implicit function theorem](../../../../../holomorphic-implicit-function-theorem.md) thus proves **$S$ is a smooth complex surface**.

To see its geometry, reduce the nondegenerate symmetric bilinear form to diagonal form over $\mathbb C$. There is a vector of nonzero self-pairing, since otherwise polarization would make the entire form zero. Normalize such a vector using a square root of its self-pairing. Its [orthogonal complement](../../../../../orthogonal-complement.md) remains nondegenerate, so induction gives an orthonormal basis. Apply the same argument to the nondegenerate form $w_0w_3-w_1w_2$: the two forms are equivalent under an invertible linear change of variables. The allowed [projective linear transformation](../../../../../projective-linear-transformation.md) therefore reduces $S$ to

$$
Q_0=\{[w_0:w_1:w_2:w_3]:w_0w_3-w_1w_2=0\}.
$$

View its coordinates as the nonzero rank-one matrix $A=\begin{pmatrix}w_0&w_1\\w_2&w_3\end{pmatrix}=uv^T$. At $[A]$, holding $[u]$ fixed and varying $[v]$ gives a [projective line](../../../../../projective-line.md), and holding $[v]$ fixed and varying $[u]$ gives another. They are distinct and meet at $[A]$. In fact these are the only lines through it: if a second rank-one matrix is $ab^T$, the entire pencil has determinant zero only if $\det(u,a)\det(v,b)=0$, so one projective factor is fixed. These are the two [rulings of a smooth quadric surface](../../../../../rulings-of-a-smooth-quadric-surface.md).

The [Segre embedding](../../../../../segre-embedding.md) is the [holomorphic map](../../../../../holomorphic-map.md)

$$
\Phi:\mathbb{CP}^1\times\mathbb{CP}^1\longrightarrow Q_0,
\qquad([u_0:u_1],[v_0:v_1])\longmapsto[u_0v_0:u_0v_1:u_1v_0:u_1v_1].
$$

Every nonzero rank-one matrix has such a factorization, unique up to reciprocal rescaling, so $\Phi$ is bijective. Its inverse is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on each open set where a matrix entry $a_{ij}\ne0$: the projective column $[a_{0j}:a_{1j}]$ recovers $[u]$, and the projective row $[a_{i0}:a_{i1}]$ recovers $[v]$. These formulas agree on overlaps. Thus the [Segre description of a smooth quadric surface](../../../../../segre-description-of-a-smooth-quadric-surface.md) gives the promised stronger conclusion

$$
\boxed{S\cong\mathbb{CP}^1\times\mathbb{CP}^1\quad\text{biholomorphically}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
