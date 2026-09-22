<h1 id="4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the segment as $AB$, where $|A|=n-k$ and $|B|=k$. The desired [array rotation](../../../../../../array-rotation.md) is $BA$. Reverse each block, then the whole segment:
```
PROCEDURE rotate(i, n, k: INTEGER);
BEGIN
  IF (k = 0) OR (k = n) THEN RETURN END;
  reverse(i, n-k);
  reverse(i+n-k, k);
  reverse(i, n)
END rotate;
```
The state changes are $AB\to A^RB\to A^RB^R\to BA$, using the [list reversal](../../../../../../list-reversal.md) identity supplied in the paper and reversal being an [involution](../../../../../../involution.md). **Three reversals implement the right rotation in $O(n)$ time and $O(1)$ auxiliary space.** The initial return covers empty and identity rotations.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
