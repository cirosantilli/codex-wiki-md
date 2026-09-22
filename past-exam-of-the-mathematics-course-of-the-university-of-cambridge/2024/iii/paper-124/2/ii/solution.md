<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

It suffices to recognize non-reachability in [NL](../../../../../../nl-complexity.md), since directed reachability is NL-complete. Let $c_k$ be the number of vertices reachable from $s$ by a directed path of length at most $k$. Clearly $c_0=1$. The [inductive counting](../../../../../../inductive-counting.md) argument computes and verifies $c_{k+1}$ from $c_k$ using logarithmic space.

For each vertex $v$, reachability within $k+1$ steps has an NL certificate: guess such a path. Non-reachability within $k+1$ steps can be certified relative to the trusted value $c_k$ by enumerating vertices $u$, exhibiting paths of length at most $k$ to exactly $c_k$ distinct vertices, and checking that none is $v$ or has an edge to $v$. Because there are exactly $c_k$ reachable vertices, this list cannot omit a reachable predecessor. Counters, vertex names and one guessed path need only logarithmic space. Repeating this check in a fixed vertex order and counting the positive cases produces the exact $c_{k+1}$.

After $|V|-1$ rounds, the procedure knows the number of all vertices reachable from $s$. It accepts non-reachability of $t$ after certifying, by the same complete enumeration, that $t$ is absent. Thus the complement of directed reachability belongs to NL. Since every NL language reduces to reachability and log-space reductions are closed under complementation, this proves the [Immerman–Szelepcsényi theorem](../../../../../../immerman-szelepcsenyi-theorem.md)

$$
\boxed{\mathbf{NL}=\mathbf{co\text{-}NL}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
