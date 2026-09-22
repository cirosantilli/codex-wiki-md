<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $p:\mathbb P(E)\to X$ be the [projectivization of a real vector bundle](../../../../../projectivization-of-a-real-vector-bundle.md), let $L_E$ be its [tautological bundle](../../../../../tautological-bundle.md), and put

$$
u=w_1(L_E)\in H^1(\mathbb P(E);\mathbb F_2).
$$

The mod-two projective bundle formula says that $H^*(\mathbb P(E);\mathbb F_2)$ is a free $H^*(X;\mathbb F_2)$-module on $1,u,\ldots,u^{d-1}$. The [Projective bundle definition of Stiefel–Whitney classes](../../../../../projective-bundle-definition-of-stiefel-whitney-classes.md) is the unique relation

$$
u^d+p^*w_1(E)u^{d-1}+\cdots+p^*w_d(E)=0.
$$

Apply the [splitting principle for real vector bundles](../../../../../splitting-principle-for-real-vector-bundles.md). After an injective pullback, write

$$
E=L_1\oplus\cdots\oplus L_d,
\qquad
E'=L'_1\oplus\cdots\oplus L'_{d'}.
$$

If $x_i=w_1(L_i)$, the projective-bundle relation factors as

$$
\prod_{i=1}^d(u+x_i)=0,
$$

so

$$
w(E)=\prod_{i=1}^d(1+x_i).
$$

The line summands of $E\oplus E'$ are the union of the two lists, hence

$$
w(E\oplus E')=w(E)w(E').
$$

Comparing the degree-$k$ components proves the [Whitney product formula for Stiefel–Whitney classes](../../../../../whitney-product-formula-for-stiefel-whitney-classes.md)

$$
w_k(E\oplus E')=\sum_{i+j=k}w_i(E)w_j(E').
$$

Injectivity of the splitting pullback returns the identity to $X$.

For real line bundles, the transition functions take values in $O(1)=\{\pm1\}$. Tensor product multiplies these signs, while the identification $\{\pm1\}\cong\mathbb Z/2$ turns multiplication into addition. The corresponding degree-one characteristic classes therefore satisfy the [First Stiefel–Whitney class of a tensor product of real line bundles](../../../../../first-stiefel-whitney-class-of-a-tensor-product-of-real-line-bundles.md) formula

$$
w_1(L\otimes L')=w_1(L)+w_1(L').
$$

Equivalently, this follows from the classification of real line bundles by $H^1(X;\mathbb F_2)$.

Now take $M=\mathbb{RP}^n$ and $E=k\gamma_{\mathbb R}^{1,n+1}$. Since

$$
E=\gamma_{\mathbb R}^{1,n+1}\otimes\mathbb R^k,
$$

a line in $E_x$ is the fixed line $\gamma_x$ tensored with a line in $\mathbb R^k$. Thus the [projectivization of copies of the real tautological line bundle](../../../../../projectivization-of-copies-of-the-real-tautological-line-bundle.md) is

$$
\mathbb P(E)\cong\mathbb{RP}^n\times\mathbb{RP}^{k-1}.
$$

Let $x$ and $v$ be the degree-one generators pulled back from the first and second factors. The [mod-two cohomology ring of real projective space](../../../../../mod-two-cohomology-ring-of-real-projective-space.md) and the [Künneth theorem](../../../../../kunneth-theorem.md) give

$$
H^*(\mathbb P(E);\mathbb F_2)
\cong
\mathbb F_2[x,v]/(x^{n+1},v^k).
$$

The tautological line $L_E$ is the tensor product of the two tautological lines, so $w_1(L_E)=x+v$. In the alternative generator $u=w_1(L_E)$, the same ring is

$$
\mathbb F_2[x,u]/(x^{n+1},(u+x)^k).
$$

The stable tangent-bundle identity

$$
T\mathbb{RP}^n\oplus\mathbf1\cong(n+1)\gamma_{\mathbb R}^{1,n+1}
$$

gives

$$
w(T\mathbb{RP}^n)=(1+x)^{n+1}.
$$

For the vertical part of the [tangent bundle of a projectivized real vector bundle](../../../../../tangent-bundle-of-a-projectivized-real-vector-bundle.md),

$$
\mathbf1\oplus\operatorname{Hom}(L_E,\omega_E)
\cong L_E^*\otimes p^*E.
$$

Each of the $k$ line summands on the right has first Stiefel–Whitney class

$$
w_1(L_E^*\otimes p^*\gamma)=w_1(L_E)+x=v.
$$

The [Whitney product formula for Stiefel–Whitney classes](../../../../../whitney-product-formula-for-stiefel-whitney-classes.md) therefore yields

$$
w(T\mathbb P(E))
=(1+x)^{n+1}(1+v)^k,
$$

the [Total Stiefel–Whitney class of the projectivization of copies of the tautological line](../../../../../total-stiefel-whitney-class-of-the-projectivization-of-copies-of-the-tautological-line.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 142](../../paper-142-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
