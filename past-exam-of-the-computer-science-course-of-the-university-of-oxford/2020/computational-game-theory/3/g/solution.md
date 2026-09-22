<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

**There is exactly one such nontrivial game for every $n\ge1$: the [unanimity game](../../../../../unanimity-game.md) requiring every player.** Put

$$
\boxed{u_N(S)=
\begin{cases}
1,&S=N,\\
0,&S\ne N.
\end{cases}
\qquad\text{Number of games}=1.}
$$

It is a [simple cooperative game](../../../../../simple-cooperative-game.md), and permuting players preserves every [coalition](../../../../../coalition-game-theory.md) value. Thus it has the required [symmetry of players in a cooperative game](../../../../../symmetry-of-players-in-a-cooperative-game.md). It is also a [convex cooperative game](../../../../../convex-cooperative-game.md): if both $S,T$ are winning, all four terms in the [supermodular](../../../../../supermodular-set-function.md) inequality have value $1$; if exactly one is winning, their union is $N$ and their intersection loses, giving equality $1=1$; if neither wins, the right-hand side is zero and the inequality follows from nonnegativity. For $n=1$ the same definition gives the sole player value $1$.

To prove uniqueness, first establish that [convex simple games are unanimity games](../../../../../convex-simple-games-are-unanimity-games.md). If $S,T$ are [winning coalitions](../../../../../winning-coalition.md), the [supermodular](../../../../../supermodular-set-function.md) inequality gives

$$
2=v(S)+v(T)\le v(S\cup T)+v(S\cap T)\le2,
$$

so their intersection is also winning. The family of [winning coalitions](../../../../../winning-coalition.md) is finite and nonempty. Its intersection $K$ is therefore winning and nonempty, since the empty [coalition](../../../../../coalition-game-theory.md) loses. Every winning [coalition](../../../../../coalition-game-theory.md) contains $K$, and monotonicity makes every superset of $K$ winning. Hence $v=u_K$.

If $K$ were a proper nonempty [subset](../../../../../subset.md) of $N$, take $i\in K$ and $j\notin K$, and let $T=N\setminus\{i,j\}$. Then $T\cup\{i\}=N\setminus\{j\}$ contains $K$ and wins, whereas $T\cup\{j\}=N\setminus\{i\}$ loses. This violates [symmetry of players in a cooperative game](../../../../../symmetry-of-players-in-a-cooperative-game.md), which requires those two [coalition](../../../../../coalition-game-theory.md) values to agree. Thus $K=N$, proving the claimed count. The “nontrivial” convention excludes the identically zero game; if that degenerate game were also called simple, it would supply one additional symmetric convex example.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
