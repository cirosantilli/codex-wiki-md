<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [linear map](../../../../../linear-map.md) $\alpha$ is a [nilpotent endomorphism](../../../../../nilpotent-linear-map.md) if $\alpha^q=0$ for some positive integer $q$, and a [semisimple endomorphism](../../../../../diagonalizable-matrix.md) if it is [diagonalizable](../../../../../diagonalizable-matrix.md) over $\mathbb C$. Decompose $V$ into its [generalized eigenspaces](../../../../../generalized-eigenspace.md) $V_\lambda=\ker(\alpha-\lambda I)^d$, where $d=\dim V$. Define $\alpha_s$ on $V_\lambda$ to be $\lambda I$, and set $\alpha_n=\alpha-\alpha_s$. Then $\alpha_s$ is diagonalizable, $\alpha_n$ is nilpotent, and both preserve these [vector subspaces](../../../../../vector-subspace.md) and commute. Thus

$$
\boxed{\alpha=\alpha_s+\alpha_n,\qquad[\alpha_s,\alpha_n]=0.}
$$

For uniqueness, suppose $\alpha=S+N$ with $S$ semisimple, $N$ nilpotent and $SN=NS$. Both commute with $\alpha$, so preserve each $V_\lambda$. On an [eigenspace](../../../../../eigenspace.md) of $S$ of [eigenvalue](../../../../../eigenvalue.md) $\mu$ inside $V_\lambda$, the map $\alpha$ is $\mu I+N$ and has only the [eigenvalue](../../../../../eigenvalue.md) $\mu$. Since the same subspace lies in $V_\lambda$, $\mu=\lambda$. Hence $S=\lambda I$ on $V_\lambda$, proving $S=\alpha_s$ and $N=\alpha_n$. This is the additive [Jordan–Chevalley decomposition](../../../../../jordan-chevalley-decomposition.md).

We need a polynomial consequence of this decomposition. [Hermite interpolation](../../../../../hermite-interpolation.md) supplies a [polynomial](../../../../../polynomial-split.md) $p$ with $p(\alpha)=\alpha_s$, by prescribing $p(t)\equiv\lambda\pmod{(t-\lambda)^d}$ for each [eigenvalue](../../../../../eigenvalue.md). For any endomorphism $T$, its semisimple part can likewise be expressed as a [polynomial](../../../../../polynomial-split.md) in $T$ with zero constant term: if zero is an [eigenvalue](../../../../../eigenvalue.md), its interpolation condition already forces this; if not, add the independent condition $p(0)=0$.

On $\operatorname{End}(V)$, the maps $\operatorname{ad}\alpha_s$ and $\operatorname{ad}\alpha_n$ commute. The first is diagonalizable, with [eigenvalues](../../../../../eigenvalue.md) $\lambda-\mu$ on $\operatorname{Hom}(V_\mu,V_\lambda)$. The second is nilpotent, since

$$
(\operatorname{ad}N)^k(T)=\sum_{j=0}^k(-1)^j\binom kj N^{k-j}TN^j,
$$

which vanishes for $k\ge2q-1$ when $N^q=0$. Uniqueness therefore proves [adjoint compatibility of additive Jordan decomposition](../../../../../adjoint-compatibility-of-additive-jordan-decomposition.md): $\operatorname{ad}\alpha_s=(\operatorname{ad}\alpha)_s$.

Now assume $\alpha\in M$. The condition $[\alpha,W]\subseteq U\subseteq W$ implies that both $W$ and $U$ are invariant under $\operatorname{ad}\alpha$, and every [polynomial](../../../../../polynomial-split.md) in $\operatorname{ad}\alpha$ with zero constant term maps $W$ into $U$. Define $\beta$ to be multiplication by $\overline\lambda$ on $V_\lambda$. It commutes with $\alpha$. On $\operatorname{Hom}(V_\mu,V_\lambda)$, $\operatorname{ad}\beta$ acts by $\overline{\lambda-\mu}$. [Polynomial interpolation](../../../../../polynomial-interpolation.md) on the finite set of differences gives $\operatorname{ad}\beta=q(\operatorname{ad}\alpha_s)$ with $q(0)=0$. The preceding paragraph then expresses $\operatorname{ad}\beta$ as a [polynomial](../../../../../polynomial-split.md) in $\operatorname{ad}\alpha$ with zero constant term. Consequently $[\beta,W]\subseteq U$, so $\beta\in M$.

The assumed [trace orthogonality nilpotence lemma](../../../../../trace-orthogonality-nilpotence-lemma.md) now follows directly. On $V_\lambda$, $\alpha=\lambda I+\alpha_n$ and $\beta=\overline\lambda I$, while the [matrix trace](../../../../../matrix-trace.md) of the nilpotent restriction of $\alpha_n$ is zero. Hence

$$
0=\operatorname{tr}(\alpha\beta)=\sum_\lambda\dim(V_\lambda)|\lambda|^2.
$$

Every summand is nonnegative, so every [eigenvalue](../../../../../eigenvalue.md) of $\alpha$ is zero. Its [Jordan–Chevalley decomposition](../../../../../jordan-chevalley-decomposition.md) therefore has $\alpha_s=0$, and **$\alpha$ is nilpotent**. Notice that neither $U$ nor $W$ was required to be a Lie subalgebra.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
