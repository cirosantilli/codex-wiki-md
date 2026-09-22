<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $G$ be a finite undirected $d$-regular [graph](../../../../../graph-split.md) on $N$ [vertices](../../../../../vertex-graph-theory.md), with [adjacency matrix](../../../../../adjacency-matrix.md) $A$ and normalized [random walk](../../../../../random-walk.md) matrix $P=A/d$. Define [edge](../../../../../edge-of-a-graph.md) expansion and normalized conductance by

$$
h(G)=\min_{0<|S|\leq N/2}\frac{e(S,S^c)}{|S|},\qquad \Phi(G)=h(G)/d.
$$

An [expander family](../../../../../expander-graph.md) has orders tending to infinity, uniformly bounded maximum degree, and a uniform positive lower bound on $h$. For a [regular graph](../../../../../regular-graph.md) the constant vector is an [eigenvector](../../../../../eigenvector.md) of $P$ with [eigenvalue](../../../../../eigenvalue.md) one. Write its [eigenvalues](../../../../../eigenvalue.md) as $1=\mu_1\geq\mu_2\geq\cdots\geq\mu_N\geq-1$, and let $\delta=1-\mu_2$. This [spectral gap](../../../../../spectral-gap.md) measures the energetic cost of departing from a constant function.

For every mean-zero vector $f$, the [spectral theorem](../../../../../spectral-theorem.md) and the [graph](../../../../../graph-split.md)'s energy identity give

$$
\frac1d\sum_{\{u,v\}\in E}(f(u)-f(v))^2
=\langle f,(I-P)f\rangle\geq\delta\|f\|_2^2.
$$

Apply this to $f=\mathbf1_S-|S|\mathbf1/N$. Its norm squared is $|S|(1-|S|/N)$ and its energy is $e(S,S^c)/d$. Therefore

$$
e(S,S^c)\geq d\delta |S|(1-|S|/N),\qquad
\boxed{\Phi(G)\geq\delta/2.}
$$

Thus a uniform [spectral gap](../../../../../spectral-gap.md) gives uniform [edge](../../../../../edge-of-a-graph.md) expansion when $d$ is fixed. This also bounds exterior [vertex](../../../../../vertex-graph-theory.md) expansion: each exterior [vertex](../../../../../vertex-graph-theory.md) accounts for at most $d$ boundary [edges](../../../../../edge-of-a-graph.md), so $|N(S)\setminus S|\geq e(S,S^c)/d$.

For the converse, take a mean-zero [eigenvector](../../../../../eigenvector.md) $f$ for $\mu_2$ and choose its sign so that its positive support has at most $N/2$ [vertices](../../../../../vertex-graph-theory.md). Put $g=f^+$, which is nonzero. Truncation decreases energy in the following precise sense: for any two real numbers $a,b$,

$$
(a^+-b^+)^2\leq(a^+-b^+)(a-b).
$$

Summing over [edges](../../../../../edge-of-a-graph.md) yields $\langle g,(I-P)g\rangle\leq\langle g,(I-P)f\rangle=\delta\|g\|_2^2$. For the threshold sets $S_t=\{v:g(v)^2>t\}$, every nonempty set lies in that small positive support. Integrating its boundary count gives the layer-cake identity

$$
\sum_{\{u,v\}\in E}|g(u)^2-g(v)^2|
=\int_0^\infty e(S_t,S_t^c)\,dt\geq h(G)\|g\|_2^2.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) bounds the left side by

$$
\left(\sum_E(g(u)-g(v))^2\right)^{1/2}
\left(\sum_E(g(u)+g(v))^2\right)^{1/2}
\leq d\sqrt{2\delta}\,\|g\|_2^2,
$$

because the first sum is at most $d\delta\|g\|_2^2$ and the second at most $2d\|g\|_2^2$. Cancelling proves the [Cheeger inequality](../../../../../cheeger-inequality.md) in both directions:

$$
\boxed{\frac{1-\mu_2}{2}\leq\Phi(G)\leq\sqrt{2(1-\mu_2)}.}
$$

Hence bounded-degree regular families have uniform [edge](../../../../../edge-of-a-graph.md) expansion exactly when their second-largest normalized [eigenvalue](../../../../../eigenvalue.md) stays uniformly below one.

