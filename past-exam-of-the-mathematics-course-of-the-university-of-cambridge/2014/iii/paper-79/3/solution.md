<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We will prove a [polynomial progression in a high-energy fourfold difference set](../../../../../polynomial-progression-in-a-high-energy-fourfold-difference-set.md). The route is to extract a large subset with a small [difference set](../../../../../difference-set.md), construct a dense [Freiman s-isomorphism](../../../../../freiman-s-isomorphism.md) model, and use the [Bogolyubov lemma](../../../../../bogolyubov-lemma.md) and the [pigeonhole principle](../../../../../pigeonhole-principle.md). To respect the proof requirement, every ingredient beyond the elementary rules for [Freiman homomorphisms](../../../../../freiman-homomorphism.md) is established below.

Assume $n\geq1$. Since three entries of an [additive quadruple](../../../../../additive-quadruple.md) determine the fourth, $E(A)\leq n^3$, so a nonvacuous hypothesis has $0<\theta\leq1$. Let $r(t)=|\{(a,b)\in A^2:a+b=t\}|$. Then $E(A)=\sum_t r(t)^2$ and $\sum_t r(t)=n^2$. Define the [popular sum](../../../../../popular-sum.md) set $S=\{t:r(t)\geq\theta n/2\}$. The contribution to [additive energy](../../../../../additive-energy.md) from its complement is at most $\theta n^3/2$. Since $r(t)\leq n$, the [bipartite graph](../../../../../bipartite-graph.md) on two copies of $A$ whose edges have sums in $S$ has at least $\theta n^2/2$ edges. Moreover $|S|\leq2n/\theta$.

Put $\delta=\theta/2$ and $\tau=\delta^2/16$. Here is a [dependent random choice](../../../../../dependent-random-choice.md) argument producing the small [difference set](../../../../../difference-set.md). Independently choose two right vertices, allowing repetition, and let $X$ be their common left neighbourhood. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $\mathbb E|X|\geq\delta^2n$. Call an ordered pair of left vertices bad if its common right neighbourhood has fewer than $\tau n$ elements. The expected number $b(X)$ of bad ordered pairs in $X$ is at most $\tau^2n^2$, because a fixed bad pair survives both random choices with probability at most $\tau^2$. Thus

$$
\mathbb E\left(|X|-\frac{64b(X)}{\delta^2n}\right)\geq\frac34\delta^2n.
$$

Choose a realization attaining at least this expectation. Then $|X|\geq3\delta^2n/4$, and $b(X)\leq\delta^2n|X|/64\leq|X|^2/48$. Remove from $X$ every vertex having more than $|X|/4$ bad partners in $X$. At most $|X|/12$ vertices are removed. The remaining set $B$ has $|B|\geq\delta^2n/2$, and any $a,b\in B$ have at least $|X|/2$ vertices $z\in X$ for which both $(a,z)$ and $(z,b)$ are good.

For such a $z$, there are at least $\tau n$ right vertices $y$ adjacent to $a,z$, and at least $\tau n$ right vertices $y'$ adjacent to $z,b$. These paths give

$$
a-b=(a+y)-(z+y)+(z+y')-(b+y'),
$$

a representation with four members of $S$. For fixed $a,b$, the tuple of four sums determines $y,z,y'$ uniquely, so there are at least $|X|\tau^2n^2/2$ distinct tuples. Select one ordered pair $a,b$ for each member of $B-B$. Tuples belonging to different differences are disjoint. Counting all possible tuples in $S^4$ proves

$$
|B-B|\leq\frac{2|S|^4}{|X|\tau^2n^2}\leq D_\theta n,
\qquad D_\theta=2^{22}\theta^{-10}.
$$

In particular, with $m=|B|$, we have $m\geq\theta^2n/8$ and $|B-B|\leq K m$ for $K=2^{25}\theta^{-12}$. This is the required small-[difference set](../../../../../difference-set.md) form of the [Balog-Szemerédi-Gowers theorem](../../../../../balog-szemeredi-gowers-theorem.md), proved by counting paths rather than cited.

