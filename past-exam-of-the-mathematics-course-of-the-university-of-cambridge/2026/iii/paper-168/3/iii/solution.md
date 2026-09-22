<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Replace $\mathcal A$ by its [upward closure of a set family](../../../../../../upward-closure-of-a-set-family.md) $\overline{\mathcal A}$; this remains an [intersecting family](../../../../../../intersecting-family.md) and can only make the desired containment easier. Apply the [regularity lemma for Boolean functions](../../../../../../regularity-lemma-for-boolean-functions.md) to its indicator with parameters $(\varepsilon/10,p,r,\varepsilon/2)$, where $r$ is chosen from part (ii) with density threshold $\varepsilon/2$. We obtain a bounded set $J$ such that all but $\varepsilon/2$ of the $\mu_p$-weighted restrictions are $(\varepsilon/10,p,r)$-quasirandom.

Let $\mathcal B\subseteq\mathcal P(J)$ consist of assignments $u$ for which the restriction is quasirandom and has $p$-biased expectation at least $\varepsilon/2$. Restrictions excluded because of irregularity contribute at most $\varepsilon/2$, and the remaining excluded restrictions contribute at most $\varepsilon/2$ by their conditional density. Hence

$$
\mu_p(\mathcal A\setminus\overline{\mathcal B})\leq\varepsilon.
$$

It remains to prove that $\mathcal B$ is intersecting. If disjoint $u,v\in\mathcal B$ existed, part (ii) would give $\mathbb E_{1/2}f_u>1/2$ and $\mathbb E_{1/2}f_v>1/2$. Couple two unbiased complementary assignments on $[n]\setminus J$. Since two subsets of a common finite probability space having measures greater than $1/2$ must intersect, some complementary pair would make both restrictions equal to one. Together with disjoint $u,v$, this would produce two disjoint members of $\mathcal A$, a contradiction. Therefore $\mathcal B$ is intersecting, proving the [Dinur-Friedgut junta theorem for intersecting families](../../../../../../dinur-friedgut-junta-theorem-for-intersecting-families.md) with $m=|J|$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
