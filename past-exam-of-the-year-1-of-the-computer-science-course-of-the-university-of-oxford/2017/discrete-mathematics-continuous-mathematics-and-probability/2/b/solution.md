<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For integers $a,b$ not both zero, replace them first by their [absolute values](../../../../../absolute-value.md), then repeat [integer division](../../../../../integer-division.md):

```
while b != 0:
    (a,b) := (b, a mod b)
return a
```

This is the [Euclidean algorithm](../../../../../euclidean-algorithm.md). Its [loop invariant](../../../../../loop-invariant.md) is that $\gcd(a,b)$ equals the original [greatest common divisor](../../../../../greatest-common-divisor.md). When $b>0$, the new remainder lies in $[0,b)$, so $b$ is a strictly decreasing nonnegative [loop variant](../../../../../loop-variant.md). At termination, $\gcd(a,0)=a$, proving correctness, including the case where one original input is zero.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
