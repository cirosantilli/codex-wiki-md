<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A finite-dimensional [Lie algebra](../../../../../lie-algebra-split.md) over the [complex numbers](../../../../../complex-number.md) $L$ is a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) when its [solvable radical](../../../../../radical-of-a-lie-algebra.md) is zero, equivalently when it has no nonzero solvable ideals. Its [Killing form](../../../../../killing-form.md) is

$$
B_L(x,y)=\operatorname{tr}_L(\operatorname{ad}x\operatorname{ad}y).
$$

The [cyclic property of the trace](../../../../../cyclic-property-of-the-trace.md) makes this [bilinear form](../../../../../bilinear-form.md) symmetric and gives its [invariance of a bilinear form on a Lie algebra](../../../../../invariance-of-a-bilinear-form-on-a-lie-algebra.md):

$$
B_L([x,y],z)=B_L(x,[y,z]).
$$

It follows that $R=\{x:B_L(x,L)=0\}$ is an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md). For $x\in R$, $\operatorname{ad}x$ induces the zero map on $L/R$. Therefore, for $x,y\in R$, the [matrix trace](../../../../../matrix-trace.md) splits over the invariant subspace $R$ and the quotient to give $B_R(x,y)=B_L(x,y)=0$. In particular $B_R([R,R],R)=0$. The [Cartan solvability criterion](../../../../../cartan-solvability-criterion.md) implies that $R$ is solvable. Since $L$ is semisimple, $R=0$: **the Killing form is nondegenerate**.

For completeness, the trace step in the [Cartan solvability criterion](../../../../../cartan-solvability-criterion.md) is precisely the mechanism of the previous solution. For a complex matrix [Lie algebra](../../../../../lie-algebra-split.md) $\mathfrak a$ with $\operatorname{tr}(xy)=0$ for $x\in[\mathfrak a,\mathfrak a]$, $y\in\mathfrak a$, set $U=[\mathfrak a,\mathfrak a]$ and $W=\mathfrak a$. If $\beta\in M$ and $x=[a,b]$, then $\operatorname{tr}(x\beta)=\operatorname{tr}(a[b,\beta])=0$, since $[b,\beta]\in U$. Linearity and the [trace orthogonality nilpotence lemma](../../../../../trace-orthogonality-nilpotence-lemma.md) show that every member of $U$ is nilpotent. The [Engel theorem](../../../../../engel-s-theorem.md) makes $U$ nilpotent and hence $\mathfrak a$ solvable. Apply this to $\mathfrak a=\operatorname{ad}R$; the kernel of this [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md) is the abelian center of $R$, so $R$ is solvable as claimed.

For an arbitrary complex [Lie algebra](../../../../../lie-algebra-split.md), a [Cartan subalgebra](../../../../../cartan-subalgebra.md) $H$ means a [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md) that is self-normalizing: $N_L(H)=\{x:[x,H]\subseteq H\}=H$. This definition does not assume that $H$ is abelian. We prove that it is abelian when $L$ is semisimple.

Use the [generalized-weight decomposition for a nilpotent Lie algebra](../../../../../generalized-weight-decomposition-for-a-nilpotent-lie-algebra.md) for the action of $H$ on $L$. Its zero generalized [weight space](../../../../../weight-space.md) is

$$
L^0=\{x:(\operatorname{ad}h)^{\dim L}x=0\text{ for every }h\in H\}.
$$

We have $H\subseteq L^0$, since $H$ is nilpotent. If $L^0/H\ne0$, the [Engel theorem](../../../../../engel-s-theorem.md) gives a nonzero coset annihilated by every $h\in H$. Its representative $x$ satisfies $[H,x]\subseteq H$, contradicting $N_L(H)=H$. Thus $L^0=H$.

For a nonzero generalized [weight](../../../../../weight-representation-theory.md) $\lambda$, choose $h_0\in H$ with $\lambda(h_0)\ne0$. The operator $\operatorname{ad}h_0$ is invertible on $L^\lambda$ and nilpotent on $H$. For $h\in H$, $z\in L^\lambda$, write $z=(\operatorname{ad}h_0)^m w$ with $m$ large enough that $(\operatorname{ad}h_0)^m h=0$. Invariance of the [Killing form](../../../../../killing-form.md) gives

$$
B_L(h,z)=(-1)^mB_L((\operatorname{ad}h_0)^m h,w)=0.
$$

On the other hand, $H$ is solvable, so the [Lie theorem](../../../../../lie-s-theorem.md) triangularizes its action on $L$. For $a,b,h\in H$, the matrix $\operatorname{ad}[a,b]$ is strictly upper triangular, while $\operatorname{ad}h$ is upper triangular. Thus $B_L([H,H],H)=0$. Together with $L=H\oplus\bigoplus_{\lambda\ne0}L^\lambda$, this yields $B_L([H,H],L)=0$. Nondegeneracy gives $[H,H]=0$.

Finally, if $x$ commutes with $H$, it normalizes $H$, hence lies in $H$. Any abelian subalgebra containing $H$ consists of such elements. Thus **$H$ is a maximal abelian subalgebra**, indeed $C_L(H)=H$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
