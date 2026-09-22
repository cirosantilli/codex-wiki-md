<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A finite-dimensional complex [Lie algebra](../../../../../lie-algebra-split.md) is a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) when its [solvable radical](../../../../../radical-of-a-lie-algebra.md) is zero, equivalently when it has no nonzero solvable ideals. Its [Killing form](../../../../../killing-form.md) is the [symmetric bilinear form](../../../../../symmetric-bilinear-form.md)

$$
B_L(x,y)=\operatorname{tr}_L(\operatorname{ad}_x\operatorname{ad}_y).
$$

The cyclic [trace](../../../../../matrix-trace.md) identity and $\operatorname{ad}_{[z,x]}=[\operatorname{ad}_z,\operatorname{ad}_x]$ give

$$
B_L([z,x],y)+B_L(x,[z,y])=0.
$$

Thus the [Killing form](../../../../../killing-form.md) is an [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md). In particular its radical $R=\{x:B_L(x,L)=0\}$ is an ideal.

We supply the [trace](../../../../../matrix-trace.md) argument needed for nondegeneracy rather than assuming the [Cartan criterion for semisimplicity](../../../../../cartan-criterion-for-semisimplicity.md). The matrix form of the [Cartan solvability criterion](../../../../../cartan-solvability-criterion.md) says: if $A\subseteq\operatorname{End}_{\mathbb C}(V)$ and $\operatorname{tr}(uv)=0$ for every $u\in[A,A]$, $v\in A$, then $A$ is solvable. To prove this direction, fix $u\in[A,A]$. Let $V=\bigoplus_\lambda V_\lambda$ be its [generalized eigenspace](../../../../../generalized-eigenspace.md) decomposition, and define $s$ to act on $V_\lambda$ by the scalar $\overline\lambda$. On $\operatorname{Hom}(V_\mu,V_\lambda)$, the semisimple part of $\operatorname{ad}_u$ has [eigenvalue](../../../../../eigenvalue.md) $\lambda-\mu$, whereas $\operatorname{ad}_s$ acts by $\overline\lambda-\overline\mu=\overline{\lambda-\mu}$. [Polynomial interpolation](../../../../../polynomial-interpolation.md) on the finitely many [eigenvalues](../../../../../eigenvalue.md), with all derivatives through the sizes of the nilpotent blocks set to zero, therefore gives

$$
\operatorname{ad}_s=p(\operatorname{ad}_u),\qquad p(0)=0.
$$

Here the same difference always has the same conjugate, so the interpolation is consistent; the prescribed zero derivatives remove every nilpotent block. Since $\operatorname{ad}_u(A)\subseteq[A,A]$, it follows that $[s,A]\subseteq[A,A]$.

Write $u=\sum_j[a_j,b_j]$. By cyclicity and the [trace](../../../../../matrix-trace.md) hypothesis,

$$
\operatorname{tr}(us)=\sum_j\operatorname{tr}(a_j[b_j,s])=0.
$$

On the other hand, $\operatorname{tr}(us)=\sum_\lambda\dim(V_\lambda)|\lambda|^2$. Thus all [eigenvalues](../../../../../eigenvalue.md) of $u$ vanish, and every element of $[A,A]$ is nilpotent. The [Engel theorem](../../../../../engel-s-theorem.md) makes $[A,A]$ nilpotent as a [Lie algebra](../../../../../lie-algebra-split.md), hence solvable; $A/[A,A]$ is abelian, so $A$ is solvable. This is the [Conjugate-spectrum proof of Cartan solvability](../../../../../conjugate-spectrum-proof-of-cartan-solvability.md).

Apply this to the Killing radical $R$. For $x,y\in R$, the adjoint actions preserve $R$ and act as zero on $L/R$, because $R$ is an ideal. Computing traces in a basis adapted to $R$ gives

$$
B_R(x,y)=B_L(x,y)=0.
$$

