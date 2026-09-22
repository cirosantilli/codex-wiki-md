<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The space $\operatorname{End}(V)$ becomes a [Lie algebra](../../../../../lie-algebra-split.md) under the commutator

$$
[X,Y]=XY-YX.
$$

A Lie subalgebra $L$ is abelian when $[L,L]=0$; nilpotent when its [lower central series of a Lie algebra](../../../../../lower-central-series-of-a-lie-algebra.md) $\gamma_{r+1}=[L,\gamma_r]$ reaches zero; and soluble when its [derived series of a Lie algebra](../../../../../derived-series-of-a-lie-algebra.md) $L^{(r+1)}=[L^{(r)},L^{(r)}]$ reaches zero.

If $H\subsetneq L$ and $L$ is nilpotent, choose the least $r$ with $\gamma_r(L)\subseteq H$. Then $\gamma_{r-1}(L)\nsubseteq H$, while

$$
[\gamma_{r-1}(L),H]\subseteq\gamma_r(L)\subseteq H.
$$

Thus the [normalizer of a Lie subalgebra](../../../../../normalizer-of-a-lie-subalgebra.md) strictly contains $H$. If $H$ is maximal proper, its normalizer must be all of $L$, so $H$ is an ideal. Solubility is insufficient: in the two-dimensional affine Lie algebra $L=\langle x,y\rangle$ with $[x,y]=y$, the maximal subalgebra $\mathbb Cx$ is not an ideal.

A [derivation of a Lie algebra](../../../../../derivation-of-a-lie-algebra.md) is a linear map $D$ satisfying

$$
D[x,y]=[Dx,y]+[x,Dy].
$$

It is inner when $D=\operatorname{ad}z$ for some $z\in L$.

Every nonzero finite-dimensional nilpotent Lie algebra has an [outer derivation of a nilpotent Lie algebra](../../../../../outer-derivation-of-a-nilpotent-lie-algebra.md). Choose a codimension-one maximal subalgebra $K$; it is an ideal by the result above, and write $L=K\oplus\mathbb Cz$. The centralizer $C_L(K)$ is nonzero because it contains $Z(L)$. Let $n$ be largest such that

$$
C_L(K)\subseteq\gamma_n(L),
$$

and choose $z_0\in C_L(K)\setminus\gamma_{n+1}(L)$. Define

$$
D(K)=0,\qquad D(z)=z_0.
$$

Because $K$ is an ideal and $z_0$ centralizes $K$, the derivation identity holds on $K\times K$ and on $z\times K$, hence everywhere. If $D=\operatorname{ad}x$, then $D(K)=0$ would put $x$ in $C_L(K)\subseteq\gamma_n(L)$, so

$$
D(z)=[x,z]\in\gamma_{n+1}(L),
$$

contrary to the choice of $z_0$. Thus $D$ is outer.

The analogous assertion fails for soluble algebras. In the affine example, a derivation has

$$
D(x)=by,\qquad D(y)=dy,
$$

and equals $\operatorname{ad}(dx-by)$. Thus every derivation is inner although $L$ is nonzero and soluble.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
