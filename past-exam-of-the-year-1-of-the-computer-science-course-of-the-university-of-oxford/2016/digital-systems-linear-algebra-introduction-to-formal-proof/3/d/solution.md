<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The blanks are **`x < 2`** and **`return x - foo(x + 1)`**. The compiled `slti` and `bne` select the first branch exactly for $x<2$. Otherwise `addi` forms $x+1$, `jal foo` returns its value in `$v0`, and `sub $v0, $s0, $v0` subtracts that value from the preserved $x$. Thus the complete high-level implementation is
```
proc bar(val x : int) : int
begin if x < 2 then
          return 1
      else
          return x - foo(x + 1)
      end
end
```
Although the immediate call increases the argument, substitution into `foo`'s two recursive calls decreases the corresponding `bar` arguments to $x-1$ and $x-2$ whenever the recursive branch is entered. The mutual [recursion](../../../../../recursion-computer-science.md) therefore terminates on ordinary integer inputs, assuming sufficient [stack](../../../../../stack-data-structure.md) space and no machine arithmetic overflow.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
