<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With a read-only input tape, [deterministic space complexity class](../../../../../../deterministic-space-complexity-class.md) $\mathrm{SPACE}(s(n))$ consists of languages decidable by deterministic [Turing machines](../../../../../../turing-machine.md) using $O(s(n))$ work-tape cells. The [nondeterministic space complexity class](../../../../../../nondeterministic-space-complexity-class.md) $\mathrm{NSPACE}(s(n))$ uses [Nondeterministic Turing machines](../../../../../../nondeterministic-turing-machine.md), with the bound holding on every computation path and acceptance meaning that some path accepts. Input storage is not charged. We use the standard finite-state, fixed-alphabet model.

The [Savitch theorem](../../../../../../savitch-s-theorem.md) is

$$
\boxed{s(n)\geq\log_2 n\Longrightarrow\mathrm{NSPACE}(s(n))\subseteq\mathrm{SPACE}(s(n)^2)}.
$$

First suppose a work-space budget $m\geq\lceil\log_2(n+2)\rceil$ is available. A [configuration graph](../../../../../../configuration-graph.md) for computations restricted to $m$ cells has configurations encoded in $O(m)$ bits: work contents, control state and head positions, including $O(\log n)$ bits for the input head. Its size is at most $2^{cm}$ for a machine-dependent constant $c$. Add accept and exit sinks if needed; the size bound merely changes $c$. A reachable configuration has a simple path of length smaller than the number of configurations.

For encoded configurations $u,v$, define $R(u,v,k)$ to ask whether a path of length at most $2^k$ exists. At $k=0$, test equality or one transition. For $k>0$, enumerate every candidate middle configuration $w$ and test

$$
R(u,v,k)=\bigvee_w\bigl[R(u,w,k-1)\wedge R(w,v,k-1)\bigr].
$$

Any path of the given length can be split into two halves of length at most $2^{k-1}$; conversely concatenation gives a path of length at most $2^k$. This proves the recursion. Taking $k=\lceil cm\rceil$ suffices. Depth is $O(m)$, and each recursive frame stores only its endpoints, the current middle configuration and counters in $O(m)$ bits. The two recursive calls are made sequentially and reuse their space. The total is $O(m^2)$, even though the time can be very large.

The printed hypothesis does not say that $s$ is computable. The [space-bound discovery by exit reachability](../../../../../../space-bound-discovery-by-exit-reachability.md) removes that issue. Begin with $m=\lceil\log_2(n+2)\rceil$ and use the preceding recursion to test both whether an accepting state is reachable within the budget and whether a reachable state has a transition leaving the budget. Accept in the first case. If acceptance is absent and an exit is reachable, double $m$ and repeat. If neither is reachable, reject: all computations remain within this finite [configuration graph](../../../../../../configuration-graph.md), and none accepts.

Every path of the original machine uses at most $C s(n)$ cells. Once $m$ reaches that bound there can be no reachable exit, so this procedure terminates. The final budget is $O(s(n))$ by doubling, and all stages reuse the same storage. Hence its deterministic space is $O(s(n)^2)$ without requiring a machine that first computes $s(n)$. This proves the stated general form.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
