<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Represent the characteristic values of a bounded universe by one Boolean slot per possible member, a Boolean-[array](../../../../../array-data-structure.md) form of a [bitset](../../../../../bitset.md):
```
class BitMapSet(val MAXVALUE: Int) extends IntSet {
  require(MAXVALUE >= 0)
  private val bits = Array.fill(MAXVALUE)(false)
  private var count = 0

  def contains(elem: Int): Boolean =
    0 <= elem && elem < MAXVALUE && bits(elem)

  def add(elem: Int): Boolean = {
    require(0 <= elem && elem < MAXVALUE, "Outside bitmap universe")
    if (bits(elem)) false
    else {
      bits(elem) = true
      count += 1
      true
    }
  }

  def size: Int = count
}
```
The [abstraction function](../../../../../abstraction-function.md) is $\alpha(bits,count)=\{x:0\leq x<MAXVALUE,\ bits(x)\}$. The [representation invariant](../../../../../representation-invariant.md) is that `bits.length==MAXVALUE`, its entries are Boolean, and `count` equals the number of true entries. Initialization gives the empty [set](../../../../../set-split.md); changing a false entry to true adds exactly its index and increments the count once. A repeated addition preserves both. All three operations have $O(1)$ [time complexity](../../../../../time-complexity.md) after initialization; storage and explicit [array](../../../../../array-data-structure.md) initialization are $\Theta(MAXVALUE)$.

**The constructor requires $MAXVALUE\geq0$, and `add` requires $0\leq elem<MAXVALUE$.** `contains` remains total by returning false outside the representable universe; [short-circuit evaluation](../../../../../short-circuit-evaluation.md) protects the index. This finite representation cannot implement unrestricted addition of every `Int` while preserving the abstract contract. Its strengthened `add` [precondition](../../../../../precondition.md) therefore makes it a restricted implementation, not a behaviorally substitutable implementation of the unrestricted trait for arbitrary clients. The [sequence](../../../../../sequence.md) client below proves that it stays within the restricted universe.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
