<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each user define its [set](../../../../../set-split.md) of eligible ads by

$$
E_i=\{j:\mathcal S^i\cap\mathcal S_j\ne\varnothing\}.
$$

This uses the [intersection](../../../../../set-intersection.md) of demographic-group memberships: belonging to one advertised group suffices, because the eligibility condition is a [set union](../../../../../set-union.md). A user in several groups still receives at most one ad.

A direct [algorithm](../../../../../algorithm-split.md) is to process users independently. For user $u_i$, scan ads $a_j$ until finding one for which some group $S_\ell$ belongs to both $\mathcal S^i$ and $\mathcal S_j$. Assign that ad and stop processing this user. If no such ad exists, leave the user unassigned. There is no upper bound on the number of different users who can receive the same ad, so these decisions do not compete for an ad resource.

For correctness, every produced impression has a shared permitted group, and the stopping rule assigns at most one ad to each user. Conversely, a user with $E_i=\varnothing$ cannot receive an ad in any [feasible solution](../../../../../feasible-point.md). Since every other user can contribute at most one impression, every [feasible solution](../../../../../feasible-point.md) has value at most

$$
\bigl|\{i:E_i\ne\varnothing\}\bigr|.
$$

The [algorithm](../../../../../algorithm-split.md) attains this bound, proving

$$
\boxed{\text{maximum impressions}=\bigl|\{i:\mathcal S^i\cap\mathcal S_j\ne\varnothing\text{ for some }j\}\bigr|.}
$$

Represent each membership [set](../../../../../set-split.md) by a length-$k$ [array](../../../../../array-data-structure.md) of [Boolean variables](../../../../../boolean-variable.md). Testing one user-ad pair costs $O(k)$, so all tests and input setup take $O(nmk+(n+m)k+n+m+k)$ time in [Big O notation](../../../../../big-o-notation.md), which is [polynomial time](../../../../../polynomial-time.md) in all three parameters. For positive $n,m,k$, this simplifies to $O(nmk)$.

A [maximum flow](../../../../../maximum-flow-problem.md) formulation gives the same result if desired: add [edges](../../../../../edge-of-a-graph.md) $s\to u_i$ with [flow network edge capacity](../../../../../flow-network-edge-capacity.md) $1$, $u_i\to a_j$ with [flow network edge capacity](../../../../../flow-network-edge-capacity.md) $1$ exactly when $j\in E_i$, and $a_j\to t$ with [flow network edge capacity](../../../../../flow-network-edge-capacity.md) $n$. By the [integral max-flow theorem](../../../../../integral-max-flow-theorem.md), an integral [maximum flow](../../../../../maximum-flow-problem.md) selects valid impressions. Setting the last [flow network edge capacity](../../../../../flow-network-edge-capacity.md) to $1$ would impose an extra restriction absent from this paper.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Advanced data structures and algorithms](../../../advanced-data-structures-and-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
