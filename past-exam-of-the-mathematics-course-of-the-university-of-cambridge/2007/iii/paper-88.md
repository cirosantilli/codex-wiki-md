# Paper 88

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper88.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper88.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 88](paper-88.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Assume $A$ is finite and nonempty; the empty case is immediate. Here $2A=A+A$. Choose a nonempty [subset](../../../set.md#subset) $X\subseteq A$ minimizing

$$
K=\frac{|X+A|}{|X|}.
$$

Taking $X=A$ as a competitor gives $K\leq C$, and every [subset](../../../set.md#subset) $Y\subseteq X$ satisfies $|Y+A|\geq K|Y|$, including $Y=\varnothing$.

We first prove the [Petridis minimal-growth lemma](../../../additive-combinatorics.md#petridis-minimal-growth-lemma) in the particular form needed: for every [finite set](../../../set.md#finite-set) $S$,

$$
|X+A+S|\leq K|X+S|.
$$

List $S=\{s_1,\ldots,s_t\}$ and let $X_j$ consist of those $x\in X$ for which $x+s_j$ does not belong to an earlier translate $X+s_h$, $h<j$. The [sets](../../../set.md) $X_j+s_j$ partition $X+S$, so $|X+S|=\sum_j|X_j|$.

If $x\in X\setminus X_j$, then $x+s_j=x'+s_h$ for some earlier $h$ and $x'\in X$. Hence every point of $x+A+s_j$ already belongs to $X+A+s_h$. Therefore the new points contributed by $(X+A)+s_j$ are contained in

$$
\bigl[(X+A)\setminus((X\setminus X_j)+A)\bigr]+s_j.
$$

Their number is at most

$$
|X+A|-|(X\setminus X_j)+A|\leq K|X|-K|X\setminus X_j|=K|X_j|.
$$

Summing over $j$ proves the lemma. With $S=A$, it gives

$$
|X+2A|\leq K|X+A|=K^2|X|.
$$

We also prove the [Ruzsa triangle inequality](../../../additive-combinatorics.md#ruzsa-triangle-inequality) directly. For each $d\in U-V$, choose one representation $d=u_d-v_d$. The map

$$
(d,x)\longmapsto(x+u_d,x+v_d)
$$

from $(U-V)\times X$ into $(X+U)\times(X+V)$ is [injective](../../../algebra.md#injective-function): subtracting the output coordinates recovers $d$, after which either coordinate recovers $x$. Thus $|U-V||X|\leq|X+U||X+V|$. Taking $U=V=2A$ now yields

$$
\boxed{|2A-2A|\leq\frac{|X+2A|^2}{|X|}\leq K^4|X|\leq C^4|A|.}
$$

This proves the required growth and [difference set](../../../additive-combinatorics.md#difference-set) estimates directly.

## 2

↑ **Parent:** [Paper 88](paper-88.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A quantitative form of [Roth theorem on three-term arithmetic progressions](../../../additive-combinatorics.md#roth-theorem-on-three-term-arithmetic-progressions) is: there is an absolute constant $C_R$ such that, for $N\geq3$, every $A\subseteq[N]$ with no nonconstant three-term [arithmetic progression](../../../arithmetic.md#arithmetic-progression) satisfies

$$
\boxed{|A|\leq C_R\frac{N}{\log\log N}.}
$$

All logarithms below are natural. We prove the [classical Roth bound for three-term progressions](../../../additive-combinatorics.md#classical-roth-bound-for-three-term-progressions) with an unoptimized $C_R=100$. The empty [set](../../../set.md) is immediate; write $\delta=|A|/N>0$.

First establish a quantitative [density increment](../../../additive-combinatorics.md#density-increment). Suppose $N\geq4\cdot10^6\delta^{-4}$. Put $M=2N+1$, embed $I=[N]$ in $G=\mathbb Z_M$, and extend all interval [functions](../../../function.md) by zero. Let $a=1_A$, $u=\delta1_I$ and $f=a-u$, the [balanced subset indicator](../../../additive-combinatorics.md#balanced-indicator-function-of-a-finite-subset). Define

$$
\widehat g(r)=\sum_{x\in G}g(x)e^{-2\pi irx/M},\qquad\Lambda(g_1,g_2,g_3)=\sum_{x+z=2y}g_1(x)g_2(y)g_3(z).
$$

The relation in the sum is modulo $M$. For interval elements its [integer](../../../number-theory.md#integer) discrepancy has absolute value less than $M$, so it is precisely the [integer](../../../number-theory.md#integer) relation. Thus $\Lambda(a,a,a)=|A|=\delta N$. The full interval count is the number of endpoint pairs of the same parity:

$$
\Lambda(1_I,1_I,1_I)=\lceil N/2\rceil^2+\lfloor N/2\rfloor^2\geq N^2/2.
$$

Consequently, since $N\geq4\delta^{-2}$,

$$
\Lambda(u,u,u)-\Lambda(a,a,a)\geq\frac{\delta^3N^2}{4}.
$$

Orthogonality of the [additive characters](../../../analysis.md#additive-character) gives

$$
\Lambda(g_1,g_2,g_3)=\frac1M\sum_r\widehat g_1(r)\widehat g_2(-2r)\widehat g_3(r),\qquad\frac1M\sum_r|\widehat g(r)|^2=\sum_x|g(x)|^2.
$$

Both identities follow by expanding the sums and using $\sum_re^{2\pi irt/M}=M$ for $t=0$ in $G$, and zero otherwise; the latter follows from a [finite geometric series](../../../real-analysis.md#finite-geometric-series). Since $M$ is odd, $r\mapsto-2r$ permutes the frequencies. Telescope the difference as

$$
\Lambda(a,a,a)-\Lambda(u,u,u)=\Lambda(f,a,a)+\Lambda(u,f,a)+\Lambda(u,u,f).
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and the displayed [Parseval identity on a finite group](../../../additive-combinatorics.md#parseval-identity-on-a-finite-group) bound each term by $\delta N\max_r|\widehat f(r)|$. Indeed, $\|a\|_2^2=\delta N$ and $\|u\|_2^2=\delta^2N$, so every product of the two remaining [L2 norms](../../../real-analysis.md#l2-norm) is at most $\delta N$. Hence

$$
\max_r|\widehat f(r)|\geq\frac{\delta^2N}{12}.
$$

The zero coefficient vanishes because $\sum f=0$, so choose a nonzero frequency $\theta=r/M$ giving this bound.

Let $Q=\lfloor\sqrt N\rfloor$. The [pigeonhole principle](../../../algebra.md#pigeonhole-principle) applied to the $Q+1$ fractional parts $0,\theta,\ldots,Q\theta$ in $Q$ intervals gives an [integer](../../../number-theory.md#integer) $1\leq q\leq Q$ with $\|q\theta\|_{\mathbb R/\mathbb Z}\leq1/Q$. Partition each [residue class](../../../number-theory.md#residue-class) modulo $q$ in $[N]$ into consecutive [arithmetic progressions](../../../arithmetic.md#arithmetic-progression) of exactly

$$
L=\left\lfloor\frac{\delta^2\sqrt N}{1000}\right\rfloor
$$

elements, leaving fewer than $L$ remainder points per residue. The total remainder $R_0$ has size at most $qL\leq\delta^2N/1000$. The size hypothesis gives $L\geq\delta^2\sqrt N/2000$. On a full [arithmetic progression](../../../arithmetic.md#arithmetic-progression) $P$, the phase $e^{-2\pi i\theta x}$ varies from its value at the first point by at most $2\pi L/Q\leq4\pi\delta^2/1000$.

Let $F_P=\sum_{x\in P}f(x)$. Replacing the phase by its first value on each full [arithmetic progression](../../../arithmetic.md#arithmetic-progression) and estimating the remainder using $|f|\leq1$ gives

$$
\sum_P|F_P|\geq\frac{\delta^2N}{12}-\frac{(4\pi+1)\delta^2N}{1000}>\frac{\delta^2N}{16}.
$$

Also $|\sum_PF_P|=|\sum_{R_0}f|\leq\delta^2N/1000$. Therefore the sum of the positive $F_P$ is

$$
\frac12\left(\sum_P|F_P|+\sum_PF_P\right)>\frac{\delta^2N}{64}.
$$

Since the total length of these [arithmetic progressions](../../../arithmetic.md#arithmetic-progression) is at most $N$, at least one has $F_P/|P|\geq\delta^2/64$. Thus the step just proved is

$$
\boxed{|P|\geq\frac{\delta^2\sqrt N}{2000},\qquad\frac{|A\cap P|}{|P|}\geq\delta+\frac{\delta^2}{64}.}
$$

An [affine map](../../../geometry-and-topology.md#affine-map) taking this [arithmetic progression](../../../arithmetic.md#arithmetic-progression) to $[|P|]$ preserves the absence of nonconstant three-term [arithmetic progressions](../../../arithmetic.md#arithmetic-progression).

Now iterate. Write $N_j,\delta_j$ for successive lengths and [subset densities](../../../additive-combinatorics.md#density-of-a-finite-subset), with $N_0=N$ and $\delta_0=\delta$. Since every [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) is at most one,

$$
\frac1{\delta_{j+1}}\leq\frac1{\delta_j}-\frac1{64+\delta_j}\leq\frac1{\delta_j}-\frac1{65}.
$$

Consequently $T=\lceil65/\delta\rceil$ successful steps are impossible. On the other hand, [subset densities](../../../additive-combinatorics.md#density-of-a-finite-subset) never decrease, so with $B=\log(2000/\delta^2)$,

$$
\log N_{j+1}\geq\frac12\log N_j-B,\qquad\log N_j\geq2^{-j}\log N-2B.
$$

Suppose $\delta\log\log N>100$. Since $T\leq66/\delta$,

$$
2^{-T}\log N>\exp\left(\frac{100-66\log2}{\delta}\right)>e^{54/\delta}.
$$

Let $D=\log(4\cdot10^6\delta^{-4})$. We have $2B+D<31+8\log(1/\delta)\leq39/\delta<e^{54/\delta}$. Therefore every length through step $T$ satisfies $\log N_j>D$, and hence $N_j\geq4\cdot10^6\delta^{-4}\geq4\cdot10^6\delta_j^{-4}$. The [density increment](../../../additive-combinatorics.md#density-increment) lemma remains applicable for all $T$ steps, contradicting the reciprocal-density bound.

Thus $\delta\log\log N\leq100$, proving the boxed theorem. The proof includes the [Fourier analysis on a finite abelian group](../../../additive-combinatorics.md#normalized-fourier-analysis-on-a-finite-abelian-group) detection, conversion to an [integer](../../../number-theory.md#integer) [arithmetic progression](../../../arithmetic.md#arithmetic-progression), and the length bookkeeping that produces the double logarithm.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

A [Freiman 2-isomorphism](../../../additive-combinatorics.md#freiman-2-isomorphism) is an [injective](../../../algebra.md#injective-function) map onto its image preserving pair-sum equality in both directions, with repeated summands allowed. Put $D=2A-2A$, so $D=-D$, $0\in D$, and $|D|<N$. We prove the [half-size cyclic Freiman model with a sharp difference-set bound](../../../additive-combinatorics.md#half-size-cyclic-freiman-model-with-a-sharp-difference-set-bound). Assume $A\ne\varnothing$; for an empty [set](../../../set.md) the conclusion is immediate.

Choose an odd auxiliary [prime](../../../number-theory.md#prime-number) $P>N$ large enough that reduction modulo $P$ is [injective](../../../algebra.md#injective-function) on $A$ and no nonzero element of $D$ reduces to zero. Choose a multiplier $t$ uniformly in $\mathbb Z_P^\times$. The forbidden residues are

$$
\mathcal F=\{jN\pmod P: j\in\mathbb Z,\ 0<|jN|<P\}.
$$

They form a symmetric [set](../../../set.md), exclude zero since $P>N$, and have [cardinality](../../../set-theory.md#cardinality) at most $2\lfloor(P-1)/N\rfloor$. For each nonzero $d\in D$, the product $td$ is uniform on the $P-1$ nonzero residues. Moreover, $td\in\mathcal F$ is the same event as $t(-d)\in\mathcal F$, so one need only sum over the $(|D|-1)/2$ opposite pairs. The [union bound](../../../probability-inequality.md#boole-s-inequality) gives

$$
\Pr\bigl(td\in\mathcal F\text{ for some }d\in D\setminus\{0\}\bigr)\leq\frac{|D|-1}{2}\frac{2\lfloor(P-1)/N\rfloor}{P-1}\leq\frac{|D|-1}{N}<1.
$$

Fix a multiplier avoiding all forbidden events. The use of opposite pairs is what achieves the threshold $N>|D|$ without an extra factor of two.

Represent each $ta\pmod P$ by an [integer](../../../number-theory.md#integer) $r(a)\in\{0,\ldots,P-1\}$. Partition these residues into the two half-intervals

$$
I_0=\{0,\ldots,(P-1)/2\},\qquad I_1=\{(P+1)/2,\ldots,P-1\}.
$$

At least half of $A$ has representatives in one of them; call this [subset](../../../set.md#subset) $A'$. Both intervals have diameter less than $P/2$, so for $a_1,a_2,a_3,a_4\in A'$ the [integer](../../../number-theory.md#integer)

$$
R=r(a_1)+r(a_2)-r(a_3)-r(a_4)
$$

satisfies $|R|<P$.

Define $\phi(a)=r(a)\pmod N$. If $a_1+a_2=a_3+a_4$, then $R\equiv0\pmod P$, hence $R=0$ and the image relation holds. Conversely, if the image relation holds, then $R=jN$. If the original difference $d=a_1+a_2-a_3-a_4$ were nonzero, $R\equiv td\pmod P$ would be nonzero; since $|R|<P$, this would be a forbidden residue in $\mathcal F$. Thus $d=0$.

Finally $\phi$ is [injective](../../../algebra.md#injective-function). If $\phi(a)=\phi(b)$, choose any $c\in A'$ and apply the converse to $\phi(a)+\phi(c)=\phi(b)+\phi(c)$, obtaining $a+c=b+c$. Therefore

$$
\boxed{|A'|\geq|A|/2,\qquad\phi:A'\longrightarrow\phi(A')\subseteq\mathbb Z_N\text{ is a Freiman 2-isomorphism}.}
$$

The construction actually works for any [integer](../../../number-theory.md#integer) $N>|D|$; the [prime](../../../number-theory.md#prime-number) hypothesis in the question is sufficient.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Fix $C$ and write $m=|A|$. Choose the permitted [prime](../../../number-theory.md#prime-number) $N$ with $Cm<N<2Cm$. Part (ii) gives a [subset](../../../set.md#subset) $A'$ of size at least $m/2$ and its [cyclic group](../../../group.md#cyclic-group) model $B\subseteq\mathbb Z_N$. Thus

$$
\frac{|B|}{N}>\frac1{4C}.
$$

To apply the interval form of [Roth theorem on three-term arithmetic progressions](../../../additive-combinatorics.md#roth-theorem-on-three-term-arithmetic-progressions), represent $B$ in $\{0,\ldots,N-1\}$ and split this interval into two consecutive intervals of length at most $\lceil N/2\rceil$. One has at least $|B|/2\geq m/4$ points. After translation, this is an [integer](../../../number-theory.md#integer) [subset](../../../set.md#subset) $B_0$ of an interval of length at most $Cm+1$ and [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) bounded below in terms of $C$ only. Pad the interval to length $L=\lceil N/2\rceil$ if necessary. If $B_0$ had no nonconstant three-term [arithmetic progression](../../../arithmetic.md#arithmetic-progression), part (i) would give

$$
\frac m4\leq|B_0|\leq\frac{C_0L}{\log\log L}\leq\frac{C_0(Cm+1)}{\log\log L}.
$$

Since $L\to\infty$ with $m$, this is impossible once $m$ is sufficiently large depending only on $C$.

Thus $B$ contains distinct elements $b_1,b_2,b_3$ with $b_1+b_3=2b_2$ modulo $N$. Their distinct preimages $a_1,a_2,a_3\in A'$ satisfy $a_1+a_3=2a_2$ in the [integers](../../../number-theory.md#integer) by the [Freiman 2-isomorphism](../../../additive-combinatorics.md#freiman-2-isomorphism). Reordering the endpoints if necessary gives

$$
\boxed{a_1,a_2,a_3\text{ form a nonconstant three-term arithmetic progression in }A.}
$$

The required size threshold depends on the fixed constant $C$; it is not a claim uniform in an arbitrarily growing $C$.

## 3

↑ **Parent:** [Paper 88](paper-88.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For disjoint nonempty [vertex](../../../graph.md#vertex-graph-theory) [sets](../../../set.md) $U,V$, write $d(U,V)=e(U,V)/(|U||V|)$. A [regular pair of vertex sets](../../../probabilistic-combinatorics.md#regular-pair-of-vertex-sets) is $\varepsilon$-regular if every $U'\subseteq U,V'\subseteq V$ with $|U'|\geq\varepsilon|U|$, $|V'|\geq\varepsilon|V|$ satisfies $|d(U',V')-d(U,V)|\leq\varepsilon$.

The [Szemerédi regularity lemma](../../../probabilistic-combinatorics.md#szemeredi-regularity-lemma) states that, for every $\varepsilon>0$ and [integer](../../../number-theory.md#integer) $m_0$, there are $M,n_0$ such that every finite simple [graph](../../../graph.md) on $n\geq n_0$ [vertices](../../../graph.md#vertex-graph-theory) has a [set partition](../../../combinatorics.md#set-partition)

$$
V=V_0\sqcup V_1\sqcup\cdots\sqcup V_m
$$

with **$m_0\leq m\leq M$, $|V_0|\leq\varepsilon n$, $|V_1|=\cdots=|V_m|$, and at most $\varepsilon m^2$ irregular unordered pairs among the nonexceptional classes**. Prove it for $0<\varepsilon\leq1/2$; larger parameters follow by using a smaller one.

For the [energy-increment proof of Szemerédi regularity](../../../probabilistic-combinatorics.md#energy-increment-proof-of-szemeredi-regularity), keep every exceptional [vertex](../../../graph.md#vertex-graph-theory) as a singleton cell in the [set partition](../../../combinatorics.md#set-partition) used to measure [regularity energy](../../../probabilistic-combinatorics.md#equitable-regularity-energy). Define the [equitable regularity energy](../../../probabilistic-combinatorics.md#equitable-regularity-energy)

$$
q(\mathcal P)=\frac1{n^2}\sum_{U,V\in\mathcal P}|U||V|d(U,V)^2.
$$

The sum is ordered, and on diagonal cells [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) means the average of the adjacency indicator, with zero on loops. Thus $0\leq q\leq1$. If $U,V$ are refined into $U_a,V_b$, expanding squares gives

$$
\sum_{a,b}|U_a||V_b|d(U_a,V_b)^2-|U||V|d(U,V)^2=\sum_{a,b}|U_a||V_b|[d(U_a,V_b)-d(U,V)]^2\geq0.
$$

The cross term vanishes because the weighted [arithmetic mean](../../../arithmetic.md#arithmetic-mean) of the refined [subset densities](../../../additive-combinatorics.md#density-of-a-finite-subset) is the original [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset). Consequently every [refinement of a set partition](../../../combinatorics.md#refinement-of-a-set-partition) increases or preserves [regularity energy](../../../probabilistic-combinatorics.md#equitable-regularity-energy).

Suppose the current nonexceptional classes have common size $t$ and there are $k$ of them. For each [irregular pair](../../../probabilistic-combinatorics.md#irregular-pair-of-vertex-sets) $V_i,V_j$, choose witnesses $A_{ij},B_{ij}$ of sizes at least $\varepsilon t$ and discrepancy greater than $\varepsilon$. Refine each class by all its incident witness [subsets](../../../set.md#subset). There are at most $k-1$ cuts in each class and at most $2^k$ resulting atoms. The witness rectangle is a union of refined rectangles. By the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), its contribution to the [variance](../../../variance.md) identity is at least

$$
|A_{ij}||B_{ij}|[d(A_{ij},B_{ij})-d(V_i,V_j)]^2>\varepsilon^4t^2.
$$

Indeed, the sum of squared deviations on the witness rectangle is at least its total weight times the square of their weighted [arithmetic mean](../../../arithmetic.md#arithmetic-mean). If more than $\varepsilon k^2$ unordered pairs are irregular, summing even just one orientation of each gives

$$
\Delta q>\varepsilon^5\frac{k^2t^2}{n^2}\geq\frac{\varepsilon^5}{4},
$$

provided the exceptional [set](../../../set.md) has at most $n/2$ [vertices](../../../graph.md#vertex-graph-theory). This is the strictly positive [regularity energy](../../../probabilistic-combinatorics.md#equitable-regularity-energy) increment.

Restore equal class sizes without losing that increment. Divide every witness atom into blocks of size $\ell=\lfloor t/4^k\rfloor$ and make every leftover [vertex](../../../graph.md#vertex-graph-theory) an exceptional singleton. This is a further [refinement of a set partition](../../../combinatorics.md#refinement-of-a-set-partition), so it cannot decrease $q$. There are at most $k2^k$ atoms, hence fewer than $k2^k\ell\leq n2^{-k}$ newly exceptional [vertices](../../../graph.md#vertex-graph-theory). If $t\geq2\cdot4^k$, then $\ell\geq t/(2\cdot4^k)$, so the number of full blocks is at most $2k4^k$. Each original class produces at least one full block: its leftovers occupy less than $2^k\ell$, whereas $t\geq4^k\ell>2^k\ell$. Thus the new class count is at least $k$.

Choose $R_* =\lceil4\varepsilon^{-5}\rceil+1$, and choose an initial [integer](../../../number-theory.md#integer) $k_0\geq m_0$ large enough that $R_*2^{-k_0}\leq\varepsilon/2$. Initially partition into $k_0$ equal classes and fewer than $k_0$ exceptional [vertices](../../../graph.md#vertex-graph-theory). Take $n_0$ large enough that this initial exception is at most $\varepsilon n/2$. During at most $R_*$ rounds, the additional exception is at most $R_*n2^{-k_0}\leq\varepsilon n/2$, so it never exceeds $\varepsilon n\leq n/2$.

A bound on class counts is obtained by iterating $k\mapsto2k4^k$ at most $R_*$ times starting at $k_0$; call the resulting bound $M$. Increasing $n_0$ further to satisfy $n_0\geq4M4^M$ guarantees $t\geq n/(2k)\geq2\cdot4^k$ at every round, so all full-block constructions are valid. If the desired regularity had not been reached after $R_*$ refinements, the [regularity energy](../../../probabilistic-combinatorics.md#equitable-regularity-energy) increments would total more than one, impossible. Therefore the process terminates with the required partition and bounds. The singleton treatment of discarded [vertices](../../../graph.md#vertex-graph-theory) is what preserves [regularity energy](../../../probabilistic-combinatorics.md#equitable-regularity-energy) monotonicity during equalization.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

First derive the [triangle removal lemma](../../../probabilistic-combinatorics.md#triangle-removal-lemma) from the [Szemerédi regularity lemma](../../../probabilistic-combinatorics.md#szemeredi-regularity-lemma). Given an allowed deletion fraction $0<\eta<1$, take $d=\eta/10$, $m_0=\lceil10/\eta\rceil$, and $0<\varepsilon\leq\min(d/4,\eta/100,1/8)$. Apply part (i), with upper class bound $M$. Delete [edges](../../../graph-theory.md#edge-of-a-graph) incident with $V_0$, inside each nonexceptional class, between [irregular pairs](../../../probabilistic-combinatorics.md#irregular-pair-of-vertex-sets), and between [regular pairs](../../../probabilistic-combinatorics.md#regular-pair-of-vertex-sets) of [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) less than $d$. Their total number is at most

$$
\left(2\varepsilon+\frac1{2m_0}+\frac d2\right)n^2<\eta n^2.
$$

These four terms are bounded respectively by $\varepsilon n^2$, $n^2/(2m_0)$, $\varepsilon n^2$, and $dn^2/2$.

If a [triangle in a graph](../../../graph.md#triangle-in-a-graph) remains, its three [vertices](../../../graph.md#vertex-graph-theory) lie in three distinct equal classes, all three [regular pairs](../../../probabilistic-combinatorics.md#regular-pair-of-vertex-sets) with [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) at least $d$. The permitted [regular triangle counting lemma](../../../probabilistic-combinatorics.md#regular-triangle-counting-lemma) gives at least $(d^3/4)t^3$ [triangles in a graph](../../../graph.md#triangle-in-a-graph) in the original [graph](../../../graph.md), where $t$ is the class size. This lower bound can also be checked directly: all but $2\varepsilon t$ [vertices](../../../graph.md#vertex-graph-theory) of the first class have at least $(d-\varepsilon)t$ neighbors in each of the other two. Those neighborhoods are large enough to use the [regular pair](../../../probabilistic-combinatorics.md#regular-pair-of-vertex-sets) condition on the remaining pair, giving at least $(d-\varepsilon)^3t^2$ [edges](../../../graph-theory.md#edge-of-a-graph) between them. Hence the total is at least $(1-2\varepsilon)(d-\varepsilon)^3t^3\geq(d^3/4)t^3$.

Since $t\geq n/(2M)$, a surviving [triangle in a graph](../../../graph.md#triangle-in-a-graph) forces at least $d^3n^3/(32M^3)$ original [triangles in a graph](../../../graph.md#triangle-in-a-graph). Thus a [graph](../../../graph.md) with fewer than $\xi n^3$ [triangles in a graph](../../../graph.md#triangle-in-a-graph), where $\xi=d^3/(64M^3)>0$, can be made [triangle-free](../../../graph.md#triangle-free-graph) by deleting fewer than $\eta n^2$ [edges](../../../graph-theory.md#edge-of-a-graph), for all sufficiently large $n$. This proves the removal lemma needed here.

Now use the [triangle-removal proof of Roth theorem](../../../additive-combinatorics.md#triangle-removal-proof-of-roth-theorem). Fix a [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) lower bound $\delta>0$ and suppose $A\subseteq[N]$, $|A|\geq\delta N$, has no nonconstant three-term [arithmetic progression](../../../arithmetic.md#arithmetic-progression). Set $m=2N+1$ and $G=\mathbb Z_m$. Use three disjoint copies $X,Y,Z$ of $G$ and put [edges](../../../graph-theory.md#edge-of-a-graph) according to

$$
xy\in E\iff y-x\in A,\qquad yz\in E\iff z-y\in A,\qquad xz\in E\iff (z-x)/2\in A.
$$

Division by two is valid because $m$ is odd. A [triangle in a graph](../../../graph.md#triangle-in-a-graph) corresponds to $a=y-x$, $b=z-y$, $c=(z-x)/2$ with $a,b,c\in A$ and $a+b=2c$. Since $A\subseteq[N]$ and $|a+b-2c|<m$, this congruence is an [integer](../../../number-theory.md#integer) equality. Progression-freeness therefore forces $a=b=c$.

Every [triangle in a graph](../../../graph.md#triangle-in-a-graph) is consequently of the form $(x,x+a,x+2a)$ with $x\in G,a\in A$, so there are exactly $m|A|$ [triangles in a graph](../../../graph.md#triangle-in-a-graph). These [triangles in a graph](../../../graph.md#triangle-in-a-graph) are edge-disjoint: an $XY$ [edge](../../../graph-theory.md#edge-of-a-graph) determines $(x,a)$; a $YZ$ [edge](../../../graph-theory.md#edge-of-a-graph) determines $a$ and then $x$; and an $XZ$ [edge](../../../graph-theory.md#edge-of-a-graph) determines $a=(z-x)/2$ and $x$. Eliminating them all requires at least $m|A|$ [edge](../../../graph-theory.md#edge-of-a-graph) deletions.

The [graph](../../../graph.md) has $3m$ [vertices](../../../graph.md#vertex-graph-theory) but only $m|A|\leq mN=O(m^2)$ [triangles in a graph](../../../graph.md#triangle-in-a-graph). Take $\eta=\delta/100$. For large enough $N$ its [triangle in a graph](../../../graph.md#triangle-in-a-graph) count is below $\xi(3m)^3$, so removal requires fewer than $\eta(3m)^2=9\delta m^2/100$ deletions. Yet

$$
m|A|\geq\delta mN\geq\frac{\delta m^2}{3}>\frac{9\delta m^2}{100},
$$

a contradiction. Therefore **every fixed positive-density [subset](../../../set.md#subset) of a sufficiently long interval contains a nonconstant three-term [arithmetic progression](../../../arithmetic.md#arithmetic-progression)**.

This proves the qualitative [Roth theorem on three-term arithmetic progressions](../../../additive-combinatorics.md#roth-theorem-on-three-term-arithmetic-progressions). The quantitative bound from part 2(i) came from the explicit Fourier iteration; the regularity-removal argument gives a density-dependent threshold without that double-logarithmic estimate.

## 4

↑ **Parent:** [Paper 88](paper-88.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Use [octahedral quasirandomness of a three-uniform hypergraph](../../../hypergraph.md#octahedral-quasirandomness-of-a-three-uniform-hypergraph), with its eighth-power normalization. Let $h:X\times Y\times Z\to\{0,1\}$ be the [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) [indicator function](../../../measure-theory.md#indicator-function), define $p=\mathbb E_{x,y,z}h(x,y,z)$, and put $g=h-p$. All [expectations](../../../probability-theory.md#expected-value) are uniform and independent on the indicated [finite sets](../../../set.md#finite-set). The [hypergraph](../../../hypergraph.md) is **$\alpha$-quasirandom** when

$$
\boxed{\|g\|_{\square^3}^8=\mathbb E_{x_0,x_1,y_0,y_1,z_0,z_1}\prod_{i,j,k\in\{0,1\}}g(x_i,y_j,z_k)\leq\alpha.}
$$

The eight triples form the faces of the tripartite octahedral configuration. Repeated choices within a part are included in this normalized average. For real $g$, the expression is nonnegative, since it equals

$$
\mathbb E_{x_0,x_1,y_0,y_1}\left(\mathbb E_z\prod_{i,j\in\{0,1\}}g(x_i,y_j,z)\right)^2.
$$

Thus the condition says that the balanced [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) [indicator function](../../../measure-theory.md#indicator-function) has [three-dimensional box norm](../../../additive-combinatorics.md#three-dimensional-box-norm) at most $\alpha^{1/8}$. If the [norm](../../../functional-analysis.md#norm) itself is used as the quasirandomness parameter instead, the eighth-power parameter here is the eighth power of that parameter; stating this convention fixes the quantitative meaning of the counting error.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

First prove the [pair-factor correlation bound for the three-dimensional box norm](../../../additive-combinatorics.md#pair-factor-correlation-bound-for-the-three-dimensional-box-norm). For real $g$ and three [functions](../../../function.md) $a(y,z),b(x,z),c(x,y)$ bounded in absolute value by one, let

$$
T=\mathbb E_{x,y,z}g(x,y,z)a(y,z)b(x,z)c(x,y).
$$

Apply the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) in $(y,z)$, placing the $x$ average inside and removing $a$. This gives

$$
|T|^2\leq\mathbb E_{y,z}\left|\mathbb E_xg(x,y,z)b(x,z)c(x,y)\right|^2.
$$

Expand this square, with independent $x_0,x_1$. Apply Cauchy-Schwarz in $(x_0,x_1,z)$, removing the product $b(x_0,z)b(x_1,z)$. The result is

$$
|T|^4\leq\mathbb E_{x_0,x_1,z}\left|\mathbb E_y g(x_0,y,z)g(x_1,y,z)c(x_0,y)c(x_1,y)\right|^2.
$$

Expand with independent $y_0,y_1$ and apply Cauchy-Schwarz in $(x_0,x_1,y_0,y_1)$, removing the four $c$ factors. Then

$$
|T|^8\leq\mathbb E_{x_0,x_1,y_0,y_1}\left|\mathbb E_z\prod_{i,j\in\{0,1\}}g(x_i,y_j,z)\right|^2=\|g\|_{\square^3}^8.
$$

Therefore **$|T|\leq\|g\|_{\square^3}$**, with no independence assumption on the three pair [functions](../../../function.md).

In this [multipartite hypergraph](../../../hypergraph.md#multipartite-hypergraph), a simplex is a [three-uniform tetrahedron](../../../hypergraph.md#three-uniform-tetrahedron): one [vertex of a hypergraph](../../../hypergraph.md#vertex-of-a-hypergraph) from each of $X,Y,Z,W$, with all four possible triples present. Write the corresponding [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) [indicator functions](../../../measure-theory.md#indicator-function) as $h_1(x,y,z),h_2(x,y,w),h_3(x,z,w),h_4(y,z,w)$, of [subset densities](../../../additive-combinatorics.md#density-of-a-finite-subset) $p,q,r,s$. Its normalized count is

$$
t=\mathbb E_{x,y,z,w}h_1h_2h_3h_4.
$$

Telescope the product exactly:

$$
h_1h_2h_3h_4-pqrs=(h_1-p)h_2h_3h_4+p(h_2-q)h_3h_4+pq(h_3-r)h_4+pqr(h_4-s).
$$

For the first term fix $w$. The remaining three factors are bounded pair [functions](../../../function.md) of $(x,y)$, $(x,z)$ and $(y,z)$, so the inequality just proved bounds its $(x,y,z)$ average by $\|h_1-p\|_{\square^3}\leq\alpha^{1/8}$. Averaging over $w$ preserves that bound. For each other term fix the [vertex of a hypergraph](../../../hypergraph.md#vertex-of-a-hypergraph) outside its balanced triple and apply the same argument, allowing an unused pair factor to be identically one. The [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) prefactors are at most one. Hence

$$
\boxed{|t-pqrs|\leq4\alpha^{1/8}.}
$$

Multiplying by $|X||Y||Z||W|$ gives

$$
\boxed{|\#\text{simplices}-pqrs|X||Y||Z||W||\leq4\alpha^{1/8}|X||Y||Z||W|.}
$$

Thus one may take the absolute constant $C=4$. This proves the complete-pair-support case of the [tetrahedron counting lemma](../../../hypergraph.md#tetrahedron-counting-lemma) directly; no lower bound on $p,q,r,s$ is needed.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Yes. The same telescoping argument proves the [counting lemma for octahedrally quasirandom three-uniform hypergraphs](../../../hypergraph.md#counting-lemma-for-octahedrally-quasirandom-three-uniform-hypergraphs) for every fixed simple three-uniform [hypergraph](../../../hypergraph.md) $F$.

Label its [vertices of a hypergraph](../../../hypergraph.md#vertex-of-a-hypergraph) $1,\ldots,v$ and give [vertex of a hypergraph](../../../hypergraph.md#vertex-of-a-hypergraph) $i$ a nonempty host part $V_i$. For each [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) $e=\{i,j,k\}$, let $h_e$ be the corresponding host [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) [indicator function](../../../measure-theory.md#indicator-function) of [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) $p_e$, with $\|h_e-p_e\|_{\square^3}\leq\alpha^{1/8}$. The normalized [labelled hypergraph copy count](../../../hypergraph.md#labelled-hypergraph-copy-count) is

$$
t_F=\mathbb E_{x_1\in V_1,\ldots,x_v\in V_v}\prod_{e\in E(F)}h_e(x_e).
$$

If the host parts are disjoint, every such [vertex of a hypergraph](../../../hypergraph.md#vertex-of-a-hypergraph) choice is automatically [injective](../../../algebra.md#injective-function). Enumerate the $m$ [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph) as $e_1,\ldots,e_m$ and telescope

$$
\prod_{j=1}^mh_{e_j}-\prod_{j=1}^mp_{e_j}=\sum_{j=1}^m\left(\prod_{i<j}p_{e_i}\right)(h_{e_j}-p_{e_j})\left(\prod_{i>j}h_{e_i}\right).
$$

In the term for $e_j=\{a,b,c\}$, fix all variables outside this triple. Since $F$ is simple and three-uniform, every other [hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) intersects $\{a,b,c\}$ in at most two [vertices of a hypergraph](../../../hypergraph.md#vertex-of-a-hypergraph). Its remaining factor therefore depends on at most two of $x_a,x_b,x_c$. Group all two-variable factors according to the pairs $(a,b),(a,c),(b,c)$. Absorb each one-variable factor into any pair containing its variable, and constants into any group. The three resulting pair [functions](../../../function.md) remain bounded by one.

The balanced factor is now multiplied by exactly the sort of pair [functions](../../../function.md) handled in part (ii). Its average has absolute value at most $\alpha^{1/8}$, independently of the fixed outside variables. Averaging those variables and summing the $m$ errors gives

$$
\boxed{|t_F-\prod_{e\in E(F)}p_e|\leq m\alpha^{1/8}.}
$$

Equivalently,

$$
\boxed{\left|\#F-\left(\prod_ep_e\right)\left(\prod_{i=1}^v|V_i|\right)\right|\leq |E(F)|\alpha^{1/8}\prod_{i=1}^v|V_i|.}
$$

This counts labelled copies preserving the specified [vertex of a hypergraph](../../../hypergraph.md#vertex-of-a-hypergraph) classes, for arbitrary intersection patterns among the [hypergraph edges](../../../hypergraph.md#edge-of-a-hypergraph), and includes the [three-uniform tetrahedron](../../../hypergraph.md#three-uniform-tetrahedron) as a special case.

For a common host [vertex of a hypergraph](../../../hypergraph.md#vertex-of-a-hypergraph) [set](../../../set.md) of size $n$, the same product average counts homomorphisms. At most $\binom v2n^{v-1}$ assignments identify a pair of distinct labelled [vertices of a hypergraph](../../../hypergraph.md#vertex-of-a-hypergraph), by the [union bound](../../../probability-inequality.md#boole-s-inequality). Thus restricting to [injective](../../../algebra.md#injective-function) copies changes the estimate by at most this amount. With a common normalized [subset density](../../../additive-combinatorics.md#density-of-a-finite-subset) $p$ the [injective](../../../algebra.md#injective-function) count is therefore $p^mn^v+O(m\alpha^{1/8}n^v+v^2n^{v-1})$. For induced copies, include the non[hypergraph edge](../../../hypergraph.md#edge-of-a-hypergraph) [indicator functions](../../../measure-theory.md#indicator-function) as additional factors; their balanced [functions](../../../function.md) are negatives of the corresponding edge-balanced [functions](../../../function.md) and have the same box [norm](../../../functional-analysis.md#norm). The same proof applies provided all the relevant triple parts satisfy the stated quasirandomness condition.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
