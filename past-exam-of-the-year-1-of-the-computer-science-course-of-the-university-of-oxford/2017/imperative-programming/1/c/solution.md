<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Propagate each carry into the next position, lengthening the array if necessary:

```
procedure Normal(var n: number)
    i := 0
    while i < len(n) do
        carry := floor(n[i] / base)
        n[i] := n[i] - carry*base
        if carry != 0 then
            if i+1 = len(n) then
                assert carry > 0
                Lengthen(n)
            n[i+1] := n[i+1] + carry
        i := i+1
```

The [integer division](../../../../../integer-division.md) identity gives a normalized remainder in $[0,base)$. The local rewrite preserves value because a carry at position $i+1$ contributes exactly what was removed at position $i$. The [loop invariant](../../../../../loop-invariant.md) is that the represented value is fixed and every position below `i` is normalized. Under the stated nonnegative-digit assumption all carries are nonnegative. Carries eventually stop beyond the finite radix expansion of the represented integer; scanning any spare allocated zeros then terminates.

This implementation also accepts signed temporary coefficients when their total represented value is nonnegative, using floor division rather than truncation toward zero. A negative carry out of the final position would make the entire represented value negative, since the already normalized lower part is smaller than the next radix power. Thus the assertion cannot fail for a nonnegative represented value. This extended [carry normalization of a digit array](../../../../../carry-normalization-of-a-digit-array.md) also makes the arithmetic routines below robust to such temporary representations.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
