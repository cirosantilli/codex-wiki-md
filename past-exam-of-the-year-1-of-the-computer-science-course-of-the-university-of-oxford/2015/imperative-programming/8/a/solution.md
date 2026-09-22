<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For `Uniform`, require a nonempty [integer interval](../../../../../integer-interval.md). Compute its size in `Long` before converting to `Double`, avoiding [integer overflow](../../../../../integer-overflow.md) in `u-l+1`. For `Flip`, require $0\leq p\leq1$, and omit zero-[probability](../../../../../probability.md) outcomes from the reported support.
```
class Uniform(l: Int, u: Int) extends FiniteDist[Int] {
  require(l <= u)
  private val size = u.toLong - l.toLong + 1L
  def getDom: List[Int] = {
    val result = List.newBuilder[Int]
    var x = l.toLong
    while (x <= u.toLong) { result += x.toInt; x += 1L }
    result.result()
  }
  def getProb(x: Int): Double =
    if (l <= x && x <= u) 1.0 / size.toDouble else 0.0
}

class Flip(p: Double) extends FiniteDist[Boolean] {
  require(0.0 <= p && p <= 1.0)
  def getDom: List[Boolean] =
    if (p == 0.0) List(false)
    else if (p == 1.0) List(true)
    else List(true, false)
  def getProb(x: Boolean): Double = if (x) p else 1.0-p
}
```
The first is a [discrete uniform distribution](../../../../../discrete-uniform-distribution.md); the second is a [Bernoulli distribution](../../../../../bernoulli-distribution.md) on [Boolean](../../../../../boolean-data-type.md) values. Their exact mathematical [probability mass functions](../../../../../probability-mass-function.md) are

$$
\boxed{p_U(x)=\begin{cases}\dfrac1{u-l+1}&l\leq x\leq u,\\0&\text{otherwise},\end{cases}\qquad p_F(\mathrm{true})=p,\quad p_F(\mathrm{false})=1-p.}
$$

Each support contains exactly the positive-[probability](../../../../../probability.md) outcomes once, and the [probabilities](../../../../../probability.md) sum to one. `Double` approximates these exact values by [floating-point arithmetic](../../../../../floating-point-arithmetic-split.md). Materializing a huge support is limited by available memory; the `Long` calculation keeps its cardinality and endpoints arithmetically correct.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
