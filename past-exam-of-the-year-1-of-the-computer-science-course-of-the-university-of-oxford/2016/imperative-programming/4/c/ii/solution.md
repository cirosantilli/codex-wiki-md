<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $a=n-k$ and $b=k$ be the lengths of the left and right blocks. Exchange the smaller block with the equally long block at the opposite end.
```
PROCEDURE rotate(i, n, k: INTEGER);
VAR a, b: INTEGER;
BEGIN
  IF (k = 0) OR (k = n) THEN RETURN END;
  a := n-k; b := k;
  IF a = b THEN
    blockswap(i, i+a, a)
  ELSIF a < b THEN
    blockswap(i, i+b, a);
    rotate(i, b, b-a)
  ELSE
    blockswap(i, i+a, b);
    rotate(i+b, a, b)
  END
END rotate;
```
If $a<b$, split $B=B_1B_2$ with $|B_2|=a$. The first [block swap](../../../../../../block-swap.md) sends $AB_1B_2$ to $B_2B_1A$; $A$ is now in its final suffix. Rotate the remaining prefix of length $b$ right by $b-a$ to send $B_2B_1$ to $B_1B_2$. If $a>b$, split $A=A_1A_2$ with $|A_1|=b$. The swap sends $A_1A_2B$ to $BA_2A_1$; the fixed prefix is $B$, and rotating the remaining length-$a$ suffix right by $b$ restores $A_1A_2$. In both cases the exchanged segments are disjoint.

The remaining length strictly decreases, so [induction](../../../../../../mathematical-induction.md) on $n$ proves [algorithm termination](../../../../../../algorithm-termination.md) and correctness. **This implements the block-exchange rotation.** It uses only simple explicit variables, but its recursive call stack can have $\Theta(n)$ depth when one block has length $1$; the iterative version removes that extra storage.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
