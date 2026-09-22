<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $D=\operatorname{ad}y$. The [generalized eigenspace](../../../../../generalized-eigenspace.md) decomposition of the [linear map](../../../../../linear-map.md) $D$ is

$$
L=\bigoplus_\lambda L_{\lambda,y},
\qquad
L_{\lambda,y}=\ker(D-\lambda I)^N
$$

for any sufficiently large $N$. Because $D$ is a [derivation](../../../../../derivation-of-a-lie-algebra.md), the [generalized-eigenspace bracket lemma](../../../../../generalized-eigenspace-bracket-lemma.md) gives

$$
[L_{\lambda,y},L_{\mu,y}]\subseteq L_{\lambda+\mu,y}.
$$

Consequently $L_{0,y}$ is a [Lie subalgebra](../../../../../lie-subalgebra.md).

The set $I(K)=\{x\in L:[x,K]\subseteq K\}$ is the [normalizer of a Lie subalgebra](../../../../../normalizer-of-a-lie-subalgebra.md) $K$. Certainly $L_{0,y}\subseteq I(L_{0,y})$. Conversely, if $x\in I(L_{0,y})$, then $y\in L_{0,y}$ gives

$$
Dx=[y,x]\in L_{0,y}.
$$

On the direct sum of the nonzero generalized eigenspaces, $D$ is [invertible](../../../../../invertible-linear-map.md). Hence the nonzero-eigenvalue component of $x$ vanishes, and

$$
\boxed{I(L_{0,y})=L_{0,y}.}
$$

Now let $K$ be a [Lie subalgebra](../../../../../lie-subalgebra.md) containing $L_{0,y}$. Since $y\in K$, the subspace $K$ is $D$-invariant. The generalized zero eigenspace of the induced map on $L/K$ is the image of $L_{0,y}$, hence is zero. If $x\in I(K)$, then $Dx=[y,x]\in K$, so $x+K$ lies in that zero eigenspace. Thus $x\in K$ and

$$
\boxed{I(K)=K.}
$$

A [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md) is one whose [lower central series](../../../../../lower-central-series-of-a-lie-algebra.md)

$$
\gamma_1(L)=L,
\qquad
\gamma_{r+1}(L)=[L,\gamma_r(L)]
$$

eventually reaches zero. Suppose $L$ is nilpotent and $K\subsetneq L$. Choose the least $r\geq2$ for which $\gamma_r(L)\subseteq K$. Then $\gamma_{r-1}(L)\nsubseteq K$, and any

$$
x\in\gamma_{r-1}(L)\setminus K
$$

satisfies $[x,K]\subseteq[L,\gamma_{r-1}(L)]=\gamma_r(L)\subseteq K$. Therefore $x\in I(K)\setminus K$, proving the [normalizer condition for a nilpotent Lie algebra](../../../../../normalizer-condition-for-a-nilpotent-lie-algebra.md)

$$
\boxed{K\subsetneq I(K).}
$$

It remains to prove the converse needed here. The [Engel lemma](../../../../../engel-lemma.md) states that if a finite-dimensional [Lie algebra of linear maps](../../../../../lie-algebra-representation.md) consists of [nilpotent maps](../../../../../nilpotent-linear-map.md), then the maps have a common nonzero vector in their kernels. To prove it, induct on the dimension of the algebra. For a maximal proper subalgebra $H$, induction applied to the action of $H$ on $L/H$ produces $x\notin H$ with $[H,x]\subseteq H$. Thus $H$ is an ideal of codimension one. Induction also gives a nonzero common kernel

$$
W=\{v:Hv=0\}.
$$

The ideal property makes $W$ invariant under $L$; a nilpotent representative of a basis of $L/H$ has a nonzero kernel on $W$, yielding a vector killed by all of $L$.

Apply the lemma to the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md). It produces a nonzero element of the [center of a Lie algebra](../../../../../center-of-a-lie-algebra.md). Induction on $\dim L$, followed by passage to the quotient by this center, proves [Engel theorem](../../../../../engel-s-theorem.md): if every $\operatorname{ad}y$ is nilpotent, then $L$ is nilpotent. The hypothesis $L_{0,y}=L$ says exactly that every $\operatorname{ad}y$ is nilpotent, so

$$
\boxed{L\text{ is nilpotent}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
