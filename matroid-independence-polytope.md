# Matroid independence polytope

↑ **Parent:** [Matroid](matroid.md)

For a finite [matroid](matroid.md) $M=(E,\mathcal I)$, the [convex hull](convex-hull.md) of the indicator vectors of its [matroid independent sets](independent-set-of-a-matroid.md) is exactly the displayed system, where $x(A)=\sum_{e\in A}x_e$. It is an integral [polytope](convex-polytope.md). The equality $x(E)=r_M(E)$ instead gives the face corresponding to [matroid bases](basis-of-a-matroid.md); independence does not require that equality.

**Proof.** If $I$ is independent, $|I\cap A|\leq r_M(A)$, so every independent indicator and every [convex combination](convex-combination.md) of them satisfies the inequalities. For the reverse inclusion, take an arbitrary real objective $c$. List its positive coordinates in nonincreasing order as $c_1\geq\cdots\geq c_k>0$, put $c_{k+1}=0$ and let $S_i$ be the first $i$ elements in this ordering. Run the [matroid greedy algorithm](matroid-greedy-algorithm.md) on these elements, obtaining an independent set $I$. At every prefix the selected elements are maximal in $S_i$: an earlier rejected element cannot become admissible after further additions, by heredity. The augmentation axiom implies that every maximal independent set in $S_i$ has size $r_M(S_i)$. Hence $|I\cap S_i|=r_M(S_i)$.

For every point satisfying the displayed system, nonnegativity and telescoping give

$$
c^Tx\leq\sum_{j=1}^kc_jx_{e_j}
=\sum_{i=1}^k(c_i-c_{i+1})x(S_i)
\leq\sum_{i=1}^k(c_i-c_{i+1})r_M(S_i)
=c^T\mathbf1_I.
$$

Thus every linear objective is maximized by an independent indicator, with the empty set used if all coefficients are nonpositive. [Singleton](singleton-mathematics.md) rank inequalities bound every coordinate between zero and one, making the system [compact](compact-space.md). If it contained a point outside the [compact](compact-space.md) [convex hull](convex-hull.md) of independent indicators, the finite-dimensional [separating hyperplane theorem](hyperplane-separation-theorem.md) would supply an objective strictly larger at that point than at every independent indicator, a contradiction. This proves equality and integrality without assuming the desired convex-hull description in advance. Negative objective coefficients are discarded explicitly; maximizing over independent sets differs from maximizing over bases when such coefficients occur.

**Table of contents**

- [Forest polytope](forest-polytope.md)

## ↑ Ancestors (5)

1. [Matroid](matroid.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Forest polytope](forest-polytope.md)
- [Solution](past-exam-of-the-integer-programming-course-of-the-university-of-oxford/2011/1/e/solution.md)
