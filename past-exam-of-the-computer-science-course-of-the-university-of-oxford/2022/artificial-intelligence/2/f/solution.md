<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Retain the ordered position state $(p,q)$, the same initial state and the [goal test](../../../../../goal-test.md) $p=q$, with unit joint-action cost. Replace the deterministic [search transition model](../../../../../search-transition-model.md) by a [set](../../../../../set-split.md)-valued outcome relation. Let

$$
R(p,u)=
\begin{cases}
\{\delta(p,L),\delta(p,R)\},&u\in\{L,R\},\\
\{\delta(p,u)\},&u\in\{U,D,W\}.
\end{cases}
$$

Then

$$
\boxed{\operatorname{Results}((p,q),(u,v))=R(p,u)\times\{\delta(q,v)\}.}
$$

Here $\delta$ for an attempted move leaving the board returns the current room. This explicit boundary convention keeps every outcome inside the [state space](../../../../../state-space.md); alternatively disable a horizontal command unless both possible destinations are legal. Mrs Robot’s commands can still be restricted to legal moves as before.

The result is a fully observable [nondeterministic planning](../../../../../nondeterministic-planning.md) problem, assuming that actual positions are observed after every step. Both possible horizontal outcomes must be represented, even though they may coincide at a boundary or when $n=1$. No outcome [probabilities](../../../../../probability.md) are supplied, so attaching equal [probabilities](../../../../../probability.md) would add an assumption. Its solution is a position-dependent plan or policy.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
