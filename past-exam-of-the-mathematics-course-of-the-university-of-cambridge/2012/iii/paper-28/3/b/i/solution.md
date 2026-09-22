<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [idele group](../../../../../../../idele-group.md) is the restricted product

$$
J_K=\prod_v' K_v^\times=\{(x_v):x_v\in K_v^\times,\ x_v\in\mathcal O_v^\times\text{ for almost every finite }v\},
$$

with componentwise multiplication and the [restricted product topology on the idele group](../../../../../../../restricted-product-topology-on-the-idele-group.md) relative to the unit groups at finite places. We need [weak approximation for number fields](../../../../../../../weak-approximation-for-number-fields.md) only at the finitely many specified coordinates, not density in the full restricted-product topology.

Here is a proof including the Archimedean places. At each finite place in $S$, choose $a_v\in K$ sufficiently close to $x_v$, using the definition of the completion. Choose a nonzero $d\in\mathcal O_K$ clearing their denominators. Pick powers $\mathfrak p_v^{m_v}$ so that $|z/d|_v<\varepsilon$ whenever $z\in\mathfrak p_v^{m_v}$. Put $I=\prod_{v\in S,\ v\text{ finite}}\mathfrak p_v^{m_v}$. For each positive rational integer $M$ coprime to the rational primes below these places, the [Chinese remainder theorem](../../../../../../../chinese-remainder-theorem.md) gives $b_M\in\mathcal O_K$ with $b_M\equiv Md a_v\pmod{\mathfrak p_v^{m_v}}$. All of $b_M+I$ satisfy the same congruences.

Under the [Minkowski embedding of a number field](../../../../../../../minkowski-embedding-of-a-number-field.md), $I$ is a full lattice in $\mathbb R^{r_1}\times\mathbb C^{r_2}$. A fundamental parallelepiped is bounded, so every real vector is within a fixed distance of this lattice, uniformly over its translates. Choose a target vector whose coordinates at the specified Archimedean places are those of $Md x_v$, assigning arbitrary values at the other Archimedean places. There is $b\in b_M+I$ within that fixed distance of the target. Dividing by $Md$ makes all specified Archimedean errors tend to zero as $M\to\infty$ through the allowed integers. At finite places $M$ is a unit, so the earlier congruence bounds persist. By taking the initial approximations sufficiently close, the ultrametric inequality gives the requested errors there too. **Thus some $\boxed{y=b/(Md)\in K}$ satisfies every required inequality.** If there are no finite places, set $I=\mathcal O_K$ and omit the congruences.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
