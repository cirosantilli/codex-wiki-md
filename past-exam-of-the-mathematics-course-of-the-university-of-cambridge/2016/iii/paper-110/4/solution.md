<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume the [uniform hypergraph](../../../../../uniform-hypergraph.md) has positive average [hypergraph vertex degree](../../../../../hypergraph-vertex-degree.md) $d$, so $nd=r e(G)$. Its [hypergraph degree measure](../../../../../hypergraph-degree-measure.md) is

$$
\boxed{\mu(S)=\frac1{nd}\sum_{u\in S}d_G(u).}
$$

It is a [probability measure](../../../../../probability-measure.md) on the vertex set; vertices of degree zero have measure zero. If the [hypergraph](../../../../../hypergraph-split.md) is regular, it equals $|S|/n$. An edgeless [hypergraph](../../../../../hypergraph-split.md) has no normalized degree measure of this form and must be treated separately.

Every edge entirely in $S$ contributes $r$ to the degree sum over $S$, giving the upper bound. For the lower bound, an edge entirely in $S$ contributes $r$, and any other edge contributes at most $r-1$. Therefore

$$
nd\mu(S)\le r e(G[S])+(r-1)(e(G)-e(G[S]))
=e(G[S])+\frac{r-1}{r}nd.
$$

Together these give **both degree-measure inequalities**:

$$
\boxed{\left(\mu(S)-1+\frac1r\right)nd\le e(G[S])\le\frac{\mu(S)nd}{r}.}
$$

In particular every [hypergraph independent set](../../../../../hypergraph-independent-set.md) has measure at most $1-1/r$, which explains why degree measure can control containers even in very nonregular [hypergraphs](../../../../../hypergraph-split.md).

**A sufficient container theorem.** For every fixed $r\ge2$, there are positive constants $\delta_r,\tau_r,c_r,K_r$ such that if $0<\tau\le\tau_r$ and

$$
d_G(\sigma)\le\delta_r d\tau^{|\sigma|-1}\quad(2\le|\sigma|\le r),
$$

there is a family of [hypergraph containers](../../../../../hypergraph-container.md) covering all [hypergraph independent sets](../../../../../hypergraph-independent-set.md), each with $\mu(C)\le1-c_r$. Each container is determined by a [container fingerprint](../../../../../container-fingerprint.md) $T$ with $|T|\le K_r\tau n$ and $\mu(T)\le K_r\tau$. In particular, for sufficiently small $\tau$, the number of containers is at most $\exp(O_r(\tau n\log(1/\tau)))$. We will give an algorithm and constants establishing this version.

The [golden rule for container algorithms](../../../../../golden-rule-for-container-algorithms.md) is that reconstruction may depend on the small [container fingerprint](../../../../../container-fingerprint.md), but never on unrevealed information about the independent set. When a deterministic test calls for inspecting a vertex, a positive membership answer is recorded in the [container fingerprint](../../../../../container-fingerprint.md), while a negative answer permits its exclusion from the container. All tests and all state updates must be reproducible using that [container fingerprint](../../../../../container-fingerprint.md). Choosing tests that permit only a few positive answers then yields few containers.

**Here is an explicit implementation with controlled links.** Use the fixed order $1,\ldots,n$, parameters $\tau,\delta,\zeta>0$, and a bound $d_G(\sigma)\le\delta d\tau^{|\sigma|-1}$ on nonsingleton [codegrees](../../../../../hypergraph-codegree.md). Let $d_s(\sigma)$ count incidences with multiplicity in the $s$-uniform [multihypergraph](../../../../../multihypergraph.md) $P_s$. Define thresholds

$$
\theta_s(\{u\})=\tau^{r-s}d_G(u),\qquad
\theta_s(\sigma)=\delta d\tau^{r-s+|\sigma|-1}\quad(|\sigma|\ge2).
$$

A saturated subset is one whose current degree has reached its threshold.

1. Put $P_r=E(G)$; start $P_s$ and their saturation families $\Gamma_s$ empty for $1\le s<r$. Put $B=\{u:d_G(u)<\zeta d\}$, $T=\varnothing$, and $C=[n]$.
1. At the current vertex $v$, for every $1\le s<r$ compute the [multiset](../../../../../multiset.md)$$
   F_{v,s}=\{f\subseteq\{v+1,\ldots,n\}:|f|=s,\ \{v\}\cup f\in P_{s+1},\ \nexists\sigma\in\Gamma_s\text{ with }\sigma\subseteq f\}.
   $$

   Retain the multiplicity from $P_{s+1}$. Compute all these [multisets](../../../../../multiset.md) before modifying any $P_s$ at this vertex.
1. Inspect $v$ if $v\notin B$ and either $v\in\Gamma_1$ or $|F_{v,s}|\ge\zeta\tau^{r-s-1}d_G(v)$ for some $s$. If it is not inspected, leave $v$ in $C$ and continue.
1. On inspection, if $v\notin I$, remove it from $C$. If $v\in I$, put it in $T$ and retain it in $C$.
1. For a vertex put in $T$, add the full [multiset](../../../../../multiset.md) $F_{v,s}$ to $P_s$ for every $s$. Then insert into $\Gamma_s$ every nonempty future subset $\sigma$ with $|\sigma|\le s$ and $d_s(\sigma)\ge\theta_s(\sigma)$. Once saturated, a subset stays in $\Gamma_s$.
1. Advance to the next vertex. To reconstruct $C$ from $T$, use exactly the same state evolution, replacing the inspected membership test $v\in I$ by $v\in T$.

