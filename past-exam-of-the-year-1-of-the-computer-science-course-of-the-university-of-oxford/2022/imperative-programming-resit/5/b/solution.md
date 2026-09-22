<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use column heights and update the cached count by the number of removed cells:

```
class Chomps(N: Int) {
  require(N > 0 && N.toLong * N.toLong <= Int.MaxValue)
  private val height = Array.fill(N)(N)
  private var remaining = (N.toLong * N.toLong).toInt

  def Count(): Int = remaining

  def Legal(x: Int, y: Int): Boolean =
    0 <= x && x < N && 0 <= y && y < height(x)

  def Move(x: Int, y: Int): Unit = {
    require(Legal(x, y), "illegal move")
    var i = x
    while (i < N && height(i) > y) {
      remaining -= height(i) - y
      height(i) = y
      i += 1
    }
  }

  def Display(): Unit = {
    require(N < 10, "single-digit display labels required")
    var y = N - 1
    while (y >= 0) {
      print(y + "  ")
      var x = 0
      while (x < N) {
        print(if (y < height(x)) "* " else "  ")
        x += 1
      }
      println()
      y -= 1
    }
    print("   ")
    var x = 0
    while (x < N) { print(x + " "); x += 1 }
    println()
  }
}
```

The strengthened [representation invariant](../../../../../representation-invariant.md) includes $remaining=\sum_i h(i)$. The move loop's processed columns have their final truncated heights, unprocessed columns retain their old heights, and each subtraction removes exactly the corresponding height reduction. Because heights are nonincreasing, once a column is no higher than `y`, neither is any later column; stopping there is valid. A legal move removes at least one token and leaves a [order ideal](../../../../../order-ideal.md).

The constructor computes $N^2$ in `Long` and checks representability before converting, avoiding [integer overflow](../../../../../integer-overflow.md) in the cached `Int` count. `Legal` rejects out-of-range coordinates before indexing. The methods meet the bounds in part (a); `Display` additionally checks its stated single-digit-label assumption.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
