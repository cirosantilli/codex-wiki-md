<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [nilpotent endomorphism](../../../../../nilpotent-linear-map.md) $x$ satisfies $x^N=0$ for some [positive integer](../../../../../positive-integer.md) $N$. A [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md) $\mathfrak g$ has a terminating [lower central series of a Lie algebra](../../../../../lower-central-series-of-a-lie-algebra.md): with $\gamma_1=\mathfrak g$ and $\gamma_{r+1}=[\mathfrak g,\gamma_r]$, one has $\gamma_r=0$ for some $r$. These are different conditions: the first concerns a particular [linear map](../../../../../linear-map.md), whereas the second concerns repeated [Lie brackets](../../../../../lie-bracket.md).

The representation form of [Engel theorem](../../../../../engel-s-theorem.md) says that if a finite-dimensional [Lie subalgebra](../../../../../lie-subalgebra.md) $L\subseteq\operatorname{End}_k(V)$ consists entirely of [nilpotent endomorphisms](../../../../../nilpotent-linear-map.md), with $0<\dim V<\infty$, then $V$ contains a nonzero vector annihilated by every element of $L$. Consequently there is a [basis](../../../../../basis.md) in which every element of $L$ is strictly upper triangular. No assumption on the [characteristic of a field](../../../../../characteristic-of-a-field.md) or algebraic closure is required.

We prove the common-vector assertion by induction on $\dim L$, simultaneously for every nonzero finite-dimensional representation space. The zero algebra is immediate. First, [nilpotence of commutation by a nilpotent endomorphism](../../../../../nilpotence-of-commutation-by-a-nilpotent-endomorphism.md) follows from

$$
(\operatorname{ad}x)^r(T)=\sum_{j=0}^r(-1)^j\binom rj x^{r-j}Tx^j.
$$

If $x^N=0$, the right-hand side vanishes for $r\geq2N-1$, in every [characteristic of a field](../../../../../characteristic-of-a-field.md). For any proper [Lie subalgebra](../../../../../lie-subalgebra.md) $M\subsetneq L$, its [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) on $L/M$ therefore consists of [nilpotent endomorphisms](../../../../../nilpotent-linear-map.md). Its image has dimension at most $\dim M<\dim L$, so the inductive assertion gives a nonzero class $y+M$ annihilated by $M$. Equivalently $y\notin M$ and $[M,y]\subseteq M$. Thus the [Engel normalizer lemma](../../../../../engel-normalizer-lemma.md) gives $M\subsetneq N_L(M)$.

Choose a maximal proper [Lie subalgebra](../../../../../lie-subalgebra.md) $M$. Its [normalizer of a Lie subalgebra](../../../../../normalizer-of-a-lie-subalgebra.md) must be all of $L$, so $M$ is an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md). Moreover $L/M$ has dimension one: otherwise a one-dimensional [Lie subalgebra](../../../../../lie-subalgebra.md) of this quotient would have a proper inverse image strictly between $M$ and $L$. By induction the space $W=\{v\in V:Mv=0\}$ is nonzero. It is invariant under $L$, since $m(xw)=x(mw)+[m,x]w=0$. Write $L=M+kx$. The restriction of the [nilpotent endomorphism](../../../../../nilpotent-linear-map.md) $x$ to $W$ has a nonzero [kernel](../../../../../kernel-of-a-linear-map.md), and any vector in that kernel is annihilated by all of $L$. This completes the induction. Apply the assertion repeatedly to $V/kv$ to obtain a complete invariant flag $0=V_0\subset V_1\subset\cdots\subset V_d=V$ with $LV_j\subseteq V_{j-1}$. A [basis](../../../../../basis.md) adapted to that flag makes every matrix strictly upper triangular.

**A nilpotent abstract [Lie algebra](../../../../../lie-algebra-split.md) need not act by nilpotent matrices.** For $V\ne0$, the scalar algebra $kI\subseteq\mathfrak{gl}(V)$ is an [abelian Lie algebra](../../../../../abelian-lie-algebra.md), hence a [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md), but $I^N=I\ne0$. No change of [basis](../../../../../basis.md) makes $I$ strictly upper triangular. The failed implication is precisely the distinction described in [nilpotent Lie algebras need not act nilpotently](../../../../../nilpotent-lie-algebras-need-not-act-nilpotently.md).

If $\mathfrak g$ is a [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md), then $(\operatorname{ad}x)^r\mathfrak g\subseteq\gamma_{r+1}$, so every $\operatorname{ad}x$ is a [nilpotent endomorphism](../../../../../nilpotent-linear-map.md). Conversely, apply [Engel theorem](../../../../../engel-s-theorem.md) to $\operatorname{ad}\mathfrak g$ acting on $\mathfrak g$. Its invariant flag is lowered by every [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) matrix, so every product of $d=\dim\mathfrak g$ such matrices vanishes. Since $\gamma_{d+1}$ is spanned by expressions $\operatorname{ad}x_1\cdots\operatorname{ad}x_d(y)$, the [lower central series of a Lie algebra](../../../../../lower-central-series-of-a-lie-algebra.md) terminates. Therefore

$$
\boxed{\mathfrak g\text{ is nilpotent}\quad\Longleftrightarrow\quad\operatorname{ad}x\text{ is nilpotent for every }x\in\mathfrak g.}
$$

Finally suppose $k$ is an [algebraically closed field](../../../../../algebraically-closed-field.md). If some $\operatorname{ad}x$ is not a [nilpotent endomorphism](../../../../../nilpotent-linear-map.md), it has a nonzero [eigenvalue](../../../../../eigenvalue.md) $\lambda$ and an [eigenvector](../../../../../eigenvector.md) $y$, giving $[x,y]=\lambda y$. The vectors $x,y$ are [linearly independent](../../../../../linear-independence.md) and span a nonabelian two-dimensional [Lie subalgebra](../../../../../lie-subalgebra.md). Conversely, a [Lie subalgebra](../../../../../lie-subalgebra.md) of a [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md) is nilpotent because its [lower central series of a Lie algebra](../../../../../lower-central-series-of-a-lie-algebra.md) lies termwise in the ambient series. A nonabelian two-dimensional [Lie algebra](../../../../../lie-algebra-split.md) has a [basis](../../../../../basis.md) $u,v$ with $[u,v]=v$: choose $v$ spanning the nonzero derived algebra and rescale a complementary vector. Its [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) has the nonzero [eigenvalue](../../../../../eigenvalue.md) $1$, so it is not nilpotent. This proves the [two-dimensional subalgebra criterion for Lie algebra nilpotence](../../../../../two-dimensional-subalgebra-criterion-for-lie-algebra-nilpotence.md):

$$
\boxed{\mathfrak g\text{ is nilpotent}\quad\Longleftrightarrow\quad\text{every two-dimensional subalgebra is abelian}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
