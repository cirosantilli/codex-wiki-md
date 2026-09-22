<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Track the length `r` of the trailing [constant segment of an array](../../../../../constant-segment-of-an-array.md), and the best length `m` anywhere in the processed prefix:
```
i := 1; r := 1; m := 1;
WHILE i < n DO
  IF a[i] = a[i-1] THEN r := r+1 ELSE r := 1 END;
  IF r > m THEN m := r END;
  i := i+1
END;
```
The [loop invariant](../../../../../loop-invariant.md) is: $1\leq i\leq n$; `r` is the length of the longest constant suffix of $a[0..i)$; and `m` is the length of the longest [constant segment of an array](../../../../../constant-segment-of-an-array.md) within $a[0..i)$. Initially all three lengths are one, using $n\geq1$.

When the next entry equals its predecessor, the trailing constant segment extends by one; otherwise its new length is one. Every new plateau either was already in the old prefix or ends at the new entry, so taking the larger of the old `m` and the new `r` preserves the [loop invariant](../../../../../loop-invariant.md). The [loop variant](../../../../../loop-variant.md) is $n-i$, a [nonnegative integer](../../../../../natural-number.md) decreased by one. At termination $i=n$, so

$$
\boxed{m=\max\{q-p:0\leq p<q\leq n,\ a[p..q)\text{ is constant}\},\qquad T(n)=\Theta(n).}
$$

The [auxiliary space](../../../../../auxiliary-space.md) is $O(1)$, and $n=1$ correctly returns one without entering the loop.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
