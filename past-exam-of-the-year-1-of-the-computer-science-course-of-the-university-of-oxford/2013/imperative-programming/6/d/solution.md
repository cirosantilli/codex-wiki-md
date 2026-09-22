<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Keep the neighboring [Fibonacci number](../../../../../fibonacci-number.md) in a private [closure](../../../../../closure-topology.md). Before calling the transition with $x=F_n$, let its captured `following` equal $F_{n+1}$.
```
def fibonacci(): Iter[BigInt] = {
  var following = BigInt(1)
  val step: BigInt => BigInt = (x: BigInt) => {
    val result = following
    following = x + following
    result
  }
  new FunIter[BigInt](BigInt(0), step)
}
```
The transition returns $F_{n+1}$ and stores $F_n+F_{n+1}=F_{n+2}$, preserving the [paired Fibonacci recurrence](../../../../../paired-fibonacci-recurrence.md). Initialization gives $F_0=0$ and $F_1=1$, so

$$
\boxed{0,1,1,2,3,5,8,13,21,\ldots.}
$$

Using `BigInt` allows all [Fibonacci numbers](../../../../../fibonacci-number.md) rather than a finite prefix before [integer overflow](../../../../../integer-overflow.md). Replacing `BigInt` by `Int` gives the source's suggested machine-[integer](../../../../../integer-split.md) interface with that limitation. With the `FunIter` implementation from part (c), each transition runs once per generated cell, and copied [iterators](../../../../../iterator.md) can advance independently while sharing the privately owned generator. A simpler alternative uses a [pure function](../../../../../pure-function.md) on pairs, $(a,b)\mapsto(b,a+b)$, and projects the first component; the [closure](../../../../../closure-topology.md) above follows the source's suggested single-value approach directly.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
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
