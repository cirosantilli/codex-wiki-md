<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work over $\mathbb C$ with finite-dimensional [Lie algebras](../../../../../lie-algebra-split.md) and [Lie algebra representation](../../../../../lie-algebra-representation.md) spaces. The adjoint form of [Engel theorem](../../../../../engel-s-theorem.md) is

$$
\boxed{\mathfrak g\text{ is nilpotent }\Longleftrightarrow
\operatorname{ad}x\text{ is nilpotent for every }x\in\mathfrak g.}
$$

Here a [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md) has terminating [lower central series](../../../../../lower-central-series.md), $\gamma_1\mathfrak g=\mathfrak g$, $\gamma_{j+1}\mathfrak g=[\mathfrak g,\gamma_j\mathfrak g]$. We prove the stronger linear statement: if $V\ne0$, $L\subseteq\mathfrak{gl}(V)$ and every member of $L$ is a [nilpotent endomorphism](../../../../../nilpotent-linear-map.md), then there is a nonzero $v\in V$ killed by all of $L$, and $L$ can be simultaneously represented by [strictly upper triangular matrices](../../../../../strictly-upper-triangular-matrix.md).

For the [proof of Engel theorem by induction and normalizers](../../../../../proof-of-engel-theorem-by-induction-and-normalizers.md), first establish a useful nilpotence fact. If $x^m=0$, left and right multiplication by $x$ on $\operatorname{End}(V)$ commute. Expanding their difference gives

$$
(\operatorname{ad}x)^N(T)=\sum_{j=0}^N(-1)^j\binom Njx^{N-j}Tx^j.
$$

For $N=2m-1$, every summand contains a power of $x$ at least $m$, so $(\operatorname{ad}x)^{2m-1}=0$. Restrictions and induced quotient maps remain nilpotent.

Now prove the common-kernel statement, the [Engel lemma](../../../../../engel-lemma.md), by induction on $\dim L$. The zero algebra is immediate. Choose a maximal proper [Lie subalgebra](../../../../../lie-subalgebra.md) $M$. Its action on $L/M$ by commutators consists of nilpotent maps by the preceding fact. Applying the lower-dimensional induction hypothesis to its image gives a nonzero coset $y+M$ with $[M,y]\subseteq M$. Hence

$$
M\subsetneq N_L(M),\qquad
N_L(M)=\{z\in L:[z,M]\subseteq M\}.
$$

The [normalizer of a Lie subalgebra](../../../../../normalizer-of-a-lie-subalgebra.md) is a [Lie subalgebra](../../../../../lie-subalgebra.md) by the [Jacobi identity](../../../../../jacobi-identity.md). Maximality implies $N_L(M)=L$, so $M$ is an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md). Moreover $L/M$ has no proper nonzero [Lie subalgebra](../../../../../lie-subalgebra.md), and every one-dimensional subspace is a [Lie subalgebra](../../../../../lie-subalgebra.md). Thus $\dim L/M=1$.

Induction also provides a nonzero common annihilator

$$
W=\{v\in V:mv=0\text{ for all }m\in M\}.
$$

It is stable under $L$: for $m\in M$, $x\in L$, $v\in W$,

$$
m(xv)=x(mv)+[m,x]v=0,
$$

because $[m,x]\in M$. Choose $x$ representing a [basis](../../../../../basis.md) of $L/M$. The restriction of the [nilpotent endomorphism](../../../../../nilpotent-linear-map.md) $x$ to the nonzero space $W$ has nonzero [kernel](../../../../../kernel-of-a-linear-map.md). A vector in this [kernel](../../../../../kernel-of-a-linear-map.md) is killed by both $M$ and $x$, hence by all of $L$. This finishes the induction. When an action is not faithful, induction is applied to its image, whose [dimension](../../../../../dimension-vector-space.md) is no larger than $\dim M$; no faithfulness assumption is hidden.

Starting with the common-kernel line, apply the same statement to each successive quotient [Lie algebra representation](../../../../../lie-algebra-representation.md) space. It constructs a [complete flag](../../../../../complete-flag.md) of [invariant subspaces](../../../../../invariant-subspace.md)

$$
0=V_0\subset V_1\subset\cdots\subset V_d=V,\qquad
\dim V_j=j,\qquad LV_j\subseteq V_{j-1}.
$$

An adapted [basis](../../../../../basis.md) represents every member of $L$ by a [strictly upper triangular matrix](../../../../../strictly-upper-triangular-matrix.md). Every product of $d$ such matrices is zero, so every iterated commutator with $d$ entries is zero as well.

Finally, if every $\operatorname{ad}x$ on $\mathfrak g$ is nilpotent, apply the linear statement to the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md). With $d=\dim\mathfrak g$, every product of $d$ adjoint operators vanishes, so $\gamma_{d+1}\mathfrak g=0$. Conversely, if $\gamma_{c+1}\mathfrak g=0$, then $(\operatorname{ad}x)^cy=0$ for all $x,y$, proving the other implication. **This proves Engel's theorem and its simultaneous-triangularization form.** The hypothesis concerns every element of the algebra, not merely a chosen set of generators.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