Absolute [eigenvalues](../../../../../eigenvalue.md) give additional information. Put $\rho=\max_{i\geq2}|\mu_i|$. Centering the indicators of $S,T$ and applying the operator-norm bound on the mean-zero subspace proves the [expander mixing lemma](../../../../../expander-mixing-lemma.md):

$$
\left|e(S,T)-\frac{d|S||T|}{N}\right|
\leq d\rho\sqrt{|S|(1-|S|/N)|T|(1-|T|/N)}.
$$

Here $e(S,T)=\mathbf1_S^TA\mathbf1_T$, so internal [edges](../../../../../edge-of-a-graph.md) are counted as oriented incidences. A small $\rho$ makes [edge](../../../../../edge-of-a-graph.md) counts resemble uniformly distributed [edges](../../../../../edge-of-a-graph.md). It also gives rapid [random walk](../../../../../random-walk.md) mixing: starting at a [vertex](../../../../../vertex-graph-theory.md), $P^t$ contracts the mean-zero component of its point mass by at most $\rho^t$ in [Euclidean norm](../../../../../euclidean-norm.md); [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) then gives total variation distance at most $\tfrac12\sqrt N\rho^t$ from the uniform distribution. A [bipartite graph](../../../../../bipartite-graph.md) has [eigenvalue](../../../../../eigenvalue.md) $-1$ and its non-lazy walk alternates sides, even if it has good [edge](../../../../../edge-of-a-graph.md) expansion. The lazy walk $(I+P)/2$ has nonconstant [eigenvalues](../../../../../eigenvalue.md) between zero and $1-\delta/2$, resolving this periodicity. It is important to distinguish the gap $1-\mu_2$ controlling cuts from the absolute bound controlling non-lazy mixing.

Here is a fully specified deterministic construction of an infinite family. Its degree is large but fixed. Set

$$
d=2^{16},\qquad D=d^2=2^{32},\qquad W=\mathbb F_2^{64},\quad |W|=D^2.
$$

Choose the lexicographically first ordered list $a_1,\ldots,a_d\in W$ satisfying

$$
\left|\frac1d\sum_{j=1}^d(-1)^{u\cdot a_j}\right|\leq\frac1{10}\qquad\text{for every }u\in W\setminus\{0\}.
$$

This finite deterministic search terminates. To prove existence, choose the list uniformly and independently. For each nonzero $u$, its signs are independent unbiased signs; the exponential-moment estimate $\cosh t\leq e^{t^2/2}$ and [Markov inequality](../../../../../markov-inequality.md) give an exceptional [probability](../../../../../probability.md) at most $2e^{-d/200}$. A [union bound](../../../../../boole-s-inequality.md) gives total failure [probability](../../../../../probability.md) at most

$$
2(2^{64}-1)e^{-2^{16}/200}<1.
$$

Thus at least one qualifying list exists. Fix it once and for all.

Let $H$ be the [Cayley graph](../../../../../cayley-graph.md) on $W$ whose $j$th neighbor of $x$ is $x+a_j$. It is an undirected $d$-regular port-labeled [graph](../../../../../graph-split.md), allowing repeated [edges](../../../../../edge-of-a-graph.md) and loops in this intermediate construction. Its [characters](../../../../../character-of-a-representation.md) $x\mapsto(-1)^{u\cdot x}$ form an [orthogonal](../../../../../orthogonal-vectors.md) [eigenbasis](../../../../../eigenbasis.md), with the displayed averages as normalized [eigenvalues](../../../../../eigenvalue.md). Therefore $\rho(H)\leq1/10$. Each loop counts as one transition port; degrees here mean row sums of the [adjacency matrix](../../../../../adjacency-matrix.md).

