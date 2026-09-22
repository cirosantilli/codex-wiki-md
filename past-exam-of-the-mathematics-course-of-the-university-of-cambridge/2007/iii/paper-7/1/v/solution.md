<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Define the [lower central series](../../../../../../lower-central-series.md) by $\Gamma_1(G)=G$ and $\Gamma_{j+1}(G)=[\Gamma_j(G),G]$. Its terms are characteristic [normal subgroups](../../../../../../normal-subgroup.md) and form a descending chain. Define the [upper central series](../../../../../../upper-central-series.md) by $Z_0(G)=1$ and

$$
Z_{i+1}(G)/Z_i(G)=Z\big(G/Z_i(G)\big).
$$

Equivalently, $Z_{i+1}(G)=\{x\in G:[x,G]\subseteq Z_i(G)\}$. These are characteristic [normal subgroups](../../../../../../normal-subgroup.md) in an ascending chain, and successive factors are central in the appropriate quotient.

For any length-$r$ [central series](../../../../../../central-series.md) $1=G_0\le\cdots\le G_r=G$, prove the two comparisons independently. Starting at $\Gamma_1(G)=G_r$, if $\Gamma_{r-i+1}(G)\le G_i$, then

$$
\Gamma_{r-i+2}(G)=[\Gamma_{r-i+1}(G),G]\le[G_i,G]\le G_{i-1}.
$$

Descending induction gives the lower containment. Starting at $G_0=Z_0(G)=1$, if $G_{i-1}\le Z_{i-1}(G)$, then $[G_i,G]\le G_{i-1}\le Z_{i-1}(G)$, which by definition gives $G_i\le Z_i(G)$. Thus the [central-series comparison theorem](../../../../../../central-series-comparison-theorem.md) yields

$$
\boxed{\Gamma_{r-i+1}(G)\le G_i\le Z_i(G)\quad(0\le i\le r).}
$$

In particular, a [nilpotent group](../../../../../../nilpotent-group.md) satisfies $\Gamma_{r+1}(G)=1$ and $Z_r(G)=G$.

Conversely, if $\Gamma_n(G)=1$, reverse the finite lower chain to obtain $1=\Gamma_n\le\Gamma_{n-1}\le\cdots\le\Gamma_1=G$. The defining commutator recurrence makes it a [central series](../../../../../../central-series.md). If $Z_n(G)=G$, the finite upper chain is already a [central series](../../../../../../central-series.md). This proves

$$
\boxed{G\text{ nilpotent}\ \Longleftrightarrow\ \Gamma_n(G)=1\text{ for some }n\ \Longleftrightarrow\ Z_n(G)=G\text{ for some }n.}
$$

Finally, for an integer $c>0$, termination at $\Gamma_{c+1}=1$ gives a [central series](../../../../../../central-series.md) of length $c$ and hence $Z_c=G$ by the comparison. Conversely, $Z_c=G$ gives a [central series](../../../../../../central-series.md) of length $c$ and hence $\Gamma_{c+1}=1$. Therefore

$$
\boxed{\Gamma_{c+1}(G)=1\quad\Longleftrightarrow\quad Z_c(G)=G.}
$$

Repeated terms cause no problem; the least such $c$ for a nontrivial group is its [nilpotency class](../../../../../../nilpotency-class.md).

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
