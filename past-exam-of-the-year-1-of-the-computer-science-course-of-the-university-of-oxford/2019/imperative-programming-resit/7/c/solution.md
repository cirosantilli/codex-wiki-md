<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Add the following concrete method inside `FiniteDist[T]`. It forms a [pushforward of a finite probability distribution](../../../../../pushforward-of-a-finite-probability-distribution.md), adding the masses of outcomes that map to the same result:
```
def map[U](f: T => U): FiniteDist[U] = {
  val source = getDom
  val weighted = source.map(x => (f(x), getProb(x)))
  val target = weighted.map(_._1).distinct
  new FiniteDist[U] {
    def getDom: List[U] = target
    def getProb(y: U): Double =
      weighted.filter(pair => pair._1 == y).map(_._2).sum
  }
}
```
The input [finite probability distribution](../../../../../finite-probability-distribution.md) is assumed to satisfy its interface, with stable masses during construction, and `f` must be a total deterministic [pure function](../../../../../pure-function.md) on its finite support. Output values need stable equality consistent with the mathematical equality being modeled; mutating equality-relevant fields afterwards would undermine any finite-support implementation. Computing `weighted` once also prevents later queries from re-evaluating `f` inconsistently.

Every source support element appears once in `weighted`. The `distinct` operation lists each image value once; every such image has a positive mathematical mass because it has a positive-mass preimage. For each $y$, filtering selects exactly those $x$ with $f(x)=y$, so `getProb(y)` is the required sum, with an empty sum of zero off the image. The fibers form a [set partition](../../../../../set-partition.md) of the original support, giving

$$
\sum_y p_2(y)=\sum_y\sum_{x:f(x)=y}p_1(x)=\sum_xp_1(x)=1.
$$

Thus **colliding images have their probabilities added, not overwritten**. For a concrete check, mapping a uniform distribution on $\{0,1,2,3\}$ by parity gives probability $1/2$ to each of $0,1$; mapping every source value to one constant gives a singleton domain with total mass one. [Floating-point rounding](../../../../../floating-point-rounding.md) can make a computed total differ slightly from one; the proof is for exact mathematical masses, and the representation uses `Double` approximations.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
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
