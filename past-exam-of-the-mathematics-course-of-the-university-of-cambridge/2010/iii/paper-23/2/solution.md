<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The coefficient [ring](../../../../../ring.md) $I$ is complete for its $p$-adic norm, with uniformizer $p$ and residue field $\overline{\mathbb F}_p$. Its residue field is infinite, so **$I$ is not compact**. The measure construction uses completeness, not compactness of the coefficient [ring](../../../../../ring.md).

An $I$-valued [p-adic measure](../../../../../p-adic-measure.md) on $G$ is a bounded $I$-linear functional

$$
\mu:C(G,I)\longrightarrow I,
$$

on the continuous functions with the uniform norm. Equivalently it assigns a value $\mu(C)\in I$ to each clopen subset, finitely additively on disjoint unions. Integration of a locally constant function is defined by

$$
\int_G\sum_j a_j\mathbf1_{C_j}\,d\mu=\sum_j a_j\mu(C_j).
$$

Refining finite clopen partitions shows that this is independent of the expression. Since every $\mu(C_j)\in I$, the nonarchimedean triangle inequality gives $|\int f\,d\mu|_p\leq\|f\|_\infty$.

Locally constant functions are uniformly dense in $C(G,I)$. Indeed, for every $n$, continuity and compactness of $G$ supply a finite clopen partition on which $f$ is constant modulo $p^nI$; choose one value of $f$ on each part. These approximations converge uniformly, and completeness of $I$ extends integration uniquely. Conversely, a bounded functional gives $\mu(C)=\mu(\mathbf1_C)$ and finite additivity. This proves the equivalence of the two definitions. Ordinary countable additivity of real measures is not part of the definition.

Define the [Iwasawa algebra](../../../../../iwasawa-algebra.md) by

$$
I[[G]]=\varprojlim_{U}I[G/U]=\varprojlim_{U,n}(I/p^nI)[G/U],
$$

where $U$ runs over open subgroups. Since $G$ is an abelian [profinite group](../../../../../profinite-group.md), every such quotient is a finite abelian [group](../../../../../group-split.md). The transition map for $V\subseteq U$ sends a basis element $[gV]$ to $[gU]$, so sums coefficients over the fibers.

A [p-adic measure](../../../../../p-adic-measure.md) defines an element of this inverse limit by

$$
\mu_U=\sum_{gU\in G/U}\mu(gU)[gU].
$$

Finite additivity is precisely compatibility under the transition maps. Conversely, compatible coefficients define values on every coset and hence on every clopen subset: any clopen subset is a union of cosets of one open subgroup, by compactness and a finite common refinement. Compatibility makes the resulting value independent of that subgroup. The preceding integration argument then constructs the [p-adic measure](../../../../../p-adic-measure.md).

Finally, multiplication is [convolution of p-adic measures](../../../../../convolution-of-p-adic-measures.md). On a finite quotient its coefficients are

$$
(\mu*\nu)(gU)=\sum_{aU\in G/U}\mu(aU)\nu(a^{-1}gU).
$$

This is exactly the coefficient of $[gU]$ in $\mu_U\nu_U$. Equivalently,

$$
\int_G h\,d(\mu*\nu)=\int_G\!\int_Gh(xy)\,d\mu(x)\,d\nu(y),
$$

first for locally constant $h$, then by uniform approximation. The Dirac measure at the identity corresponds to the identity element of the [group algebra](../../../../../group-algebra.md). We have proved a bijection respecting addition, scalar multiplication and multiplication:

$$
\boxed{I[[G]]\simeq\operatorname{Meas}(G,I).}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