We next control higher [iterated sumsets](../../../../../iterated-sumset.md). Choose a nonempty $X\subseteq B$ minimizing $\rho=|X-B|/|X|$, so $\rho\leq K$. We prove the [Petridis minimal-growth lemma](../../../../../petridis-minimal-growth-lemma.md) in the form $|X-B+C|\leq\rho|X+C|$ for finite $C$. Order $C=\{c_1,\ldots,c_t\}$, and let $X_i$ consist of those $x\in X$ for which $x+c_i$ is new in the union of the translates $X+c_j$. Then $\sum_i|X_i|=|X+C|$. Every member of $(X\setminus X_i)-B+c_i$ already occurs in an earlier translate of $X-B$. By minimality, $|(X\setminus X_i)-B|\geq\rho|X\setminus X_i|$, also when the complement is empty. Thus the new contribution from $X-B+c_i$ is at most $\rho|X_i|$. Sum over $i$ to prove the lemma. Iterating with $C=-(j-1)B$ gives $|X-jB|\leq K^j|X|$.

For completeness, the [Ruzsa triangle inequality](../../../../../ruzsa-triangle-inequality.md) in the needed form is

$$
|U-W|\,|V|\leq|U-V|\,|V-W|.
$$

For each $d\in U-W$, fix $d=u_d-w_d$. The map $(d,v)\mapsto(u_d-v,v-w_d)$ is injective: adding the coordinates recovers $d$, and then $v$. Take $U=kB$, $W=\ell B$, $V=X$ and apply the preceding bounds. We obtain the [Plünnecke-Ruzsa inequality](../../../../../plunnecke-ruzsa-inequality.md)

$$
|kB-\ell B|\leq K^{k+\ell}|X|\leq K^{k+\ell}m.
$$

In particular $T=8B-8B$ has at most $K^{16}m$ elements.

We now prove a slightly wasteful version of the [Ruzsa modeling lemma](../../../../../ruzsa-modelling-lemma.md), avoiding any assumption about the diameter of $B$. Set $q=8|T|$. Choose a prime $p$ larger than all $|t|$, $t\in T$, and much larger than $q$. Arbitrarily large primes exist by the elementary argument that a prime divisor of one plus the product of all primes up to a given bound exceeds that bound. For a uniformly chosen nonzero multiplier $r$ modulo $p$, each nonzero $t\in T$ has $rt$ uniform among the nonzero residues. Call a multiplier forbidden if some such $rt$ agrees modulo $p$ with $jq$, where $|jq|<p$. There are at most $2p/q+1\leq3p/q$ such residues. For $p\geq4$, a [union bound](../../../../../boole-s-inequality.md) therefore makes the probability of being forbidden less than

$$
\frac{4(|T|-1)}q<\frac12.
$$

Choose a nonforbidden $r$. Represent $rB$ by integers in $[0,p-1]$ and partition that interval into sixteen consecutive pieces of diameter less than $p/16$. One piece contains the images of a subset $B'\subseteq B$ with $|B'|\geq m/16$. Let $\phi(b)$ be the integer representative of $rb$ in that piece, reduced modulo $q$.

