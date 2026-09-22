<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**[Depth-first tree search](../../../../../depth-first-tree-search.md) is neither complete nor optimal for minimizing rounds.**

For incompleteness, use the two-row, three-column board from part (c), with exit $(1,2)$. If stay is the first action explored, [depth-first tree search](../../../../../depth-first-tree-search.md) follows the repeating state forever. Moving the rabbit down instead survives the round: under legal horizontal-then-vertical movement the fox moves to $(1,0)$ and then $(1,1)$, leaving the rabbit safely at the exit. Thus a one-round escape exists but is never reached in this action order.

For nonoptimality, use an unobstructed one-row board with columns $0,\ldots,6$, initial fox column $0$, initial rabbit column $4$, and exits at columns $3$ and $6$. Moving left once escapes at column $3$ with the fox at column $2$. Moving right twice escapes at column $6$ with successive fox positions $2,4$. A [depth-first tree search](../../../../../depth-first-tree-search.md) that explores the latter route first returns **two rounds although one suffices**. This counterexample supplies an actual returned, suboptimal escape independently of the infinite-branch example.

## ↑ Ancestors (11)

1. [E](../e.md)
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
