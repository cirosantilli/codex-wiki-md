<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Maintain one [array index](../../../../../array-index.md) per input and a candidate value. Cycle through the [arrays](../../../../../array-data-structure.md), counting consecutive agreements with that candidate; when a larger head is encountered, start counting agreements again. `p` is an auxiliary [array](../../../../../array-data-structure.md) of $m$ indices, not a copy of any input.
```
PROCEDURE commonMany(as, n, m);
VAR p: ARRAY m OF INTEGER;
    j, candidate, agree, x: INTEGER;
BEGIN
  FOR j := 0 TO m-1 DO
    p[j] := 0;
    IF n[j] = 0 THEN RETURN None END
  END;
  candidate := as[0][0];
  j := 0; agree := 0;
  WHILE agree < m DO
    IF p[j] = n[j] THEN RETURN None END;
    x := as[j][p[j]];
    IF x < candidate THEN
      p[j] := p[j] + 1
    ELSIF x = candidate THEN
      agree := agree + 1;
      j := (j + 1) MOD m
    ELSE
      candidate := x;
      agree := 1;
      j := (j + 1) MOD m
    END
  END;
  RETURN Some(candidate)
END commonMany;
```
The [loop invariant](../../../../../loop-invariant.md) has three parts. All indices satisfy $0\leq p[t]\leq n[t]$; no discarded entry is common to every input; and every original common value is at least `candidate`. Additionally, the `agree` cyclically consecutive [arrays](../../../../../array-data-structure.md) immediately preceding index `j` have heads equal to `candidate`. These facts are true initially, with an empty agreement run.

A head below `candidate` is not globally common, by the lower-bound clause, so advancing its pointer is safe. A head above `candidate` gives a new lower bound: every globally common value lies in this array's unprocessed suffix and so is at least its head. Only this array is yet certified to agree with the new candidate. An equal head extends the run by one. An exhausted suffix proves absence; a run of $m$ agreements covers every array exactly once and proves that `candidate` is common, and the lower-bound clause proves minimality. The exhaustion test precedes each dereference, including after the last entry of a suffix is discarded.

For [algorithm termination](../../../../../algorithm-termination.md) and [time complexity](../../../../../time-complexity.md), charge comparisons to the pair `(j,p[j])`. A fixed entry is discarded at most once, can raise the candidate at most once, and can be counted as an agreement at most once: before the same array is revisited, either the algorithm has finished or the candidate has strictly increased. Thus there are at most three comparisons per input entry, besides the $O(m)$ initialization. **The result is the smallest common value or `None` in $O(m+\sum_t n[t])$ time and $O(m)$ auxiliary space.** For $m=1$, the first head immediately gives the answer.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
