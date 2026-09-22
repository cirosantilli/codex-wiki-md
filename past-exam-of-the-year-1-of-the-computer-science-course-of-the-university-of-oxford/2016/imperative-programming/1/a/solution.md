<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use two [array indices](../../../../../array-index.md), advancing only the smaller current entry. Here and in Questions 1–4, code is structured [Oberon](../../../../../oberon-programming-language.md)-style pseudocode: `RETURN` exits a procedure, `Some(x)` and `None` distinguish success and absence, and `AND` short-circuits from left to right. Arithmetic is exact where the source asks us to ignore [integer overflow](../../../../../integer-overflow.md).
```
PROCEDURE common(a, N, b, M): INTEGER;
VAR i, j: INTEGER;
BEGIN
  i := 0; j := 0;
  WHILE a[i] # b[j] DO
    IF a[i] < b[j] THEN i := i + 1
    ELSE j := j + 1
    END
  END;
  RETURN a[i]
END common;
```
Let $z$ be the smallest common value, and let $a[p]=b[q]=z$. Existence implies $N,M>0$. A useful [loop invariant](../../../../../loop-invariant.md) is $0\leq i\leq p<N$, $0\leq j\leq q<M$, with no common value among the discarded prefixes $a[0..i)$ and $b[0..j)$. Initially the prefixes are empty. If $a[i]<b[j]$, then $a[i]$ cannot equal any entry of $b[j..M)$ because that [sorted array](../../../../../sorted-array.md) is increasing; it cannot be a common value in the discarded prefix either. Moreover $i=p$ would imply $z=a[i]<b[j]\leq z$, a contradiction. Thus $i<p$ and incrementing $i$ is safe. The other branch is symmetric.

Every guard and return therefore uses valid [array indices](../../../../../array-index.md), even without explicit bounds tests. The [loop variant](../../../../../loop-variant.md) $(p-i)+(q-j)$ decreases on each iteration. At exit the equal entries form a common value no larger than $z$, hence equal $z$. There are at most $N+M-2$ increments and constant work per increment. **The procedure returns the smallest common value in $O(N+M)$ time and $O(1)$ auxiliary space.**

## ↑ Ancestors (12)

1. [A](../a.md)
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
