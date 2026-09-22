<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A maximal [intersecting family](../../../../../intersecting-family.md) $\mathcal F\subseteq\mathcal P([n])$ is an [up-set](../../../../../up-set.md): if $A\in\mathcal F$ and $A\subseteq B$, then $B$ intersects every member, so maximality forces $B\in\mathcal F$. For every complementary pair $\{A,A^c\}$, at most one member lies in $\mathcal F$. If neither did, maximality would give $B\in\mathcal F$ disjoint from $A$; then $B\subseteq A^c$, and the up-set property would put $A^c$ in $\mathcal F$, a contradiction. Exactly one set from each complementary pair occurs, so

$$
\boxed{|\mathcal F|=2^{n-1}.}
$$

For $n\geq4$, three pairwise nonisomorphic examples are:

- the star $\{A:1\in A\}$;
- the triangle family $\{A:|A\cap\{1,2,3\}|\geq2\}$;
- the majority family $\{A:|A|>n/2\}$ when $n$ is odd, and, when $n$ is even, this family together with the $n/2$-sets containing $1$.

Their smallest members have different sizes except at $n=4$, where the inclusion graphs of the minimal two-sets are respectively a triangle and a three-edge star. Thus they are nonisomorphic.

The [Erdős-Ko-Rado theorem](../../../../../erdos-ko-rado-theorem.md) says that if $n\geq2r$ and $\mathcal F\subseteq[n]^{(r)}$ is intersecting, then

$$
|\mathcal F|\leq\binom{n-1}{r-1}.
$$

For the [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md) proof, the family of complements $\mathcal F^c\subseteq[n]^{(n-r)}$ is disjoint from the $(n-r)$th upper shadow of $\mathcal F$: otherwise one member of $\mathcal F$ would be contained in the complement of another. Kruskal–Katona says that when $|\mathcal F|=\binom{n-1}{r-1}$ this upper shadow has at least $\binom{n-1}{r}$ members, with a strict corresponding inequality above that threshold. Since these two disjoint families lie in one level of size $\binom nr$, the EKR bound follows.

For the averaging proof, place $[n]$ in a cyclic order. Among the $n$ cyclic intervals of length $r$, an intersecting family contains at most $r$: after fixing one interval, the possible intersecting intervals can be paired by their first separating endpoint. Double-counting pairs consisting of a cyclic order and a member of $\mathcal F$ that appears as an interval gives

$$
\frac{|\mathcal F|}{\binom nr}\leq\frac rn,
$$

which is the same bound. This is the [Katona circle method](../../../../../katona-circle-method.md).

The minimum size $f_r(n)$ does not tend to infinity. Fix a core $S\subseteq[n]$ of size $2r-1$ and take

$$
\mathcal F=[S]^{(r)}.
$$

Any two members intersect. If an $r$-set $A$ is not contained in $S$, then $|A\cap S|\leq r-1$, so the remaining at least $r$ points of $S$ contain a member of $\mathcal F$ disjoint from $A$. Thus $\mathcal F$ is maximal intersecting in $[n]^{(r)}$, and

$$
f_r(n)\leq\binom{2r-1}{r}
$$

independently of $n$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 109](../../paper-109-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
