<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Implement the three consumers directly with [while loops](../../../../../while-loop.md). These methods consume the receiver; `exists` stops immediately after the first witness:
```
trait RichIter[T] extends Iter[T] {
  def foreach(f: T => Unit): Unit = {
    while (hasNext) f(next())
  }

  def exists(p: T => Boolean): Boolean = {
    while (hasNext) {
      if (p(next())) return true
    }
    false
  }

  def foldLeft[U](x: U)(f: (U, T) => U): U = {
    var result = x
    while (hasNext) result = f(result, next())
    result
  }
}
```
For `foreach`, the [loop invariant](../../../../../loop-invariant.md) is that `f` has been called once, in order, on exactly the consumed prefix. For `exists`, provided it has not returned, every consumed entry fails the [predicate](../../../../../predicate.md); a returned `true` has a witness, while exhaustion proves there is none. For `foldLeft`, after $j$ consumed entries the [loop invariant](../../../../../loop-invariant.md) is

$$
\mathrm{result}=f(\cdots f(f(x,a_1),a_2)\cdots,a_j),
$$

with `result = x` at $j=0$. Thus initialization, one further application, and exhaustion prove the required [left fold](../../../../../left-fold.md). On finite inputs, the remaining length is a [loop variant](../../../../../loop-variant.md) for each loop. Callbacks are assumed not to mutate this [iterator](../../../../../iterator.md) independently.

$$
\boxed{\operatorname{foreach}:\text{ordered consumption};\quad\operatorname{exists}:\text{short-circuit search};\quad\operatorname{foldLeft}:\text{left-associated accumulation}.}
$$

With constant-cost callbacks and [iterator](../../../../../iterator.md) operations, full consumption costs $\Theta(n+1)$; `exists` may return earlier. Empty inputs respectively do nothing, return `false`, and return `x`. Infinite inputs need not terminate, except that `exists` terminates upon reaching a witness.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
