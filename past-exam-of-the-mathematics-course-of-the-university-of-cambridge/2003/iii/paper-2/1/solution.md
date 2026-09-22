<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $R$ be a commutative [Artinian ring](../../../../../artinian-ring.md). We prove finite [composition length](../../../../../composition-length.md) first, without assuming the conclusion that $R$ is [Noetherian](../../../../../noetherian-ring.md).

Every [prime ideal](../../../../../prime-ideal.md) is maximal. Indeed, an Artinian [integral domain](../../../../../integral-domain.md) is a field: for $a\ne0$, stabilization of $(a^m)$ gives $a^m=a^{m+1}b$, and cancellation gives $ab=1$. There are only finitely many [maximal ideals](../../../../../maximal-ideal.md). To see this, choose a minimal finite intersection $L=\mathfrak m_1\cap\cdots\cap\mathfrak m_s$ using the [descending chain condition](../../../../../descending-chain-condition.md). Minimality gives $L\subseteq\mathfrak m$ for any other maximal ideal $\mathfrak m$. Since $\mathfrak m_1\cdots\mathfrak m_s\subseteq L$, primeness forces one $\mathfrak m_i\subseteq\mathfrak m$, and maximality makes them equal. Thus the [Jacobson radical](../../../../../jacobson-radical.md) $J$ is this finite intersection, and the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) gives

$$
R/J\cong\prod_{i=1}^sR/\mathfrak m_i.
$$

We also need nilpotence of $J$. Its powers stabilize; put $I=J^m$ at a stabilization stage, so $I^2=I$. If $I\ne0$, choose an ideal $L$ minimal subject to $IL\ne0$. Since $I(IL)=IL\ne0$, minimality gives $IL=L$. Choose $a\in L$ with $Ia\ne0$. Minimality applied to the subideal $Ra$ gives $L=Ra$. The equality $IL=L$ then yields $a=xa$ for some $x\in I\subseteq J$. But $1-x$ is a unit by the [unit criterion for the Jacobson radical](../../../../../unit-criterion-for-the-jacobson-radical.md); hence $a=0$, a contradiction. Therefore $J^m=0$.

Each layer $J^i/J^{i+1}$ is an [Artinian module](../../../../../artinian-module.md) over the finite product of fields $R/J$. Its components over those fields are finite-dimensional: an infinite-dimensional vector space has a strictly descending chain of subspaces. Each layer consequently has finite [composition length](../../../../../composition-length.md). The finite filtration

$$
R\supset J\supset\cdots\supset J^m=0
$$

proves that $R$ itself has finite [composition length](../../../../../composition-length.md), and therefore satisfies the [ascending chain condition](../../../../../ascending-chain-condition.md) on ideals. **Every commutative Artinian ring is Noetherian.** The zero ring satisfies the conclusion trivially.

The relevant [Artin–Wedderburn theorem](../../../../../artin-wedderburn-theorem.md) says that a [semisimple ring](../../../../../semisimple-ring.md) which is a [right Artinian ring](../../../../../right-artinian-ring.md) has the form

$$
\boxed{R\cong\prod_{i=1}^sM_{n_i}(D_i),}
$$

where the $D_i$ are [division rings](../../../../../division-ring.md) and the positive integers $n_i$ and division rings are unique up to permutation and isomorphism. The division rings need not be commutative or finite-dimensional over a field. Conversely every such finite product is semisimple and a [right Artinian ring](../../../../../right-artinian-ring.md).

Here is a proof which also works if semisimplicity is initially expressed as $J(R)=0$. A nonzero right ideal contains a minimal nonzero [right ideal](../../../../../right-ideal.md) $L$ by the [descending chain condition](../../../../../descending-chain-condition.md); $L$ is a [simple module](../../../../../irreducible-module.md). If $L^2=0$, then for every $l\in L$ and $r\in R$, $(lr)^2=0$, so $1-lr$ has inverse $1+lr$. The [unit criterion for the Jacobson radical](../../../../../unit-criterion-for-the-jacobson-radical.md) would give $L\subseteq J(R)=0$, a contradiction. Thus some $a\in L$ induces a nonzero map $L\to L$ by left multiplication. This map is an isomorphism, since $L$ is simple. Choose $e\in L$ with $ae=a$. Then $a(e^2-e)=0$ and injectivity on $L$ gives $e^2=e$. We obtain $L=eR$ and the splitting

$$
R_R=eR\oplus(1-e)R.
$$

For a right ideal $K$ containing $e$, the same argument splits $K=eR\oplus(K\cap(1-e)R)$. Repeatedly split a minimal right ideal out of the remaining summand. The remaining summands form a strictly descending chain of right ideals, so the process terminates. Thus

$$
R_R\cong\bigoplus_{i=1}^sS_i^{\oplus n_i}
$$

for pairwise nonisomorphic [simple modules](../../../../../irreducible-module.md) $S_i$.

A nonzero map between [simple modules](../../../../../irreducible-module.md) is an isomorphism: its kernel and image leave no alternatives. Thus $D_i=\operatorname{End}_R(S_i)$ is a [division ring](../../../../../division-ring.md), and $\operatorname{Hom}_R(S_i,S_j)=0$ for $i\ne j$. This is the needed [Schur lemma](../../../../../schur-s-lemma.md). Taking endomorphisms of the direct sum gives $\prod_iM_{n_i}(D_i)$. Finally, left multiplication identifies $R$ with $\operatorname{End}_R(R_R)$: a right-module endomorphism sends $r$ to $f(1)r$, and composition corresponds to multiplication in $R$, not its opposite. This proves the displayed ring isomorphism.

For the converse, the right regular module of $M_n(D)$ is the direct sum of its $n$ row modules. Each row module is simple, since elementary matrices and nonzero scalar inverses send any nonzero row to any prescribed row. A finite product therefore has a finite semisimple regular module and is a [right Artinian ring](../../../../../right-artinian-ring.md). The simple-module multiplicities and their endomorphism division rings recover the factors, establishing uniqueness.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
