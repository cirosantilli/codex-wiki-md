<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove closure using [complete reducibility of semisimple Lie algebra representations](../../../../../../weyl-s-theorem-on-complete-reducibility.md), rather than assuming that a [Lie subalgebra](../../../../../../lie-subalgebra.md) is closed under polynomials in its elements. Write the matrix [Jordan–Chevalley decomposition](../../../../../../jordan-chevalley-decomposition.md) as $X=S+N$. On $\operatorname{End}(V)$, the [commutator](../../../../../../commutator.md) operator $\operatorname{ad}S$ is diagonalizable: if $S$ has eigenspaces $V_\lambda$, then its eigenvalue on $\operatorname{Hom}(V_\lambda,V_\mu)$ is $\mu-\lambda$. The operator $\operatorname{ad}N$ is nilpotent: if $N^r=0$, then

$$
(\operatorname{ad}N)^k(A)=\sum_{j=0}^k(-1)^j\binom{k}{j}N^{k-j}AN^j=0\qquad(k\geq2r-1).
$$

The two operators commute because $[S,N]=0$. Uniqueness of the [Jordan–Chevalley decomposition](../../../../../../jordan-chevalley-decomposition.md) therefore says that $\operatorname{ad}S$ is the semisimple part of $\operatorname{ad}X$. Since a matrix's semisimple part is a polynomial in that matrix, and $\mathfrak g$ is invariant under $\operatorname{ad}X$, it follows that

$$
[S,\mathfrak g]\subseteq\mathfrak g.
$$

Now regard $\operatorname{End}(V)$ as a [Lie algebra representation](../../../../../../lie-algebra-representation.md) of $\mathfrak g$ under commutators. By [complete reducibility of semisimple Lie algebra representations](../../../../../../weyl-s-theorem-on-complete-reducibility.md), there is an invariant complement $M$ with $\operatorname{End}(V)=\mathfrak g\oplus M$. Write $S=Y+C$, with $Y\in\mathfrak g$ and $C\in M$. For $A\in\mathfrak g$, the normalization property gives $[C,A]=[S,A]-[Y,A]\in\mathfrak g$, while invariance of $M$ gives $[C,A]\in M$. Thus $[C,A]=0$: $C$ commutes with the whole [Lie algebra](../../../../../../lie-algebra-split.md).

Decompose $V=\bigoplus_jV_j$ into irreducible $\mathfrak g$-modules. Each $V_j$ is preserved by $X$, hence by its polynomial parts $S,N$, and also by $Y$; therefore it is preserved by $C$. By the [Schur lemma](../../../../../../schur-s-lemma.md), $C|_{V_j}=c_jI$. A [semisimple Lie algebra](../../../../../../semisimple-lie-algebra-split.md) is a [perfect Lie algebra](../../../../../../perfect-lie-algebra.md), so every element is a sum of [Lie brackets](../../../../../../lie-bracket.md) and has trace zero on every finite-dimensional representation. Consequently $\operatorname{tr}(X|_{V_j})=\operatorname{tr}(Y|_{V_j})=0$. Also $N|_{V_j}$ is nilpotent, so it has trace zero; hence

$$
\operatorname{tr}(S|_{V_j})=0,\qquad c_j\dim V_j=\operatorname{tr}(C|_{V_j})=0.
$$

Thus every $c_j$ is zero, $C=0$, and $S=Y\in\mathfrak g$. Finally $N=X-S\in\mathfrak g$. We have proved

$$
\boxed{X_s,X_n\in\mathfrak g.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
