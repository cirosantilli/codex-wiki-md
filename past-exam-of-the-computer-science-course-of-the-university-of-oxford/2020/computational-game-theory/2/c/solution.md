<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The equilibrium assignment is $(S_1,S_2,S_3,S_4)\mapsto(r_2,r_3,r_4,r_1)$, with [utility](../../../../../utility.md) [vector](../../../../../vector.md) $(0.7,0.7,0.9,0.4)$.** Apply [backward induction](../../../../../backward-induction.md) to the finite [perfect-information game](../../../../../perfect-information-game.md), accounting for the two friendship pairs in every terminal assignment. Student $S_4$ receives the last room and has no remaining choice. Given the first two rooms, $S_3$ chooses the remaining room maximizing their own room value plus $0.4$ if adjacent to $S_2$.

The following complete third-stage comparisons summarize the continuations. The [utility](../../../../../utility.md) in the last column is $S_2$'s resulting [utility](../../../../../utility.md), after $S_3$ makes the indicated [best response](../../../../../best-response.md).

| $S_1$ room | $S_2$ room | Optimal $S_3$ room | Resulting $U_2$ |
| --- | --- | --- | --- |
| $r_1$ | $r_2$ | $r_4$ | $0.5$ |
| $r_1$ | $r_3$ | $r_2$ | $0.7$ |
| $r_1$ | $r_4$ | $r_2$ | $0$ |
| $r_2$ | $r_1$ | $r_4$ | $0$ |
| $r_2$ | $r_3$ | $r_4$ | $0.7$ |
| $r_2$ | $r_4$ | $r_3$ | $0.4$ |
| $r_3$ | $r_1$ | $r_2$ | $0.4$ |
| $r_3$ | $r_2$ | $r_4$ | $0.5$ |
| $r_3$ | $r_4$ | $r_2$ | $0$ |
| $r_4$ | $r_1$ | $r_2$ | $0.4$ |
| $r_4$ | $r_2$ | $r_1$ or $r_3$ | $0.9$ |
| $r_4$ | $r_3$ | $r_2$ | $0.7$ |

For example, after $S_1$ takes $r_2$ and $S_2$ takes $r_3$, student $S_3$ compares $r_1$, giving $0$, with $r_4$, giving $0.5+0.4=0.9$. Choosing $r_4$ also gives $S_2$ the adjacency bonus, making $U_2=0.3+0.4=0.7$. The last room $r_1$ is adjacent to $S_1$'s $r_2$.

The table makes $S_2$ choose $r_3,r_3,r_2,r_2$ after first-stage choices $r_1,r_2,r_3,r_4$, respectively. Their resulting consequences for $S_1$ are $0.5,0.7,0$, and either $0$ or $0.4$. Thus $S_1$ strictly prefers $r_2$, proving the displayed outcome.

There is an off-path tie for $S_3$ after $(r_4,r_2)$, so the entire [subgame perfect equilibrium](../../../../../subgame-perfect-equilibrium.md) [strategy profile](../../../../../strategy-profile.md) need not be unique. Either choice, or any mixture of them, gives $S_1$ at most $0.4$ after choosing $r_4$, below $0.7$. The equilibrium assignment on the played path is therefore unaffected by this tie. Specifying these optimal continuations at every history, including the unplayed ones, supplies a [subgame perfect equilibrium](../../../../../subgame-perfect-equilibrium.md) rather than merely a proposed path.

## ↑ Ancestors (11)

1. [C](../c.md)
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