We next define the [zig-zag product](../../../../../zig-zag-product.md) and prove the bound used for iteration. A port labeling of a $D_0$-regular undirected [graph](../../../../../graph-split.md) $F$ gives an involution $\operatorname{Rot}_F(v,a)=(w,b)$, recording the endpoint and reverse port. If a $d$-regular [graph](../../../../../graph-split.md) $H_0$ has [vertex](../../../../../vertex-graph-theory.md) set $[D_0]$, the product has [vertices](../../../../../vertex-graph-theory.md) $(v,a)\in V(F)\times[D_0]$. For each ordered pair of small-graph ports, move from $a$ to $a'$ in $H_0$, follow the big [edge](../../../../../edge-of-a-graph.md) $\operatorname{Rot}_F(v,a')=(w,b')$, and move from $b'$ to $b$ in $H_0$. The endpoint is $(w,b)$; reversing the steps reverses the two small-graph port labels. The product is undirected, has $|V(F)|D_0$ [vertices](../../../../../vertex-graph-theory.md), and has degree $d^2$.

Write $B=I\otimes P_{H_0}$ and let $R$ be the permutation matrix of $\operatorname{Rot}_F$. The normalized product operator is $BRB$. For a mean-zero unit vector, decompose $f=u+v$ into its cloud-constant part and its cloud-orthogonal part. Then $Bu=u$, $\|Bv\|\leq\rho(H_0)\|v\|$, and $\|R\|=1$. The compression of $R$ to cloud-constant vectors is exactly $P_F$, so $|\langle u,Ru\rangle|\leq\rho(F)\|u\|^2$. Expanding the quadratic form and applying [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
|\langle f,BRBf\rangle|
\leq\rho(F)\|u\|^2+2\rho(H_0)\|u\|\|v\|+\rho(H_0)^2\|v\|^2
\leq\rho(F)+2\rho(H_0)+\rho(H_0)^2.
$$

The operator is symmetric, so its mean-zero [operator norm](../../../../../operator-norm.md) is bounded by this same quantity. No unproved product spectral estimate is needed.

Start with the loop-inclusive [complete graph](../../../../../complete-graph.md) $G_0$ on $D$ [vertices](../../../../../vertex-graph-theory.md), whose normalized matrix is $J/D$ and whose nonconstant [eigenvalues](../../../../../eigenvalue.md) are all zero. Given a $D$-regular $G_t$, its two-step [graph](../../../../../graph-split.md) $G_t^2$ has degree $D^2$ and normalized operator $P_{G_t}^2$. Label a two-step [edge](../../../../../edge-of-a-graph.md) by its ordered pair of ports; reversal reverses the path and its reverse ports. These $D^2$ labels are the [vertex](../../../../../vertex-graph-theory.md) set of the fixed [graph](../../../../../graph-split.md) $H$. Define

$$
G_{t+1}=G_t^2\mathbin{\mathrm{zigzag}}H.
$$

It has degree $d^2=D$, and its number of [vertices](../../../../../vertex-graph-theory.md) is $N_{t+1}=N_tD^2$, hence $N_t=D^{2t+1}$. By the proved bound,

$$
\rho(G_{t+1})\leq\rho(G_t)^2+\frac{21}{100}.
$$

Starting from zero, induction gives $\rho(G_t)\leq1/2$, since $(1/2)^2+21/100=46/100<1/2$. The cut-energy argument therefore gives multiplicity-counted [edge](../../../../../edge-of-a-graph.md) expansion at least $D/4$ for every $G_t$.

To obtain ordinary simple [graphs](../../../../../graph-split.md), delete loops and merge parallel [edges](../../../../../edge-of-a-graph.md). The maximum degree is at most $D$, and any one unordered [vertex](../../../../../vertex-graph-theory.md) pair had multiplicity at most $D$. Thus every cut retains at least $1/D$ of its multiplicity-counted boundary, giving

$$
\boxed{|V(G_t)|=D^{2t+1}\longrightarrow\infty,\qquad \Delta\leq D,\qquad h\geq1/4.}
$$

These simple [graphs](../../../../../graph-split.md) form an [expander family](../../../../../expander-graph.md). Every choice is deterministic: the finite base search is fixed independently of $t$, and the recursive [edge](../../../../../edge-of-a-graph.md) rules determine all subsequent adjacency lists. Once that base is fixed, adjacency lists can be generated successively using the previous lists, with a constant amount of work per output [edge](../../../../../edge-of-a-graph.md). This is [squaring and zig-zag iteration yields bounded-degree expanders](../../../../../squaring-and-zig-zag-iteration-yields-bounded-degree-expanders.md). The spectral argument supplies the uniform expansion guarantee and explains why squaring improves the [eigenvalues](../../../../../eigenvalue.md) while the product restores a constant degree.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
