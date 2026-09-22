<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $\rho:\mathfrak g\to\mathfrak{gl}(V)$ be a finite-dimensional [Lie algebra representation](../../../../../lie-algebra-representation.md). The form denoted $B_V$ is

$$
\boxed{B_V(X,Y)=\operatorname{tr}_V\bigl(\rho(X)\rho(Y)\bigr).}
$$

It is the [Trace form of a Lie algebra representation](../../../../../trace-form-of-a-lie-algebra-representation.md); the [Killing form](../../../../../killing-form.md) $B$ without a subscript is specifically the case $V=\mathfrak g$, $\rho=\operatorname{ad}$. The distinction matters: the form of the trivial representation cannot detect whether the algebra is semisimple.

Linearity of $\rho$ and [trace](../../../../../matrix-trace.md) proves bilinearity, and cyclicity of the [trace](../../../../../matrix-trace.md) gives symmetry. With $A=\rho(X)$, $D=\rho(Y)$ and $C=\rho(Z)$, the representation identity gives

$$
\begin{aligned}
B_V([X,Y],Z)&=\operatorname{tr}((AD-DA)C)\\
&=\operatorname{tr}(ADC-ACD)=\operatorname{tr}(A(DC-CD))\\
&=B_V(X,[Y,Z]).
\end{aligned}
$$

Thus it is an [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md), and in particular the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) preserves the [Killing form](../../../../../killing-form.md).

The [Cartan solvability criterion](../../../../../cartan-solvability-criterion.md) has two useful formulations. For a finite-dimensional complex [Lie algebra](../../../../../lie-algebra-split.md) $\mathfrak g$,

$$
\boxed{\mathfrak g\text{ is solvable}\quad\Longleftrightarrow\quad B(\mathfrak g,[\mathfrak g,\mathfrak g])=0.}
$$

Its matrix version says that a [Lie subalgebra](../../../../../lie-subalgebra.md) $L\subseteq\mathfrak{gl}(V)$ is solvable precisely when $\operatorname{tr}(xy)=0$ for all $x\in[L,L]$ and $y\in L$. We prove the matrix version first, with ordinary [trace](../../../../../matrix-trace.md) in $V$.

If $L$ is solvable, the [Lie theorem](../../../../../lie-s-theorem.md) makes all its matrices upper triangular. Their [commutators](../../../../../commutator.md) are strictly upper triangular, so multiplying such a matrix by an upper triangular one still has zero diagonal and hence zero [trace](../../../../../matrix-trace.md). This proves the easy direction.

Conversely assume the trace-orthogonality condition and fix $x\in[L,L]$. We show that all [eigenvalues](../../../../../eigenvalue.md) of $x$ vanish. Use its [Additive Jordan decomposition](../../../../../jordan-chevalley-decomposition.md) $x=x_s+x_n$ with $[x_s,x_n]=0$. On the [generalized eigenspace](../../../../../generalized-eigenspace.md) $V_\lambda$ of $x$, define an auxiliary endomorphism $y$ to be $\overline\lambda I$. This $y$ need not be in $L$; we only need control of its [commutator](../../../../../commutator.md) with $L$.

On $\operatorname{Hom}(V_\mu,V_\lambda)$, $\operatorname{ad}x_s$ acts by $\lambda-\mu$ and $\operatorname{ad}y$ by $\overline\lambda-\overline\mu$. Choose a [polynomial](../../../../../polynomial-split.md) $q$ with $q(0)=0$ and $q(\lambda-\mu)=\overline{\lambda-\mu}$ at the finitely many distinct differences. [Polynomial interpolation](../../../../../polynomial-interpolation.md) supplies it because equal differences have equal conjugates. Therefore $\operatorname{ad}y=q(\operatorname{ad}x_s)$.

The [adjoint compatibility of additive Jordan decomposition](../../../../../adjoint-compatibility-of-additive-jordan-decomposition.md) identifies $\operatorname{ad}x_s$ as the semisimple part of $\operatorname{ad}x$. Elementary [Jordan–Chevalley decomposition](../../../../../jordan-chevalley-decomposition.md) gives $\operatorname{ad}x_s=p(\operatorname{ad}x)$ for a [polynomial](../../../../../polynomial-split.md) $p$ with $p(0)=0$. Hence $\operatorname{ad}y$ is a [polynomial](../../../../../polynomial-split.md) in $\operatorname{ad}x$ with zero constant term. Since $\operatorname{ad}x$ maps $L$ into $[L,L]$ and preserves that [Lie algebra ideal](../../../../../ideal-of-a-lie-algebra.md), we obtain

