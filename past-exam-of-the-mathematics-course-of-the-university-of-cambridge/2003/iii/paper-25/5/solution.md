<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

We state the integer form of [Freiman theorem for integer sets](../../../../../freiman-theorem-for-integer-sets.md): for every $K\ge1$ there are finite constants $r(K),C(K)$ such that every finite nonempty $A\subset\mathbb Z$ with doubling at most $K$ lies in a proper [generalized arithmetic progression](../../../../../generalized-arithmetic-progression.md) of rank at most $r(K)$ and cardinality at most $C(K)|A|$. An arbitrary [abelian group](../../../../../abelian-group.md) requires the coset-progression version, allowing a subgroup factor. We prove the integer statement, with no claim of optimized constants.

We use the allowed [Plünnecke inequality](../../../../../plunnecke-inequality.md) and basic [Freiman isomorphism](../../../../../freiman-2-isomorphism.md) facts, and explicitly prove the modelling, Fourier and covering steps. Two geometry-of-numbers consequences are used as permitted: a cyclic rank-$d$ phase-radius-$\rho$ [Bohr set](../../../../../bohr-set.md) contains a proper symmetric progression of rank at most $d+1$ and size at least $c(d,\rho)$ times the cyclic group order; and a rank-$r$ integer progression with parameter-box volume $V$ can be contained in a proper progression of rank at most $r$ and size at most $c_rV$. These follow from successive minima and lattice basis reduction. All these constants depend only on the displayed rank and radius, not on the ambient order or step sizes.

First construct a dense cyclic model of a large subset. Put $D=8A-8A$ and $q=8|D|$. Plünnecke gives $|D|\le K^{16}|A|$. Choose an auxiliary prime $p$ so large that every nonzero integer in $D$ stays nonzero modulo $p$, and $p>2q$. Arbitrarily large primes exist: a purported finite list would miss a prime divisor of one plus their product. For a uniform nonzero multiplier $\lambda\pmod p$, each nonzero $d\in D$ has $\lambda d$ uniformly distributed among the nonzero residues. The forbidden residues are those represented by nonzero multiples of $q$ with absolute value less than $p$; there are at most $2(p-1)/q$ of them. The union bound gives failure probability at most

$$
(|D|-1)\frac{2(p-1)/q}{p-1}<\frac14.
$$

Thus choose $\lambda$ avoiding them for every nonzero $d\in D$.

Represent the dilated elements of $A$ in $[0,p-1]$, divide this interval into nine consecutive subintervals, and retain a most-populated one. It defines $A'\subseteq A$ with $|A'|\ge|A|/9$. If $u(a)$ is the chosen representative of $\lambda a$, eight-term sums of representatives from this subinterval have a range shorter than $p$: eight times its width is less than $8p/9$. Consequently every original eight-term relation lifts from equality modulo $p$ to equality of the representative sums as integers.

Now reduce these representatives modulo $q$. If their two eight-term sums agree modulo $q$, their integer difference is a multiple of $q$ of absolute value below $p$. A nonzero such difference would give a forbidden residue $\lambda d$ for some nonzero $d\in D$. If $d=0$, its representative difference is already zero. Hence there are no new relations either. The map is therefore a [Freiman s-isomorphism](../../../../../freiman-s-isomorphism.md) of order eight onto $B\subseteq\mathbb Z/q\mathbb Z$. It is injective, by padding shorter relations to eight terms with a fixed retained point. Its density satisfies

$$
\beta=|B|/q\ge\frac1{72K^{16}}.
$$

This proves the [cyclic Freiman model of a small-doubling integer set](../../../../../cyclic-freiman-model-of-a-small-doubling-integer-set.md) needed below.

Next we prove the [cyclic Bogolyubov lemma](../../../../../cyclic-bogolyubov-lemma.md). Use normalized finite-group Fourier analysis on $\mathbb Z/q\mathbb Z$. The convolution

$$
r=1_B*1_B*1_{-B}*1_{-B}
$$

