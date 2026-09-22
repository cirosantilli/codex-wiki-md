<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**Every [subgame perfect equilibrium](../../../../../subgame-perfect-equilibrium.md) outcome is [Pareto optimal](../../../../../pareto-efficiency.md) under the stated consecutive-friend and bonus conditions.** Partition the choosing order into blocks: a single student without a friend, or two friends who choose consecutively. Their slots in the choosing order are adjacent; the proof must separately establish when their allocated rooms will be adjacent.

Let $R$ be the rooms remaining before a friend block, with leader $i$ and follower $j$. Because $0\le v_{i,r},v_{j,r}\le1$ and $f_i,f_j>1$, each friend strictly prefers every adjacent-to-friend allocation to every nonadjacent one. After leader $i$ takes room $r$ with an available adjacent room, follower $j$ therefore takes their uniquely highest-valued room among the available neighbors of $r$. The leader consequently knows they will receive the adjacency bonus.

If $R$ contains at least one pair of adjacent rooms, let $E(R)$ be its nonisolated rooms: the rooms having an available neighbor. Leader $i$ must choose from $E(R)$, because choosing there guarantees [utility](../../../../../utility.md) greater than $1$, whereas an isolated choice gives at most $1$. Since the bonus is then fixed and room values are distinct, the leader chooses their unique maximum-value room in $E(R)$. The follower chooses their unique best neighbor. Later students cannot change either allocated room, so later play cannot alter these two students' [utilities](../../../../../utility.md).

If $R$ contains no adjacent pair, neither friend can obtain the bonus under any allocation of rooms from $R$. Both simply choose their uniquely most valuable remaining room in turn. Removing rooms cannot create a new physical adjacency, so no hidden later move can change that conclusion. A one-student block likewise chooses their unique best available room.

Now compare the equilibrium assignment $a$ with any proposed [Pareto improvement](../../../../../pareto-improvement.md) $a'$. Induct over these blocks, assuming earlier blocks' rooms are already fixed. Thus $a$ and $a'$ have the same remaining [set](../../../../../set-split.md) $R$ at the present block. A lone student's room must stay fixed by strict preferences.

For a friend block obtaining adjacency in $a$, both students must retain adjacency in $a'$: losing a bonus larger than $1$ cannot be compensated by any room-value increase. The leader's room in $a'$ must therefore belong to $E(R)$. It cannot differ from the unique highest-valued room the leader selected there without reducing that leader's [utility](../../../../../utility.md). Once the leader's room is fixed, the follower likewise must retain the uniquely best available neighbor. If $R$ has no adjacent pair, both rooms stay fixed by the ordinary strict-ranking argument.

Thus every block's rooms are unchanged. The only assignment weakly improving all students is $a$ itself, so no strict improvement is possible. This proves [Pareto efficiency of serial dictatorship with consecutive friends](../../../../../pareto-efficiency-of-serial-dictatorship-with-consecutive-friends.md). The proof applies to every [subgame perfect equilibrium](../../../../../subgame-perfect-equilibrium.md), since the required choices at each block are strict [best responses](../../../../../best-response.md) determined by the available rooms.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
