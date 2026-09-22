<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the iterative [Euclidean algorithm](../../../../../euclidean-algorithm.md) for a nonnegative numerator and positive denominator:

```
function GCD(m,n): integer
    a := m
    b := n
    while b != 0 do
        r := a mod b
        a := b
        b := r
    return a

procedure Reduce(var m,n)
    require m >= 0 and n > 0
    d := GCD(m,n)
    m := m div d
    n := n div d
```

The [loop invariant](../../../../../loop-invariant.md) is $\gcd(a,b)=\gcd(m_0,n_0)$ with $a,b\geq0$. The nonnegative [loop variant](../../../../../loop-variant.md) is $b$: when positive, the new remainder is strictly smaller. Thus the final $a$ is the positive [greatest common divisor](../../../../../greatest-common-divisor.md). Dividing both numerator and denominator by it preserves the [rational number](../../../../../rational-number.md) and makes them [coprime](../../../../../coprime-integers.md). The stated [proper fraction](../../../../../proper-fraction.md) case is included, but the same code works for every nonnegative numerator, a fact useful in part (d). In particular, **zero reduces to $0/1$**.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
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
