<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Work with integral [cohomology](../../../../../cohomology-split.md). For a frame $v=(v_1,\ldots,v_k)$ in the [complex Stiefel manifold](../../../../../complex-stiefel-manifold.md), define

$$
E_v=\{w\in\mathbb C^n:\langle w,v_i\rangle=0\text{ for every }i\}.
$$

These fibres form the [complement bundle on a complex Stiefel manifold](../../../../../complement-bundle-on-a-complex-stiefel-manifold.md), a complex [vector subbundle](../../../../../vector-subbundle.md) of the trivial rank-$n$ bundle. Indeed

$$
P_v=I-\sum_{i=1}^k v_iv_i^*
$$

is a smooth orthogonal projector of constant complex rank $n-k$; locally projecting suitable fixed basis vectors and applying [Gram-Schmidt process](../../../../../gram-schmidt-process.md) provides bundle frames. The underlying real [vector bundle](../../../../../vector-bundle.md) has rank $r=2(n-k)$ and is oriented by its complex structure: a complex change of frame has real determinant equal to the positive number $|\det_{\mathbb C}A|^2$.

A point of its [sphere bundle](../../../../../sphere-bundle.md) is $(v_1,\ldots,v_k,w)$ with $\|w\|=1$ and $w$ orthogonal to the frame. Appending $w$ gives a diffeomorphism

$$
\boxed{S(E)\cong V_{k+1}(\mathbb C^n),}
$$

whose inverse forgets the last vector while retaining it as the unit vector in the complement. Thus the asserted homotopy equivalence is actually an identification of sphere bundles, for $0\leq k<n$.

Start the induction at $V_0(\mathbb C^n)=\{\mathrm{point}\}$, with cohomology the exterior algebra on no generators. Suppose

$$
H^*(V_k(\mathbb C^n);\mathbb Z)=\Lambda_{\mathbb Z}(a_{2n-1},a_{2n-3},\ldots,a_{2n-2k+1}).
$$

This is a free abelian group in every degree, and for $k\geq1$ its smallest positive degree is $2n-2k+1=r+1$. Hence $H^r(V_k;\mathbb Z)=0$. This vanishing holds at $k=0$ as well, since the base is a point and $r=2n>0$. The [Euler class](../../../../../euler-class-of-a-vector-bundle.md) $e(E)$ belongs to this zero group and is therefore zero.

For this oriented rank-$r$ [vector bundle](../../../../../vector-bundle.md), the [Gysin sequence of a sphere bundle](../../../../../gysin-sequence-of-a-sphere-bundle.md) has segment

$$
H^{j-r}(V_k)\xrightarrow{\smile e(E)}H^j(V_k)\xrightarrow{\pi^*}H^j(V_{k+1})\xrightarrow{\pi_!}H^{j-r+1}(V_k)\xrightarrow{\smile e(E)}H^{j+1}(V_k).
$$

Because $e(E)=0$, this becomes

$$
0\longrightarrow H^j(V_k)\xrightarrow{\pi^*}H^j(V_{k+1})\xrightarrow{\pi_!}H^{j-r+1}(V_k)\longrightarrow0.
$$

In particular $H^*(V_{k+1};\mathbb Z)$ is torsion-free. At $j=r-1$, choose a class $a\in H^{r-1}(V_{k+1};\mathbb Z)$ with $\pi_!a=1$. Its restriction to the sphere fibre is an integral generator. The [projection formula for sphere bundle integration](../../../../../projection-formula-for-sphere-bundle-integration.md), with the conventional fibre-integration sign, is

$$
\pi_!(\pi^*b\smile a)=b\smile\pi_!a=b.
$$

It can be obtained from the relative cohomology of the disk/sphere pair and the [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md). Consequently every cohomology class of $V_{k+1}$ is uniquely expressible as $\pi^*c+\pi^*b\smile a$: subtract the second term using its fibre integral, then use exactness to identify the remaining term; injectivity of $\pi^*$ and the projection formula prove uniqueness. This establishes an additive splitting by the old monomials and the old monomials multiplied by $a$.

To establish the ring, $|a|=r-1$ is odd, so [graded commutativity of the cup product](../../../../../graded-commutativity-of-the-cup-product.md) gives $a^2=-a^2$, and hence $2a^2=0$. The torsion-freeness just proved now gives $a^2=0$. Graded commutativity also gives the required anticommutation with each old odd generator, and the old relations persist under the injective ring map $\pi^*$. The additive splitting proves that there are no additional relations. This is exactly [Gysin ring splitting for an odd-dimensional sphere bundle](../../../../../gysin-ring-splitting-for-an-odd-dimensional-sphere-bundle.md), and supplies a new exterior generator of degree

$$
r-1=2n-2k-1.
$$

Induction therefore proves the full ring calculation

$$
\boxed{H^*(V_k(\mathbb C^n);\mathbb Z)\cong\Lambda_{\mathbb Z}(a_{2n-1},a_{2n-3},\ldots,a_{2n-2k+1}),\qquad 0\leq k\leq n.}
$$

Over $\mathbb Z$, graded commutativity by itself only kills twice an odd square; torsion-freeness is the essential extra step in this [integral cohomology of a complex Stiefel manifold](../../../../../integral-cohomology-of-a-complex-stiefel-manifold.md) proof.

Finally an ordered orthonormal $n$-frame is a [unitary matrix](../../../../../unitary-matrix.md), so $V_n(\mathbb C^n)=U(n)$. Each exterior generator may be included once or omitted from a basis monomial. The rank of degree $j$ is therefore the number of subsets of the generator degrees $1,3,\ldots,2n-1$ summing to $j$. Multiplication of their two-term generating factors gives

$$
\boxed{\sum_{j\geq0}b_j(U(n))t^j=\prod_{i=0}^{n-1}(1+t^{2i+1}).}
$$

The highest exponent is $1+3+\cdots+(2n-1)=n^2$, agreeing with the real dimension of the [unitary group](../../../../../unitary-group.md), and the total rank is $2^n$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
