<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the remainder form of the [Euclidean algorithm](../../../../../euclidean-algorithm.md) to compute the [greatest common divisor](../../../../../greatest-common-divisor.md), then divide both components of the [fraction](../../../../../fraction.md) by it:
```
def Reduce(num: Int, den: Int): (Int, Int) = {
  require(0 <= num && num < den)
  var a = den
  var b = num
  while (b != 0) {
    val r = a % b
    a = b
    b = r
  }
  (num / a, den / a)
}
```
The [loop invariant](../../../../../loop-invariant.md) is $a>0$, $b\geq0$, and $\gcd(a,b)=\gcd(den,num)$. Initially it holds by symmetry of the [greatest common divisor](../../../../../greatest-common-divisor.md). For $b>0$, the [integer division](../../../../../integer-division.md) identity $a=qb+r$, with $0\leq r<b$, shows that $a,b$ and $b,r$ have exactly the same common [integer divisors](../../../../../divisor.md). Thus the update preserves the [loop invariant](../../../../../loop-invariant.md). The [loop variant](../../../../../loop-variant.md) is the nonnegative [integer](../../../../../integer-split.md) $b$, which strictly decreases on each iteration. At exit $b=0$, so $a=\gcd(den,num)>0$. Dividing by $a$ preserves the [rational number](../../../../../rational-number.md) and makes the returned components [coprime](../../../../../coprime-integers.md). In particular, **zero is returned as $(0,1)$**. No multiplication is needed, and all remainders remain within the original nonnegative `Int` range.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
