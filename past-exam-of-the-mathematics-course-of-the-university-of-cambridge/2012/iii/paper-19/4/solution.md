<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The multiplicative [norm](../../../../../norm.md) first rules out [zero divisors](../../../../../zero-divisor.md): if $xy=0$ and $x\neq0$, then $0=|x||y|$ forces $y=0$. If the dimension is zero the claimed bound already holds, so suppose it is positive.

It is worth checking that the printed description of a ring with an underlying real [vector space](../../../../../vector-space-split.md) really permits differentiation of multiplication. This follows from the norm identity even if compatibility with real scalars is not separately stated. For fixed $x$, the map $L_x(y)=xy$ is additive by distributivity, and

$$
|L_x(y)-L_x(z)|=|x(y-z)|=|x||y-z|.
$$

It is therefore [continuous](../../../../../continuous-function.md). Additivity gives rational linearity. Approximating a real number by rationals and using continuity proves $L_x(ty)=tL_x(y)$ for every real $t$. The same argument holds in the other variable. This is [automatic real bilinearity from a multiplicative norm](../../../../../automatic-real-bilinearity-from-a-multiplicative-norm.md), so multiplication is a [bilinear map](../../../../../bilinear-map.md) between finite-dimensional [vector spaces](../../../../../vector-space-split.md), and hence is smooth.

Let $S=\{x\in A:|x|=1\}$ be the [unit sphere](../../../../../unit-sphere.md) of the given [positive-definite bilinear form](../../../../../positive-definite-bilinear-form.md). It is a copy of $S^{n-1}$. The squaring map

$$
Q:S\to S,\qquad Q(x)=x^2,
$$

is well defined because $|x^2|=|x|^2=1$, and is smooth. [Commutativity](../../../../../commutativity.md) gives its derivative

$$
DQ_x(v)=xv+vx=2xv.
$$

For $x\in S$ and $v\neq0$, the norm identity gives $|DQ_x(v)|=2|v|$, so the derivative is injective, including on the [tangent space](../../../../../tangent-space.md) $T_xS=x^\perp$. It takes tangent vectors into $T_{x^2}S$ since $Q$ maps the [sphere](../../../../../sphere.md) to itself. Alternatively, polarization of $|xy|^2=|x|^2|y|^2$ gives $\langle xy,xz\rangle=|x|^2\langle y,z\rangle$, so $\langle x^2,2xv\rangle=2\langle x,v\rangle=0$ directly.

The only identifications under squaring are antipodal:

$$
Q(x)=Q(y)\ \Longrightarrow\ (x-y)(x+y)=0\ \Longrightarrow\ y=x\text{ or }y=-x.
$$

The factorization uses [commutativity](../../../../../commutativity.md), and the last implication uses the absence of [zero divisors](../../../../../zero-divisor.md). Conversely $Q(-x)=Q(x)$. It follows that $Q$ induces an injective smooth map

$$
q:\mathbb{RP}^{n-1}=S/(x\sim-x)\longrightarrow S^{n-1}.
$$

The antipodal [quotient map](../../../../../quotient-map.md) is a local [diffeomorphism](../../../../../diffeomorphism.md), so the injectivity of $DQ$ implies injectivity of $Dq$. Since [Real projective space](../../../../../real-projective-space.md) is [compact](../../../../../compact-space.md), the stated [compact injective immersion is an embedding](../../../../../compact-injective-immersion-is-an-embedding.md) theorem makes $q$ a closed embedding.

For $n\geq2$ its source and target have the same dimension $n-1$. The [inverse function theorem](../../../../../inverse-function-theorem.md) makes its image open as well as closed in the connected [sphere](../../../../../sphere.md) $S^{n-1}$. It is nonempty, so the image is the whole [sphere](../../../../../sphere.md); consequently $q$ is a [diffeomorphism](../../../../../diffeomorphism.md). But for $n\geq3$ this is impossible:

$$
\pi_1(\mathbb{RP}^{n-1})\cong\mathbb Z/2,
\qquad \pi_1(S^{n-1})=0.
$$

Indeed, the antipodal two-sheeted [covering map](../../../../../covering-space.md) $S^{n-1}\to\mathbb{RP}^{n-1}$ has simply connected total space in this range, and is its [universal cover](../../../../../universal-cover.md), with deck group $\mathbb Z/2$. A [sphere](../../../../../sphere.md) of dimension at least two is [simply connected](../../../../../simply-connected-space.md). These [fundamental groups](../../../../../fundamental-group.md) cannot be those of homeomorphic spaces.

We have obtained the [dimension bound for a commutative Euclidean normed algebra](../../../../../dimension-bound-for-a-commutative-euclidean-normed-algebra.md):

$$
\boxed{\dim_{\mathbb R}A\leq2.}
$$

The real numbers and complex numbers with their usual products and Euclidean norms attain dimensions one and two. In dimension two, the induced map $\mathbb{RP}^1\to S^1$ is entirely compatible with the argument: the [circle](../../../../../circle.md) squaring map identifies exactly the two antipodal preimages. We neither assume a multiplicative identity nor use a classification of real division algebras; the squaring argument proves the bound from the supplied hypotheses.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
