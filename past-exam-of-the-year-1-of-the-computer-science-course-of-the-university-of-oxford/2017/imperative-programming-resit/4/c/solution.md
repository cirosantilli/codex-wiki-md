<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a helper whose first argument is a private result list. It adds a coefficient to an existing power, deleting a cancellation, or allocates a new node:

```
accumulate(VAR r: poly; c: T; e: INTEGER):
    if c == 0: return
    p = r; prev = NIL
    while p != NIL and p.power != e:
        prev = p; p = p.next
    if p == NIL:
        q = new term(c,e,r)
        r = q
    else:
        p.coeff = p.coeff+c
        if p.coeff == 0:
            if prev == NIL: r = p.next
            else: prev.next = p.next

addPoly(x,y):
    r = NIL
    p = x
    while p != NIL:
        accumulate(r,p.coeff,p.power)
        p = p.next
    p = y
    while p != NIL:
        accumulate(r,p.coeff,p.power)
        p = p.next
    return r
```

Here `VAR` applies to the list variable `r`; coefficients and powers are value arguments. The helper preserves one node per power and excludes zero coefficients. After each loop iteration, the result represents exactly the processed input terms. Every result node is fresh, so neither input's nodes or links are changed, even if the two inputs alias or share tails. For unsorted inputs of lengths $m,n$, a simple worst-case bound is $O((m+n)^2)$ for these repeated scans.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
