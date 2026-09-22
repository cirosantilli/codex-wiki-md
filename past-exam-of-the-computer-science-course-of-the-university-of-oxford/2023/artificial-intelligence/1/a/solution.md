<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $V$ be the traversable squares and $H\subseteq V$ the exits. Sample the [state space](../../../../../state-space.md) at the end of each complete round, so a live state is $s=(r,f)\in V\times V$ with $r\ne f$. The given starting positions specify the initial state. The board and exits are fixed problem data, rather than changing components of the [state space](../../../../../state-space.md).

The rabbit has at most five actions: stay or move to one of its traversable orthogonally adjacent squares. A [search transition model](../../../../../search-transition-model.md) first applies that action, giving $r'$, and immediately checks for capture at $r'=f$. Otherwise hold $r'$ fixed and apply the fox rule twice, checking for capture after each step. A capture is terminal failure; it must not be overlooked merely because the fox could subsequently move elsewhere. A surviving successor is $(r',f'')$. Equivalently, omit actions whose complete-round outcome is capture.

The [goal test](../../../../../goal-test.md) is **the rabbit is on an exit after surviving the fox's entire turn**: $r'\in H$ and no capture occurred in that round. Merely entering an exit before the fox moves is insufficient. Each surviving [search transition model](../../../../../search-transition-model.md) step has cost one when minimizing rounds.

Only legal moves are considered when applying the stated horizontal preference: try a legal horizontal step that reduces horizontal separation, otherwise a legal vertical step that reduces vertical separation, otherwise stay. If a blocked preferred direction is instead interpreted as forcing a stay immediately, the counterexamples below and all completeness and optimality conclusions remain valid.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
