<h1 id="10/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [one-row in-place Life update](../../../../../../one-row-in-place-life-update.md) needs only one saved row plus a few running sums. Before processing row $i$, `above[j]` stores the old row $i-1$, and all rows $i$ and below are still old. Let a column sum be the number of old live cells in that column in rows $i-1,i,i+1$. The three adjacent column sums, minus the center, give the required neighbour count.
```
java
static int columnSum(boolean[][] board, boolean[] above,
                     int i, int j) {
    int total = above[j] ? 1 : 0;
    if (board[i][j]) total++;
    if (i + 1 < board.length && board[i + 1][j]) total++;
    return total;
}

static void stepInPlace(boolean[][] board) {
    int width = board[0].length;
    boolean[] above = new boolean[width];
    for (int i = 0; i < board.length; i++) {
        int left = 0;
        int middle = columnSum(board, above, i, 0);
        for (int j = 0; j < width; j++) {
            int right = j + 1 < width
                ? columnSum(board, above, i, j + 1) : 0;
            boolean oldCenter = board[i][j];
            int neighbours = left + middle + right
                - (oldCenter ? 1 : 0);
            boolean newCenter = neighbours == 3
                || (oldCenter && neighbours == 2);
            above[j] = oldCenter;
            board[i][j] = newCenter;
            left = middle;
            middle = right;
        }
    }
}
```
When column $j$ is processed, `left` and `middle` were computed before their cells were overwritten. `right` is computed now from untouched column $j+1$, including its untouched `above[j+1]` entry. Thus all three sums describe old cells. Saving `oldCenter` into `above[j]` preserves the old current row for the next row's processing; no later computation in the current row rereads that changed entry, because its old contribution is already in the running sums. This proves the inner-loop invariant and then the row invariant by induction.

Initially `above` is all false, representing the dead exterior above the board. The missing left and right columns contribute zero; the bottom row omits any row below it. Hence all four boundaries follow the required convention. **The update takes $O(HW)$ time and one $W$-element auxiliary boolean vector**, which is exactly a 1000-element vector for the requested board. It uses one board array throughout and does not silently keep a second board or two auxiliary rows.

## ↑ Ancestors (11)

1. [D](../d.md)
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
