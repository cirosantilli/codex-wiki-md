<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Normalize the amount to $r=k\bmod N$, with $0\leq r<N$; negative $k$ then naturally denotes a right rotation. When $r=0$, return without touching the elements. Otherwise the map $j\mapsto(j+r)\bmod N$ has $g=\gcd(N,r)$ disjoint [permutation cycles](../../../../../permutation-cycle.md), each of length $N/g$. Use representatives $0,\ldots,g-1$:
```
PROCEDURE RotateLeft(k: INTEGER);
VAR r, g, x, y, h, s, j, next: INTEGER; saved: T;
BEGIN
  r := k MOD N;
  IF r # 0 THEN
    x := N; y := r;
    WHILE y # 0 DO h := x MOD y; x := y; y := h END;
    g := x; s := 0;
    WHILE s < g DO
      saved := a[s]; j := s;
      IF j >= N-r THEN next := j-(N-r) ELSE next := j+r END;
      WHILE next # s DO
        a[j] := a[next]; j := next;
        IF j >= N-r THEN next := j-(N-r) ELSE next := j+r END
      END;
      a[j] := saved; s := s+1
    END
  END
END RotateLeft;
```
The conditional calculation of `next` implements addition modulo $N$ without first forming a possibly overflowing `j+r`. [Oberon](../../../../../oberon-programming-language.md)'s `MOD` with positive divisor supplies the nonnegative remainder. The first loop is the [Euclidean algorithm](../../../../../euclidean-algorithm.md), with [loop invariant](../../../../../loop-invariant.md) $\gcd(x,y)=\gcd(N,r)$ and decreasing nonzero remainder.

For the outer loop, cycles with representatives below `s` are complete and every other cycle retains its original values. In one cycle, write $c_t=(s+tr)\bmod N$. The inner [loop invariant](../../../../../loop-invariant.md) is `saved = A[s]`, $j=c_t$, and $a[c_u]=A[c_{u+1}]$ for $0\leq u<t$, with the remaining sources still untouched. When the next index returns to `s`, the saved value closes the cycle. The cycle length is $N/g$: writing $N=gN'$ and $r=gr'$ with $\gcd(N',r')=1$, the least positive $t$ with $tr\equiv0\pmod N$ is $N'$. Each residue class modulo $g$ is one cycle, justifying the chosen representatives.

**Every element is read once and written once: $2N$ element accesses**, compared with $2Nk$ for $k>1$ repetitions of part (b). The zero rotation uses none. The [running time](../../../../../running-time.md) is $O(N)$ and auxiliary space is constant; the original [array](../../../../../array-data-structure.md) $A$ is proof notation, not a copy made by the program.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