A difference of eight sums of these representatives has absolute value less than $p/2$. If its original difference in $B$ is zero, it is a multiple of $p$, hence zero. Conversely, if its reduction modulo $q$ is zero, it equals $jq$ with $|jq|<p$; our choice of $r$ forces its original difference to be zero. This proves that $\phi$ is a [Freiman s-isomorphism](../../../../../freiman-s-isomorphism.md) of order eight. Injectivity follows by padding a one-term equality to eight terms with a fixed element. Consequently $D=\phi(B')\subseteq G=\mathbb Z/q\mathbb Z$ has [subset density](../../../../../density-of-a-finite-subset.md)

$$
\alpha=|D|/q\geq\alpha_0:=\frac1{128K^{16}},
\qquad q\geq8m\geq\theta^2n.
$$

No primality of $q$ is needed.

Here is the cyclic [Bogolyubov lemma](../../../../../bogolyubov-lemma.md) with all its [Fourier analysis on a finite abelian group](../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md) details. Use $\widehat f(r)=\mathbb E_xf(x)e(-rx/q)$, $f=1_D$, and [normalized convolution on a finite group](../../../../../normalized-convolution-on-a-finite-group.md). A [finite geometric series](../../../../../finite-geometric-series.md) proves orthogonality, and expanding the finite sums proves the [Parseval identity on a finite group](../../../../../parseval-identity-on-a-finite-group.md), [Fourier inversion on a finite group](../../../../../fourier-inversion-on-a-finite-group.md), and $\widehat{f*g}=\widehat f\widehat g$. For $\widetilde f(x)=f(-x)$, the nonnegative function

$$
F=f*f*\widetilde f*\widetilde f
$$

has support exactly $2D-2D$ and [Fourier coefficients on a finite abelian group](../../../../../fourier-coefficient-on-a-finite-abelian-group.md) $|\widehat f(r)|^4$. Put $\Gamma=\{r\ne0:|\widehat f(r)|\geq\alpha^{3/2}/\sqrt8\}$. The [Parseval identity on a finite group](../../../../../parseval-identity-on-a-finite-group.md) gives $|\Gamma|\leq8\alpha^{-2}$. The total fourth moment of the frequencies outside $\Gamma\cup\{0\}$ is at most $\alpha^4/8$.

If $\|rx/q\|\leq1/16$ for every $r\in\Gamma$, then $\operatorname{Re}e(rx/q)\geq\cos(\pi/8)>3/4$. The zero frequency contributes $\alpha^4$ with no loss. Separating the large and small frequencies in [Fourier inversion on a finite group](../../../../../fourier-inversion-on-a-finite-group.md) yields

$$
F(x)\geq\frac34\sum_r|\widehat f(r)|^4-\frac74\frac{\alpha^4}{8}
\geq\frac{17}{32}\alpha^4>0.
$$

Thus $2D-2D$ contains the [Bohr set](../../../../../bohr-set.md) expressed in distance coordinates by $\|rx/q\|\leq1/16$. This is consistent with the existing character-distance convention for a [Bohr set](../../../../../bohr-set.md): here it is enough that each character lies in the corresponding short arc around one.

We finally prove the needed [nonwrapping progression in a cyclic Bohr set](../../../../../nonwrapping-progression-in-a-cyclic-bohr-set.md), including for composite $q$. Write $d=|\Gamma|$ and $Q=\lfloor q^{1/(d+1)}\rfloor$. Partition the $d$-dimensional unit cube into $Q^d$ boxes. The $Q^d+1$ points with coordinates $jr/q$ modulo one, $0\leq j\leq Q^d$, give by the [pigeonhole principle](../../../../../pigeonhole-principle.md) an integer $1\leq t\leq Q^d$ with $\|rt/q\|\leq1/Q$ for all $r\in\Gamma$. Then

$$
P=\{0,t,2t,\ldots,\lfloor Q/16\rfloor t\}\subseteq2D-2D.
$$

These points are distinct modulo $q$, since their integer representatives lie between zero and $Q^{d+1}/16\leq q/16$. Their number is at least $q^{1/(d+1)}/32$. For $d=0$ the same argument simply chooses $t=1$.

The [Freiman s-isomorphism](../../../../../freiman-s-isomorphism.md) induces a bijection $\Phi:2B'-2B'\to2D-2D$: define it on a representation by taking the same two positive and two negative images. Equality of representations uses an order-four relation, and injectivity uses the converse relation. If three consecutive members $y_{j-1},y_j,y_{j+1}$ of $P$ satisfy $y_{j-1}+y_{j+1}=2y_j$, their preimages satisfy the same equality, since its expansion is an equality of eight-term sums in $B'$. Hence the inverse image of $P$ is an ordinary [arithmetic progression](../../../../../arithmetic-progression.md) in $2B'-2B'\subseteq2A-2A$, with distinct terms.

To remove the multiplicative constant from the length bound, let $R=\lceil8\alpha_0^{-2}\rceil$ and $\beta=1/(R+1)$. The length just proved is at least $c_\theta n^\beta$, where $c_\theta=\theta^{2\beta}/32>0$. Choose $N_0\geq3$ so that $c_\theta n^\beta\geq n^{\beta/2}$ for $n\geq N_0$, and set $\gamma=\min\{\beta/2,\log3/\log N_0\}$. For $2\leq n<N_0$, two distinct members of $A$ give a nonzero $u\in A-A$, and $\{-u,0,u\}\subseteq2A-2A$ has length three, at least $n^\gamma$. For $n=1$, the singleton $\{0\}$ suffices. **In every nonempty case,**

$$
\boxed{2A-2A\text{ contains a nonconstant progression of length at least }n^\gamma\quad(n\geq2),}
$$

with $\gamma>0$ depending only on $\theta$. If empty sets are permitted, the required length is zero and there is no substantive assertion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 79](../../paper-79-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