The matrix [Lie algebra](../../../../../lie-algebra-split.md) $\operatorname{ad}_R(R)$ consequently satisfies the [trace](../../../../../matrix-trace.md) criterion and is solvable. Its kernel is $Z(R)$, an abelian ideal; a central extension of a solvable algebra is solvable. Thus $R$ is solvable. This proves the reusable assertion that the [Killing radical is a solvable ideal](../../../../../killing-radical-is-a-solvable-ideal.md). Semisimplicity forces $R=0$, and hence **$B_L$ is nondegenerate**.

A [Cartan subalgebra](../../../../../cartan-subalgebra.md) is a nilpotent subalgebra $H$ which is self-normalizing:

$$
N_L(H)=\{x\in L:[x,H]\subseteq H\}=H.
$$

For a complex semisimple algebra this is equivalently a maximal toral subalgebra. The nilpotent, self-normalizing definition permits a proof of the restricted nondegeneracy without first assuming the toral characterization.

Use the [generalized-weight decomposition for a nilpotent Lie algebra](../../../../../generalized-weight-decomposition-for-a-nilpotent-lie-algebra.md) for the adjoint action of $H$:

$$
L=\bigoplus_\lambda L^\lambda,\qquad
L^\lambda=\{v:(\operatorname{ad}_h-\lambda(h)I)^{\dim L}v=0\text{ for all }h\in H\}.
$$

For completeness, the stability underlying this decomposition follows directly from nilpotence of $H$. For fixed $h$, every $\operatorname{ad}_h$ on $H$ is nilpotent. If $T=\rho(h)$ and $S=\rho(y)$ in a finite-dimensional representation, then $(\operatorname{ad}_T)^rS=0$ for sufficiently large $r$. The identity

$$
(T-aI)^N S=\sum_{j=0}^N\binom Nj (\operatorname{ad}_T)^j(S)(T-aI)^{N-j}
$$

shows that $S$ preserves each [generalized eigenspace](../../../../../generalized-eigenspace.md) of $T$. Starting with a basis of $H$, refine these primary decompositions successively; all summands remain $H$-invariant. Each resulting summand has only one [eigenvalue](../../../../../eigenvalue.md) for each basis element. The [Lie theorem](../../../../../lie-s-theorem.md) triangularizes the action on that summand, so those [eigenvalues](../../../../../eigenvalue.md) extend to a single linear character $\lambda$ on all of $H$. This proves the displayed decomposition and nilpotence of all shifted operators there.

Since $H$ is nilpotent, $H\subseteq L^0$. The space $L^0$ is a subalgebra: repeated use of the derivation rule for $\operatorname{ad}_h$ shows that the bracket of two generalized zero-[eigenvectors](../../../../../eigenvector.md) is another such vector. If $L^0/H\ne0$, the adjoint action of $H$ on this quotient consists entirely of nilpotent maps. The [Engel theorem](../../../../../engel-s-theorem.md) supplies a nonzero coset $x+H$ with $[H,x]\subseteq H$, contradicting self-normalization. Therefore the [zero generalized weight space of a Cartan subalgebra](../../../../../zero-generalized-weight-space-of-a-cartan-subalgebra.md) is exactly $H$.

Finally, $B_L(H,L^\lambda)=0$ when $\lambda\ne0$. Choose $h\in H$ with $\lambda(h)\ne0$ and put $T=\operatorname{ad}_h$. On $H$, a power $T^m$ vanishes. On $L^\lambda$, $T$ is invertible. For $u\in H$ and $v\in L^\lambda$, write $v=T^m w$; invariance gives

$$
B_L(u,v)=B_L(u,T^m w)=(-1)^mB_L(T^m u,w)=0.
$$

If $u\in H$ is orthogonal to $H$, it is now orthogonal to every summand of $L$, so nondegeneracy of $B_L$ implies $u=0$. **The restriction $B_L|_{H\times H}$ is nondegenerate.** This establishes the [nondegeneracy of the Killing form on a Cartan subalgebra](../../../../../nondegeneracy-of-the-killing-form-on-a-cartan-subalgebra.md) for every [Cartan subalgebra](../../../../../cartan-subalgebra.md), without requiring a chosen root basis.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
