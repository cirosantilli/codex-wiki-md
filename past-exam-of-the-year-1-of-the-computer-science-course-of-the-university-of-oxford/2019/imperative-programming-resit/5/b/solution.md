<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the row boundary and cache its sum. The restriction on the initial total makes the fixed `Int` return type of `Count` meaningful; `Display` separately checks the requested single-digit coordinate range.
```
class Chomps(N: Int) {
  require(N > 0 && N.toLong * N.toLong <= Int.MaxValue.toLong)
  private val row = Array.fill(N)(N)
  private var remaining = N * N

  def Count(): Int = remaining

  def Legal(x: Int, y: Int): Boolean =
    0 <= x && x < N && 0 <= y && y < N && x < row(y)

  def Move(x: Int, y: Int): Unit = {
    require(Legal(x, y))
    var j = y
    while (j < N) {
      val next = math.min(row(j), x)
      remaining -= row(j) - next
      row(j) = next
      j += 1
    }
  }

  def Display(): Unit = {
    require(N < 10)
    var y = N - 1
    while (y >= 0) {
      print(y.toString + " ")
      var x = 0
      while (x < N) {
        print(if (x < row(y)) "* " else "  ")
        x += 1
      }
      println()
      y -= 1
    }
    print("  ")
    var x = 0
    while (x < N) {
      print(x.toString + " ")
      x += 1
    }
    println()
  }
}
```
The additional [representation invariant](../../../../../representation-invariant.md) is $remaining=\sum_{j=0}^{N-1}row(j)$. It initially holds. For `Move`, write $row_0$ for the boundary at entry. The [loop invariant](../../../../../loop-invariant.md) says that rows before $y$ are unchanged, rows from $y$ through $j-1$ equal $\min(row_0(i),x)$, rows from $j$ onwards still equal $row_0(i)$, and `remaining` equals the sum of the current entries. The [loop variant](../../../../../loop-variant.md) is $N-j$. Each iteration subtracts exactly the newly removed number of cells from the cache. At exit all affected rows are truncated as required, and the nonincreasing boundary is restored. During a partially completed update it need not be nonincreasing; only the stated [loop invariant](../../../../../loop-invariant.md), not the full externally visible [representation invariant](../../../../../representation-invariant.md), is required internally.

For `Display`, the outer [loop invariant](../../../../../loop-invariant.md) says that exactly the rows with indices greater than $y$ have been printed correctly; its [loop variant](../../../../../loop-variant.md) is $y+1$. The inner [loop invariant](../../../../../loop-invariant.md) says that the current row's first $x$ cells have been emitted correctly; its [loop variant](../../../../../loop-variant.md) is $N-x$. The final labels loop has the same decreasing [loop variant](../../../../../loop-variant.md), and prints exactly the first $x$ column labels before each iteration. [Short-circuit evaluation](../../../../../short-circuit-evaluation.md) in `Legal` checks both coordinates before indexing. **An illegal `Move` fails before changing the board.**

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
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
