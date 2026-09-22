<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

Use the following standard facts: $A_5$ has order $60$ and is a nonabelian [simple group](../../../../../simple-group.md); the [coset action](../../../../../coset-action.md) on the cosets of an index-$j$ [subgroup](../../../../../subgroup.md) is a transitive [homomorphism](../../../../../homomorphism.md) into $S_j$. If $H<A_5$ has index $j>1$, that action is nontrivial. Its [kernel](../../../../../kernel-of-a-linear-map.md) is a [normal subgroup](../../../../../normal-subgroup.md), hence is trivial by simplicity. It would therefore embed $A_5$ in $S_j$. For $j=2,3,4$ this is impossible since $j!<60$. **There are no [subgroups](../../../../../subgroup.md) of indices 2, 3 or 4.**

An index-5 [subgroup](../../../../../subgroup.md) has order $12$ by [Lagrange's theorem](../../../../../lagrange-s-theorem.md). Consider its natural action on the five letters. It cannot be transitive, since an orbit of size 5 would divide its order by the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md). If it had no fixed letter, its orbits would have sizes 2 and 3. It would then be a [subgroup](../../../../../subgroup.md) of the [permutations](../../../../../permutation.md) preserving that partition, namely $S_2\times S_3$. Exactly half of those 12 [permutations](../../../../../permutation.md) are even, so $(S_2\times S_3)\cap A_5$ has order 6, too small to contain $H$.

Thus $H$ fixes a letter $i$. The stabilizer of $i$ in $A_5$ is the copy of $A_4$ consisting of even [permutations](../../../../../permutation.md) of the other four letters; it has order 12. Containment and equality of orders force $H$ to equal that stabilizer. Conversely each such stabilizer has index 5. Consequently

$$
\boxed{\text{The index-5 subgroups are precisely }\operatorname{Stab}_{A_5}(i),\quad i=1,\ldots,5.}
$$

These five [subgroups](../../../../../subgroup.md) are distinct: for $i\ne j$, a [three-cycle](../../../../../three-cycle.md) on letters other than $i$ can move $j$, so it belongs to the stabilizer of $i$ but not that of $j$.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
