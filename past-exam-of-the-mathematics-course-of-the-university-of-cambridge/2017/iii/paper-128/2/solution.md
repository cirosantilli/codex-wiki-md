<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [right Noetherian ring](../../../../../right-noetherian-ring.md) satisfies the [ascending chain condition](../../../../../ascending-chain-condition.md) on [right ideals](../../../../../right-ideal.md); equivalently, every [right ideal](../../../../../right-ideal.md) is a [finitely generated module](../../../../../finitely-generated-module.md).

Here is a [noncommutative Hilbert basis theorem](../../../../../noncommutative-hilbert-basis-theorem.md) proof adapted to the stated hypothesis. Set $F_{-1}=0$ and

$$
F_n=\sum_{i=0}^n Ax^i=\sum_{i=0}^n x^iA.
$$

The equality follows inductively from $A+xA=A+Ax$, by moving one coefficient past one $x$ at a time. These spaces form an exhaustive [filtered algebra](../../../../../filtered-algebra.md) structure on $B$, with $F_nF_m\subseteq F_{n+m}$. This does not assert uniqueness of the displayed expressions or the existence of a coefficient-moving [automorphism](../../../../../automorphism.md).

For a [right ideal](../../../../../right-ideal.md) $I\subseteq B$, define

$$
L_n=\{a\in A:ax^n\in I+F_{n-1}\}.
$$

Each $L_n$ is a [right ideal](../../../../../right-ideal.md) of $A$. In fact, if $a\in L_n$ and $c\in A$, write $cx^n=x^nb+u$ with $b\in A$, $u\in F_{n-1}$; then $acx^n=(ax^n)b+au\in I+F_{n-1}$. Also $L_n\subseteq L_{n+1}$ by right multiplication by $x$. Since $A$ is a [right Noetherian ring](../../../../../right-noetherian-ring.md), this ascending chain stabilizes at some $L_N$.

Choose finite generators $a_{nj}$ for each $L_n$, $0\leq n\leq N$, and choose $f_{nj}\in I$ with $f_{nj}-a_{nj}x^n\in F_{n-1}$. These finitely many elements generate $I$ as a [right ideal](../../../../../right-ideal.md). To see this, induct on $m$ for $f\in I\cap F_m$. Write $f=ax^m+u$ with $u\in F_{m-1}$; then $a\in L_m$. Put $d=\min(m,N)$ and express $a=\sum_j a_{dj}c_j$. Write $c_jx^d=x^db_j+u_j$ with $u_j\in F_{d-1}$. The difference

$$
f-\sum_j f_{dj}b_jx^{m-d}
$$

lies in $I\cap F_{m-1}$, so the induction applies. At $m=0$ the remainder is zero. Hence **$B$ is right Noetherian**.

For the [quantum torus](../../../../../quantum-torus.md), take $q\in k^\times$ and the convention $YX=qXY$. Begin with the [polynomial ring](../../../../../polynomial-ring.md) $k[X]$, which is [Noetherian](../../../../../noetherian-ring.md) by the [Hilbert basis theorem](../../../../../hilbert-basis-theorem.md). Adjoining $X^{-1}$ preserves the hypothesis because it commutes with $k[X]$, and gives $k[X^{\pm1}]$. Adjoin $Y$ next. The relation $Yf(X)=f(qX)Y$ and its inverse coefficient-moving relation give $A+YA=A+AY$ for $A=k[X^{\pm1}]$. Finally adjoin $Y^{-1}$ to $k[X^{\pm1}][Y;\sigma]$, where $\sigma(X)=qX$. On a [monomial](../../../../../monomial.md), $Y^{-1}X^iY^j=q^{-i}X^iY^{j-1}$; when $j=0$ this is in $AY^{-1}$, and when $j>0$ it is in $A$. The reverse inclusion follows by the same relation. The preceding argument applies at each step, proving **the quantum torus is right Noetherian**. Nonzero $q$ is required for this notation.

For a [noncommutative ring](../../../../../noncommutative-ring.md), a [prime ideal of a noncommutative ring](../../../../../prime-ideal-of-a-noncommutative-ring.md) means a proper two-sided [ideal](../../../../../ideal.md) $P$ such that $UV\subseteq P$ for two-sided [ideals](../../../../../ideal.md) $U,V$ implies $U\subseteq P$ or $V\subseteq P$. Equivalently, $aAb\subseteq P$ implies $a\in P$ or $b\in P$. This definition does not require $A/P$ to be a [noncommutative domain](../../../../../noncommutative-domain.md).

Retain the [right Noetherian ring](../../../../../right-noetherian-ring.md) hypothesis for the last assertion. More generally, the [ascending chain condition](../../../../../ascending-chain-condition.md) on two-sided [ideals](../../../../../ideal.md) suffices. We claim that every proper two-sided [ideal](../../../../../ideal.md) $I$ contains a product of finitely many [prime ideals of a noncommutative ring](../../../../../prime-ideal-of-a-noncommutative-ring.md), each containing $I$. If not, choose a maximal counterexample $I$. It cannot be a [prime ideal of a noncommutative ring](../../../../../prime-ideal-of-a-noncommutative-ring.md). Thus there are two-sided [ideals](../../../../../ideal.md) $U,V$ strictly containing $I$ with $UV\subseteq I$: add $I$ to the two witnesses for failure of the defining condition for a [prime ideal of a noncommutative ring](../../../../../prime-ideal-of-a-noncommutative-ring.md). By maximality, both $U$ and $V$ contain products of finitely many [prime ideals of a noncommutative ring](../../../../../prime-ideal-of-a-noncommutative-ring.md) containing them. Concatenating these products gives a product inside $UV\subseteq I$, a contradiction.

Apply the claim to $I=0$ in a nonzero $A$, obtaining $P_1\cdots P_r=0$. Every [prime ideal of a noncommutative ring](../../../../../prime-ideal-of-a-noncommutative-ring.md) $Q$ contains one of the $P_i$, by repeated application of the definition of a [prime ideal of a noncommutative ring](../../../../../prime-ideal-of-a-noncommutative-ring.md). For the [prime radical of a noncommutative ring](../../../../../prime-radical-of-a-noncommutative-ring.md) $N$, it follows that

$$
\boxed{N=P_1\cap\cdots\cap P_r,\qquad N^r=0.}
$$

Indeed, $N\subseteq P_i$ gives $N^r\subseteq P_1\cdots P_r=0$, and $\bigcap_iP_i\subseteq Q$ for every $Q$ gives equality of the intersections. If $A=0$, the empty intersection is the whole zero [ring](../../../../../ring.md) and the conclusion is immediate.

The final assertion is false for arbitrary [algebras](../../../../../algebra-split.md) without the preceding chain condition. For example, in the commutative [ring](../../../../../ring.md) $k[z_1,z_2,\ldots]/(z_i^2:i\geq1)$ the [nilradical](../../../../../nilradical.md) is $(z_1,z_2,\ldots)$, its only [prime ideal](../../../../../prime-ideal.md), but the product of any number of distinct $z_i$ is nonzero. Thus this [nilradical](../../../../../nilradical.md) is not a [nilpotent ideal](../../../../../nilpotent-ideal.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 128](../../paper-128-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
