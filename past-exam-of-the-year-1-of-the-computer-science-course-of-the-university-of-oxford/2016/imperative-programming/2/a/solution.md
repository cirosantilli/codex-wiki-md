<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Evaluate the supplied [function](../../../../../function-split.md) once at each positive [integer](../../../../../integer-split.md), retaining its largest value so far. In particular do not initialize the maximum to zero: $f$ might be negative everywhere.
```
PROCEDURE record(f, emit);
VAR n, best, y: INTEGER;
BEGIN
  best := f(1);
  emit(1);
  n := 2;
  WHILE TRUE DO
    y := f(n);
    IF y > best THEN
      emit(n);
      best := y
    END;
    n := n + 1
  END
END record;
```
At the loop head the [loop invariant](../../../../../loop-invariant.md) is $n\geq2$, `best` $=\max\{f(i):1\leq i<n\}$, and precisely the [record values](../../../../../record-value.md) with argument less than $n$ have been emitted, in increasing argument order. The first argument is a record because its comparison set is empty. The strict test correctly excludes ties. Updating `best` only on a strict increase preserves the [loop invariant](../../../../../loop-invariant.md).

**Exactly one call of `f` is made per processed argument.** For an arbitrary supplied [function](../../../../../function-split.md), an unexamined argument can have a value larger than all previous values, so skipping its evaluation cannot be correct in general. This assumes $f$ is a total, deterministic [function](../../../../../function-split.md); the requested infinite computation ignores [integer overflow](../../../../../integer-overflow.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
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
