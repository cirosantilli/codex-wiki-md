<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $u_n$ be the rationalized universal class of degree $n$. **The [rational cohomology of an integral Eilenberg–MacLane space](../../../../../rational-cohomology-of-an-integral-eilenberg-maclane-space.md) is**

$$
\boxed{H^*(K(\mathbb Z,n);\mathbb Q)\cong
\begin{cases}
\Lambda_{\mathbb Q}(u_n),&n\text{ odd},\\
\mathbb Q[u_n],&n\text{ even}.
\end{cases}}
$$

Here $\Lambda$ is an [exterior algebra](../../../../../exterior-algebra.md). For $n=1$, $K(\mathbb Z,1)\simeq S^1$. The standard path-loop spectral-sequence calculation supplies the induction: in

$$
K(\mathbb Z,n-1)\longrightarrow PK(\mathbb Z,n)
\longrightarrow K(\mathbb Z,n),
$$

the total space is contractible and the fundamental fiber class transgresses to $u_n$. An odd exterior fiber generator gives an even polynomial base generator. An even polynomial fiber generator gives an odd exterior base generator; the differential on its $k$th power has coefficient $k$, which is invertible over $\mathbb Q$. The multiplicative spectral sequence then has no remaining positive-degree classes in the total space. This is the rational transgression calculation for [Eilenberg–MacLane spaces](../../../../../eilenberg-maclane-space.md); it includes the absence of additional base generators.

For $m=2n+1\geq3$, choose $S^m\to K(\mathbb Z,m)$ representing the integral fundamental class. The ring calculation shows that this map is a rational [homology](../../../../../homology-split.md) equivalence: both spaces have rational [cohomology](../../../../../cohomology-split.md) only in degrees zero and $m$. The [rational Whitehead theorem](../../../../../rational-whitehead-theorem.md) for [simply connected](../../../../../simply-connected-space.md) spaces identifies their rational [homotopy groups](../../../../../homotopy-group.md). Since the target has only $\pi_m=\mathbb Z$, **the [rational homotopy groups of a sphere](../../../../../rational-homotopy-groups-of-a-sphere.md) in odd dimension are**

$$
\boxed{\pi_i(S^{2n+1})\otimes\mathbb Q=
\begin{cases}
\mathbb Q,&i=2n+1,\\
0,&i\ne2n+1.
\end{cases}}
$$

For $n=0$, this follows directly from $\pi_1(S^1)=\mathbb Z$ and the contractible [universal cover](../../../../../universal-cover.md) of the circle, which makes every higher [homotopy group](../../../../../homotopy-group.md) zero.

Let $M=\mathbb{CP}^2\#\mathbb{CP}^2$, with the standard complex orientations. It is [simply connected](../../../../../simply-connected-space.md) by the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) applied to the punctured summands. Classes $a,b\in H^2(M;\mathbb Q)$ can be chosen from the two summands. Their cross product vanishes, while their squares equal the oriented top class:

$$
ab=0,\qquad a^2=b^2=\omega.
$$

Thus the [cohomology ring of the connected sum of two complex projective planes](../../../../../cohomology-ring-of-the-connected-sum-of-two-complex-projective-planes.md) is

$$
H^*(M;\mathbb Q)=\mathbb Q[a,b]/(ab,a^2-b^2),
\qquad |a|=|b|=2.
$$

The two relations also kill all cubic monomials, so its dimensions are $1,2,1$ in degrees $0,2,4$ and zero otherwise.

We use the [Sullivan minimal model](../../../../../sullivan-minimal-model.md) dictionary: for a [simply connected](../../../../../simply-connected-space.md) finite-type space, the dual of its degree-$i$ generator space is $\pi_i(M)\otimes\mathbb Q$. The following free graded-commutative differential algebra is the [Sullivan model of the connected sum of two complex projective planes](../../../../../sullivan-model-of-the-connected-sum-of-two-complex-projective-planes.md):

$$
\boxed{\mathcal M=(\Lambda(a_2,b_2,r_3,s_3),d),
\quad da=db=0,\quad dr=ab,\quad ds=a^2-b^2.}
$$

It is minimal because all differentials of generators are decomposable.

To verify that no further generators are required, observe that $ab,a^2-b^2$ is a [regular sequence](../../../../../regular-sequence.md) in $\mathbb Q[a,b]$. The first polynomial is a nonzerodivisor. If $(a^2-b^2)h$ is divisible by $ab$, restricting to each coordinate axis forces $h$ to vanish on both axes, hence to be divisible by $ab$. The second polynomial is therefore a nonzerodivisor modulo the first. The [Koszul complex](../../../../../koszul-complex.md) of this [regular sequence](../../../../../regular-sequence.md) is exactly $\mathcal M$, so its [cohomology](../../../../../cohomology-split.md) is the quotient ring above, with no additional odd [cohomology](../../../../../cohomology-split.md).

For completeness, choose rational polynomial forms representing $a,b$ on $M$. Their product and the difference of their squares are exact; choose degree-three primitives for them. Sending $r,s$ to those primitives defines a differential-algebra map from $\mathcal M$ to the rational polynomial forms on $M$. It induces the specified cohomology-ring isomorphism and hence is a [quasi-isomorphism](../../../../../quasi-isomorphism.md). This verifies the model directly, rather than assuming that a [cohomology](../../../../../cohomology-split.md) presentation alone automatically determines all rational [homotopy](../../../../../homotopy.md).

The model has exactly two degree-two and two degree-three generators. Consequently **the [rational homotopy groups of the connected sum of two complex projective planes](../../../../../rational-homotopy-groups-of-the-connected-sum-of-two-complex-projective-planes.md) are**

$$
\boxed{\pi_i(\mathbb{CP}^2\#\mathbb{CP}^2)\otimes\mathbb Q=
\begin{cases}
\mathbb Q^2,&i=2,3,\\
0,&i=1\text{ or }i\geq4.
\end{cases}}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
