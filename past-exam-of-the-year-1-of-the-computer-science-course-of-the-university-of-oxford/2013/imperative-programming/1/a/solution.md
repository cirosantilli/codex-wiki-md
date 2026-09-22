<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Evaluate the [mixed radix](../../../../../mixed-radix.md) representation from its most significant end, using [Horner's method](../../../../../horner-s-method.md). There is no need to compute the positional weights separately.
```
def digsToInt(xs: Array[Int], bs: Array[Int]): Int = {
  require(xs.length == bs.length)
  val N = xs.length
  var i = N
  var acc = 0
  while (i > 0) {
    i -= 1
    acc = xs(i) + bs(i) * acc
  }
  acc
}
```
The digit conditions $0\leq xs(i)<bs(i)$ are additional [preconditions](../../../../../precondition.md). The [loop invariant](../../../../../loop-invariant.md) at the loop test is

$$
0\leq i\leq N,\qquad
acc=\sum_{k=i}^{N-1}xs(k)\prod_{j=i}^{k-1}bs(j).
$$

An empty [sum](../../../../../sum.md) is zero and an empty [product](../../../../../product-of-numbers.md) is one, so initialization at $i=N$ is correct. For the next digit, writing $i'=i-1$ gives

$$
xs(i')+bs(i')acc
=\sum_{k=i'}^{N-1}xs(k)\prod_{j=i'}^{k-1}bs(j),
$$

which preserves the [loop invariant](../../../../../loop-invariant.md). The [loop variant](../../../../../loop-variant.md) is $i$. At termination $i=0$, giving

$$
\boxed{acc=xs\otimes bs.}
$$

The code executes exactly $N$ multiplications, meeting the bound, and uses $O(1)$ [auxiliary space](../../../../../auxiliary-space.md). When $N=0$ it returns zero. For the time representation in the source, it computes $s+60(m+60h)$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