has Fourier expansion $r(x)=\sum_\chi|\widehat{1_B}(\chi)|^4\chi(x)$. Let $\Gamma$ consist of those characters whose Fourier coefficient has modulus at least $\beta^{3/2}/\sqrt2$. Parseval gives $|\Gamma|\le2\beta^{-2}$, and the fourth-power tail outside $\Gamma$ is at most $\beta^4/2$. The zero character belongs to $\Gamma$ and contributes $\beta^4$.

For the phase-distance [Bohr set](../../../../../bohr-set.md) $\mathcal B=\{x:\|\arg\chi(x)/(2\pi)\|\le1/10\text{ for all }\chi\in\Gamma\}$, every retained character has real part at least $\cos(\pi/5)>3/4$. Therefore

$$
r(x)\ge\tfrac34\beta^4-\tfrac12\beta^4>0\quad(x\in\mathcal B).
$$

The support of this convolution is $2B-2B$, so $\mathcal B\subseteq2B-2B$. Apply the stated [progression in a Bohr set from successive minima](../../../../../progression-in-a-bohr-set-from-successive-minima.md) consequence. It supplies a symmetric proper progression $P_B\subseteq2B-2B$ of rank bounded by a function of $K$ and size at least $c(K)q$, hence at least $c(K)|A|$ after adjusting the constant.

Lift this progression back to the integers. The inverse Freiman map induces

$$
\psi:2B-2B\longrightarrow2A'-2A',\qquad
b_1+b_2-b_3-b_4\longmapsto a_1+a_2-a_3-a_4.
$$

Equality of two representations uses a four-term relation on each side, so $\psi$ is well defined and injective. If $y,z,y+z$ all lie in this difference set, the relation between their representations involves at most six original terms on either side. The order-eight model therefore gives $\psi(y+z)=\psi(y)+\psi(z)$ and $\psi(0)=0$. Along every coordinate path within the symmetric progression box, all partial sums remain in $P_B$. It follows that

$$
\psi\left(\sum_i n_iv_i\right)=\sum_i n_i\psi(v_i).
$$

Thus $P=\psi(P_B)$ is a symmetric proper integer progression of the same rank and cardinality, and $P\subseteq2A-2A$. This proves the [Freiman lifting of a progression](../../../../../freiman-lifting-of-a-progression.md) step, including why a sufficiently high-order model was selected.

It remains to cover all of $A$, not merely its large modeled subset. Since $P\subseteq2A-2A$, Plünnecke gives

$$
|A+P|\le|3A-2A|\le K^5|A|.
$$

Choose $X\subseteq A$ maximal such that the translates $x+P$ are pairwise disjoint. Their union lies in $A+P$, so $|X|\le K^5|A|/|P|\le C_1(K)$. For every $a\in A$, maximality makes $a+P$ meet some $x+P$, giving $a\in x+P-P$. Consequently

$$
A\subseteq X+(P-P).
$$

This proves the needed [Ruzsa covering lemma](../../../../../ruzsa-covering-lemma.md) directly.

Write $P=\{\sum_{i=1}^r n_iw_i:|n_i|\le L_i\}$ and $X=\{x_1,\ldots,x_s\}$. The set

$$
Q=\left\{\sum_{j=1}^s\epsilon_jx_j+\sum_{i=1}^rn_iw_i:
\epsilon_j\in\{0,1\},\ |n_i|\le2L_i\right\}
$$

contains $X+(P-P)$ and hence $A$. Its rank is at most $r+s$, bounded only by $K$, and its parameter-box volume is at most $2^{r+s}|P|$. Also $|P|\le|2A-2A|\le K^4|A|$, so this volume is at most $C_2(K)|A|$. The allowed integer properification consequence now contains $Q$ in a proper progression of bounded rank and size at most $C(K)|A|$. Therefore

$$
\boxed{A\subseteq Q'\text{ proper},\qquad\operatorname{rank}Q'\le r(K),\qquad |Q'|\le C(K)|A|.}
$$

This proves Freiman's theorem, using geometry of numbers only in the two explicitly stated places.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
