<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use disjoint [Java arrays](../../../../../../java-array.md) for the old and new generations:
```
java
static void step(boolean[][] old, boolean[][] next) {
    for (int i = 0; i < old.length; i++) {
        for (int j = 0; j < old[i].length; j++) {
            next[i][j] = nextCell(old, i, j);
        }
    }
}
```
Every decision reads only `old`, so all cells undergo the simultaneous [Conway Game of Life](../../../../../../conway-game-of-life.md) transition. The second board must have the same dimensions and share no row arrays with the first. Afterwards swap their references for the following step.

Writing each new cell immediately into the input board would expose a mixture of old and new states to later neighbour counts. The result would depend on the traversal order and would no longer be the specified simultaneous automaton. For example, put the three live cells at $(2,1),(2,2),(2,3)$ on an otherwise dead $5\times5$ board. The simultaneous result is the vertical triple $(1,2),(2,2),(3,2)$. During a naive row-major overwrite, $(1,2)$ becomes live first. The next cell $(1,3)$ now sees that new cell as well as the old cells $(2,2),(2,3)$, so it is incorrectly born with three counted neighbours. This explicitly exhibits the mixture of generations. **A second generation array, or explicit preservation of overwritten old information, is essential.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10](../../10.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
