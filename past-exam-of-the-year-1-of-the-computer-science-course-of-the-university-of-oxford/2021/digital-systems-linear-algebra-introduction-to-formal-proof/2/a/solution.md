<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The shifts multiply the original [array](../../../../../array-data-structure.md) indices by four, and the following additions form [byte](../../../../../byte.md) [memory addresses](../../../../../memory-address.md). The load into `$s0` changes the variable $x$ itself, but the address of the next element of A has already been saved. The complete effect is

```
i = x
x = A[i]
B[y] = x + A[i + 1]
```

Here `i` is a fresh temporary. **Both the assignment to $x$ and the assignment to $B[y]$ matter.** Writing only $B[y]=A[x]+A[x+1]$ would omit the observable change to $x$. The interpretation assumes four-[byte](../../../../../byte.md) [array](../../../../../array-data-structure.md) elements, valid aligned addresses, and arithmetic within range; the source uses trapping signed additions. The address of $B[y]$ is computed before $x$ changes.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
