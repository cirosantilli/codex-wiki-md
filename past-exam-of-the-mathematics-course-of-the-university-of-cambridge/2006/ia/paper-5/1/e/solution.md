<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For a nonnegative integer parameter $n$, make both branches of a [structural recursion](../../../../../../structural-recursion.md) execute:
```
sml
fun binaryWalk 0 = ()
  | binaryWalk n = (binaryWalk (n - 1); binaryWalk (n - 1));
```
The semicolon sequences two calls, so this is not a conditional choosing just one branch. The recursion tree has $2^n$ leaves and $2^{n+1}-1$ calls. Its [time complexity](../../../../../../time-complexity.md) satisfies $T(n)=2T(n-1)+\Theta(1)$, giving **$\Theta(2^n)$**. Here $n$ is the parameter specified by the question, not its binary encoding length; only $\Theta(n)$ calls are simultaneously on the stack.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
