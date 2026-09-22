<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An $R$-point means a unital [algebra homomorphism over a field](../../../../../../algebra-homomorphism-over-a-field.md) $\alpha:k_q[x,y]\to R$, as in [points of a noncommutative algebra](../../../../../../points-of-a-noncommutative-algebra.md). It is specified by $X=\alpha(x)$ and $Y=\alpha(y)$ satisfying $YX=qXY$. For $R=\mathbb C$ and $q$ not a [root of unity](../../../../../../root-of-unity.md), $q\ne1$, so scalar commutativity gives $(1-q)XY=0$. Hence the **scalar points are the union of the two coordinate axes**:

$$
\boxed{\{(z,0):z\in\mathbb C\}\cup\{(0,w):w\in\mathbb C\}.}
$$

For matrix-valued [points of a noncommutative algebra](../../../../../../points-of-a-noncommutative-algebra.md), put $H=\mathbb C^n$ and let $H_\lambda(X)=\ker(X-\lambda I)^n$ be a [generalized eigenspace](../../../../../../generalized-eigenspace.md). From $XY=q^{-1}YX$,

$$
(X-q^{-1}\lambda I)^nY=q^{-n}Y(X-\lambda I)^n.
$$

Therefore $YH_\lambda(X)\subseteq H_{q^{-1}\lambda}(X)$, interpreting a missing [eigenvalue](../../../../../../eigenvalue.md) as the zero space. In particular the [linear subspaces](../../../../../../vector-subspace.md) $V_X=\bigoplus_{\lambda\ne0}H_\lambda(X)$ and $H_0(X)$ are invariant under both matrices. If $\lambda\ne0$, the numbers $\lambda,q^{-1}\lambda,\ldots,q^{-n}\lambda$ are distinct. A nonzero vector $Y^nv$ with $v\in H_\lambda(X)$ would force all $n+1$ intervening [generalized eigenspaces](../../../../../../generalized-eigenspace.md) to be nonzero, impossible in dimension $n$. Thus $Y^nV_X=0$: **$Y$ is nilpotent on $V_X$**, although $X$ is invertible there.

Apply the same argument with $X,Y$ exchanged, using $XY=q^{-1}YX$. The sum $V_Y$ of the nonzero $Y$ [generalized eigenspaces](../../../../../../generalized-eigenspace.md) is invariant under both matrices, and $X$ is nilpotent on it. Consequently $V_Y\subseteq H_0(X)$. Conversely, since $Y$ is nilpotent on $V_X$, its nonzero [generalized eigenspaces](../../../../../../generalized-eigenspace.md) all lie in $H_0(X)$. Decompose the restriction of $Y$ to that invariant space into its nonzero and zero [generalized eigenspaces](../../../../../../generalized-eigenspace.md):

$$
H_0(X)=V_Y\oplus U,\qquad U=H_0(X)\cap H_0(Y).
$$

The zero [generalized eigenspace](../../../../../../generalized-eigenspace.md) of $Y$ is $X$-invariant by the scaling identity, so $U$ is invariant under both matrices. On $U$, both matrices have only zero [eigenvalues](../../../../../../eigenvalue.md), hence are [nilpotent matrices](../../../../../../nilpotent-matrix.md). This proves the [spectral decomposition of a quantum-plane point](../../../../../../spectral-decomposition-of-a-quantum-plane-point.md):

$$
\boxed{\mathbb C^n=V_X\oplus V_Y\oplus U.}
$$

Here $V_X,V_Y$ mean sums of [generalized eigenspaces](../../../../../../generalized-eigenspace.md), not merely ordinary [eigenspaces](../../../../../../eigenspace.md); that distinction is necessary for non-diagonalizable points.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
