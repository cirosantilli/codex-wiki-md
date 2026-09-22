<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

We first prove the needed [Petridis minimal-growth lemma](../../../../../petridis-minimal-growth-lemma.md), including the expansion estimate rather than assuming it. For finite nonempty sets $A,B$, choose a nonempty $X\subseteq A$ minimizing $r=|X+B|/|X|$. For any finite set $C=\{c_1,\ldots,c_s\}$, define

$$
X_i=\{x\in X:x+c_i\notin\bigcup_{j<i}(X+c_j)\}.
$$

Then $|X+C|=\sum_i|X_i|$. An element from $(X\setminus X_i)+B+c_i$ has already appeared in an earlier $X+B+c_j$, so the new contribution of $X+B+c_i$ has size at most

$$
|X+B|-|(X\setminus X_i)+B|\leq r|X|-r|X\setminus X_i|=r|X_i|.
$$

The inequality follows from minimality of $r$ on subsets of $A$, with an empty subset contributing zero. Summing proves $|X+B+C|\leq r|X+C|$. Iteration gives $|X+jB|\leq r^j|X|$, for every $j\geq0$; in particular, $|jB|\leq r^j|X|$ by translating $jB$ into $X+jB$.

Apply this with $B=A$, so $r\leq K$. It follows that

$$
\boxed{|\ell A|\leq K^\ell|A|=K^\ell N\quad(\ell\geq2).}
$$

This is the required [Plünnecke inequality](../../../../../plunnecke-inequality.md).

We will also use the mixed-[sumset](../../../../../sumset.md) bound $|mA-nA|\leq K^{m+n}N$. To justify it, the [Ruzsa triangle inequality](../../../../../ruzsa-triangle-inequality.md) says

$$
|P-Q|\,|T|\leq|P-T|\,|T-Q|.
$$

Choose one representation $z=p_z-q_z$ for each $z\in P-Q$. The map $(z,t)\mapsto(p_z-t,t-q_z)$ is injective: adding the two coordinates recovers $z$, then the chosen representation recovers $t$. This proves the inequality. Apply it with $P=mA$, $Q=nA$, $T=-X$ and the minimal-growth set already chosen. The bounds on $X+mA$ and $X+nA$ give the mixed-[sumset](../../../../../sumset.md) estimate, including $0A=\{0\}$.

The [Ruzsa covering lemma](../../../../../ruzsa-covering-lemma.md) states: if $S,T$ are finite, $T\ne\varnothing$, and $|S+T|\leq L|T|$, then there is $D\subseteq S$, $|D|\leq L$, such that $S\subseteq D+T-T$. Choose $D$ maximal with the translates $d+T$, $d\in D$, pairwise disjoint. They lie in $S+T$, so $|D||T|\leq|S+T|$. Maximality says each $s+T$ meets some $d+T$, which writes $s=d+t_1-t_2$. This proves both assertions.

Let $T=A-A$. The mixed-[sumset](../../../../../sumset.md) bounds give $|T|\leq K^2N$ and $|2T+A|=|3A-2A|\leq K^5N$. Apply the [Ruzsa covering lemma](../../../../../ruzsa-covering-lemma.md) to $S=2T$ and the set $A$. There is $D\subseteq2T$ of size $q\leq K^5$ with

$$
2T\subseteq D+T.
$$

Induction then gives $\ell T\subseteq(\ell-1)D+T$. The number of possible sums of $\ell-1$ elements from the $q$-element set $D$ is at most the number of multiplicity vectors, namely $\binom{\ell+q-2}{q-1}$. Since $A-a_0\subseteq T$ for any $a_0\in A$, we obtain the explicit [polynomial growth of iterated sumsets](../../../../../polynomial-growth-of-iterated-sumsets.md)

$$
\boxed{|\ell A|\leq K^2\binom{\ell+q-2}{q-1}N,\qquad 1\leq q\leq K^5.}
$$

For fixed $K>1$, this polynomial in $\ell$ is eventually smaller than $K^{\epsilon\ell}$. For example, take $q_*=\lceil K^5\rceil$ and choose $\ell_0(K,\epsilon)$ so that $2\log K+q_*\log(\ell+q_*)\leq\epsilon\ell\log K$ for every $\ell\geq\ell_0$; such a threshold exists because $\log\ell/\ell\to0$. Therefore

$$
\boxed{|\ell A|\leq K^{\epsilon\ell}N\quad\text{for all }\ell\geq\ell_0(K,\epsilon).}
$$

For $K=1$, a finite integer set has $|A+A|\geq2|A|-1$ (list the increasing sums $a_1+a_1,\ldots,a_1+a_N,a_2+a_N,\ldots,a_N+a_N$). Thus $N=1$, and the asserted bound holds for every $\ell$. Nonemptiness is implicit in the [doubling constant](../../../../../doubling-constant.md) hypothesis.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
