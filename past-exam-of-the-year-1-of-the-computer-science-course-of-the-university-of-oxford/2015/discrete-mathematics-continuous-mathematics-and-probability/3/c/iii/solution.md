<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $(a_0,b_0)=(a,b)$. At each iteration with $b_i>0$, compute the [remainder](../../../../../../remainder.md) $r_i=a_i\bmod b_i$, then set

$$
\boxed{(a_{i+1},b_{i+1})=(b_i,r_i).}
$$

Stop at the first index $n$ with $b_n=0$ and return $a_n$. The positive second coordinates strictly decrease, so [algorithm termination](../../../../../../algorithm-termination.md) follows from the [well-ordering principle](../../../../../../well-ordering-principle-for-the-natural-numbers.md). The equality of [greatest common divisors](../../../../../../greatest-common-divisor.md) established in (ii) is a [loop invariant](../../../../../../loop-invariant.md), and at termination it gives

$$
\boxed{a_n=\gcd(a_n,0)=\gcd(a,b).}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
