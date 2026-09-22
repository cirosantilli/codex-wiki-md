<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the [product of finite probability distributions](../../../../../product-of-finite-probability-distributions.md), enumerate the [Cartesian product](../../../../../cartesian-product.md) of the two supports and multiply the two [probability masses](../../../../../probability-mass.md).
```
def product[T,U](d: FiniteDist[T], d2: FiniteDist[U]): FiniteDist[(T,U)] =
  new FiniteDist[(T,U)] {
    private val dom = for (x <- d.getDom; y <- d2.getDom) yield (x,y)
    def getDom: List[(T,U)] = dom
    def getProb(p: (T,U)): Double = d.getProb(p._1) * d2.getProb(p._2)
  }
```
Each pair appears once because both original supports have no duplicates. Exact [probabilities](../../../../../probability.md) are positive on that support, and normalization follows by finite distributivity:

$$
\sum_{x,y}p_1(x)p_2(y)=\left(\sum_xp_1(x)\right)\left(\sum_yp_2(y)\right)=1.
$$

For the [pushforward of a finite probability distribution](../../../../../pushforward-of-a-finite-probability-distribution.md), sum all masses in each [fiber of a function](../../../../../fiber-of-a-function.md); simply overwriting repeated image values would lose [probability](../../../../../probability.md).
```
def image[T,U](d: FiniteDist[T], f: T => U): FiniteDist[U] =
  new FiniteDist[U] {
    private val weighted = d.getDom.map(x => (f(x), d.getProb(x)))
    private val dom = weighted.map(_._1).distinct
    def getDom: List[U] = dom
    def getProb(y: U): Double =
      weighted.foldLeft(0.0) { case (total, (z,p)) =>
        if (z == y) total+p else total
      }
  }
```
Assume the given [finite probability distributions](../../../../../finite-probability-distribution.md) are fixed and `f` is a pure total [function](../../../../../function-split.md) on the source support. Distinct image values form exactly the positive-mass support. The [fibers](../../../../../fiber-of-a-function.md) partition the original support, proving

$$
\boxed{p_{\mathrm{product}}(x,y)=p_1(x)p_2(y),\qquad p_{\mathrm{image}}(z)=\sum_{x:f(x)=z}p_1(x),\qquad\sum_zp_{\mathrm{image}}(z)=1.}
$$

For example, sending a [discrete uniform distribution](../../../../../discrete-uniform-distribution.md) on $\{1,2,3,4\}$ to parity produces masses $1/2$ and $1/2$, not four distinct outcomes. Exact algebra establishes the [finite probability distribution](../../../../../finite-probability-distribution.md) laws; `Double` computes approximations, with the usual possibility of rounding and [floating-point underflow](../../../../../floating-point-underflow.md) for very small products.

## ↑ Ancestors (12)

1. [D](../d.md)
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
