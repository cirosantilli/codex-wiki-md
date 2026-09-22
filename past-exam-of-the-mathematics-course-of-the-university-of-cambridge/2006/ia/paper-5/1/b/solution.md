<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [Standard ML](../../../../../../standard-ml.md) length function visits each list constructor once:
```
sml
fun length [] = 0
  | length (_ :: xs) = 1 + length xs;
```
Writing $T(n)$ for its [time complexity](../../../../../../time-complexity.md), $T(n)=T(n-1)+\Theta(1)$ and $T(0)=\Theta(1)$. Thus **$T(n)=\Theta(n)$**. Arithmetic is treated as unit cost; the example concerns list traversal rather than arbitrary-precision arithmetic.

## ↑ Ancestors (11)

1. [B](../b.md)
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