$$
[y,L]\subseteq[L,L].
$$

No assumption that $x_s$, $x_n$ or $y$ belongs to $L$ was made.

Write $x=\sum_i[a_i,b_i]$ with $a_i,b_i\in L$. Cyclicity and the assumed orthogonality now give

$$
\operatorname{tr}(xy)=\sum_i\operatorname{tr}([a_i,b_i]y)=\sum_i\operatorname{tr}(a_i[b_i,y])=0.
$$

On the other hand the nilpotent parts have zero [trace](../../../../../matrix-trace.md) on each [generalized eigenspace](../../../../../generalized-eigenspace.md), so

$$
\operatorname{tr}(xy)=\sum_\lambda (\dim V_\lambda)\lambda\overline\lambda=\sum_\lambda (\dim V_\lambda)|\lambda|^2.
$$

Thus all $\lambda$ are zero and $x$ is a [nilpotent endomorphism](../../../../../nilpotent-linear-map.md). This is the [Conjugate-spectrum proof of Cartan solvability](../../../../../conjugate-spectrum-proof-of-cartan-solvability.md).

The permitted [Engel theorem](../../../../../engel-s-theorem.md), in the form needed here, states: a finite-dimensional [Lie subalgebra](../../../../../lie-subalgebra.md) of [endomorphisms](../../../../../endomorphism.md) in which every element is nilpotent has a nonzero vector annihilated by all its elements, and iteration on quotients makes every element simultaneously strictly upper triangular. Apply it to $[L,L]$. The strictly upper triangular algebra is nilpotent, so $[L,L]$ is a [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md) and therefore solvable. Since $L/[L,L]$ is abelian, the [derived series of a Lie algebra](../../../../../derived-series-of-a-lie-algebra.md) of $L$ terminates too. This proves the matrix criterion.

Apply it to $L=\operatorname{ad}\mathfrak g$. The condition on $B$ is exactly the matrix condition on $L$. Thus $\operatorname{ad}\mathfrak g$ is solvable. The [kernel](../../../../../kernel-of-a-linear-map.md) of $\operatorname{ad}$ is the [center of a Lie algebra](../../../../../center-of-a-lie-algebra.md), which is abelian, so $\mathfrak g$ is solvable as well: once the derived series maps to zero it is central, and its next term vanishes. Conversely a solvable $\mathfrak g$ has solvable adjoint image, proving the abstract [Cartan solvability criterion](../../../../../cartan-solvability-criterion.md) in both directions.

A finite-dimensional [Lie algebra](../../../../../lie-algebra-split.md) is a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) when it has no nonzero solvable [Lie algebra ideal](../../../../../ideal-of-a-lie-algebra.md), equivalently its [solvable radical](../../../../../radical-of-a-lie-algebra.md) is zero. Let $R=\operatorname{rad}B=\{x:B(x,\mathfrak g)=0\}$. Invariance makes $R$ an ideal. For $x,y\in R$, $\operatorname{ad}x$ induces zero on $\mathfrak g/R$, and the block [trace](../../../../../matrix-trace.md) gives $B_R(x,y)=B_{\mathfrak g}(x,y)=0$, where $B_R$ is the adjoint [Killing form](../../../../../killing-form.md) of $R$ itself. The [Cartan solvability criterion](../../../../../cartan-solvability-criterion.md) therefore makes $R$ solvable. If $\mathfrak g$ is semisimple, $R=0$.

Conversely suppose $B$ is a [nondegenerate bilinear form](../../../../../nondegenerate-bilinear-form.md). If a nonzero solvable ideal existed, its last nonzero derived term $A$ would be an abelian ideal of $\mathfrak g$. For $a\in A$ and $x\in\mathfrak g$, the operator $\operatorname{ad}a\,\operatorname{ad}x$ has image in $A$ and is zero on $A$, so its square and its [trace](../../../../../matrix-trace.md) are zero. Thus $B(A,\mathfrak g)=0$, contradicting nondegeneracy. This is [Abelian ideals lie in the radical of the Killing form](../../../../../abelian-ideals-lie-in-the-radical-of-the-killing-form.md). We conclude the [Cartan criterion for semisimplicity](../../../../../cartan-criterion-for-semisimplicity.md):

$$
\boxed{\mathfrak g\text{ is semisimple}\quad\Longleftrightarrow\quad B\text{ is nondegenerate}.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