Every generated edge of $P_s$ extends to an original edge by adding $r-s$ earlier vertices from $T$. Thus, for a [hypergraph independent set](../../../../../hypergraph-independent-set.md) $I$, no singleton generated in $P_1$ can be a member of $I$. In particular an inspected vertex in $\Gamma_1$ cannot give a positive membership answer. All other positive answers are recorded. The [golden rule for container algorithms](../../../../../golden-rule-for-container-algorithms.md) now proves that the reconstructed container contains $I$ and that its state depends only on $T$.

**Control the possible overshoot at saturation.** The [multisets](../../../../../multiset.md) are added in batches; merely claiming $d_s(\sigma)\le\theta_s(\sigma)$ would be wrong. In the last batch that increases $d_s(\sigma)$, the set $\sigma$ was not yet saturated, and the batch comes from some vertex $v\notin\sigma$. Its contribution is at most $d_{s+1}(\sigma\cup\{v\})$. Hence

$$
d_s(\sigma)\le\theta_s(\sigma)+d_{s+1}(\sigma\cup\{v\}).
$$

Induction downwards from $P_r$ yields, for $|\sigma|\ge2$,

$$
d_s(\sigma)\le(r-s+1)\delta d\tau^{r-s+|\sigma|-1}.
$$

Indeed the two terms in the last-batch bound have coefficients $1$ and $r-s$ with the same power of $\tau$. Applying this nonsingleton bound to $\{u,v\}$ gives the singleton estimate

$$
d_s(u)\le\tau^{r-s}\bigl(d_G(u)+(r-s)\delta d\bigr)
\le\tau^{r-s}\bigl(d_G(u)+r\delta d\bigr).
$$

Summing over $U$, using $|U|\le n$, proves **the requested estimate at every stage of the algorithm**:

$$
\boxed{\sum_{u\in U}d_s(u)\le\tau^{r-s}nd\bigl(\mu(U)+r\delta\bigr).}
$$

It applies with multiplicities; replacing the [multisets](../../../../../multiset.md) by sets in the accounting would invalidate the argument.

**Check that the [container fingerprint](../../../../../container-fingerprint.md) is small and the container loses positive measure.** Assign each positive inspected vertex to one index $s$ witnessing its test. Its added link batch has size at least $\zeta\tau^{r-s-1}d_G(v)$. Distinct batches count separately in the [multiset](../../../../../multiset.md). Since $|P_s|=s^{-1}\sum_u d_s(u)$, the preceding bound gives

$$
\mu(T)\le\frac{r\tau}{\zeta}(1+r\delta),\qquad
|T|\le\frac{rn\tau}{\zeta^2}(1+r\delta).
$$

The second inequality uses $d_G(v)\ge\zeta d$ for every $v\in T$.

For completeness, the loss of measure can be verified by a short incidence count. Put $D=([n]\setminus C)\cup T\cup B$ and $a_s=|P_s|/(\tau^{r-s}nd)$. Every saturated singleton belongs to $D$. Partition $P_{s+1}$ by its earliest vertex. An earliest vertex in $D$ accounts for at most $\tau^{r-s-1}nd(\mu(D)+r\delta)$ incidences. For any other earliest vertex, the unsaturated link has size less than $\zeta\tau^{r-s-1}d_G(v)$; the remaining edges meet some saturated subset of $\Gamma_s$.

For a saturated nonsingleton $\sigma$, the degree bounds imply $d_{s+1}(\sigma)\le(r/\tau)d_s(\sigma)$. For a saturated singleton the corresponding bound is $d_{s+1}(u)\le\tau^{-1}d_s(u)+r\delta d\tau^{r-s-1}$. Every multiedge of $P_s$ has fewer than $2^s$ nonempty subsets. These observations give

$$
a_{s+1}\le r2^s a_s+\mu(D)+\zeta+2r\delta\quad(2\le s<r).
$$

For $s=1$, all saturated subsets are singletons in $D$, so directly summing their $P_2$ degrees gives

$$
a_2\le2\mu(D)+\zeta+3r\delta.
$$

Since $a_r=1/r$, these inequalities prevent $D$ from having arbitrarily small measure. To make the constants explicit, let

$$
A=r2^r,\quad L=3A^{r-2},\quad b=\frac1{rL},\quad
\zeta=\frac b8,\quad\delta_r=\frac{b}{24r},\quad
\tau_r=\frac{b\zeta}{16r},\quad c_r=\frac b2.
$$

Iterating the displayed inequalities gives $a_r\le L(\mu(D)+\zeta+3r\delta)$, hence $\mu(D)\ge3b/4$ whenever $\delta\le\delta_r$. Also $r\delta\le1$, so $\tau\le\tau_r$ gives $\mu(T)\le2r\tau/\zeta\le b/8$, while $\mu(B)\le\zeta=b/8$. Therefore

$$
\boxed{\mu(C)\le1-\mu(D)+\mu(T)+\mu(B)\le1-b/2=1-c_r.}
$$

One can take $K_r=2r/\zeta^2$ in the stated [container fingerprint](../../../../../container-fingerprint.md) bounds. Counting subsets of size at most $K_r\tau n$ gives the asserted bound on the number of containers. Thus the explicit algorithm produces the family promised by the sufficient [hypergraph container theorem](../../../../../hypergraph-container-theorem.md), as well as the required intermediate degree estimate.

For the standard weak-threshold formulation, see [Online containers for hypergraphs](https://arxiv.org/html/1611.01433). The constants above come from the explicit incidence estimates given here.

For $r=1$, no multilevel construction is needed: take the sole container to be the vertices that are not singleton edges. It contains every [hypergraph independent set](../../../../../hypergraph-independent-set.md) and has degree measure zero when $d>0$; its fingerprint is empty. The requested degree-sum inequality follows directly from the definition of $\mu$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 110](../../paper-110-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
