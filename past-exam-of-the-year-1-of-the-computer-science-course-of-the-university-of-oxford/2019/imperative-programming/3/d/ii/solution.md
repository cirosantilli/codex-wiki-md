<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The original routine uses $O(1)$ auxiliary space and at most $O(N^2)$ membership work. A bitmap with universe size $M$ uses **$\Theta(M)$ extra storage and $\Theta(N)$ work in the [sequence](../../../../../../sequence.md)-generation loop** because membership and insertion each take constant time. Here the safe universal bound chooses $M=N(N-1)/2+1$, so extra storage is $\Theta(N^2)$ for growing $N$.

Initialization must be accounted for separately: creating and clearing a Boolean [array](../../../../../../array-data-structure.md) of length $M$ takes $\Theta(M)$ work in the usual [array](../../../../../../array-data-structure.md)-initialization model. Consequently **the complete one-shot routine takes $\Theta(M+N)$**, which is $\Theta(N^2)$ with this conservative universe bound. The faster lookup does not make that quadratic setup disappear. If the bitmap is already initialized, or the analysis explicitly charges only the generation phase, the remaining phase is linear. A tighter known bound on values can reduce the universe cost, but no unproved growth bound is needed here.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
