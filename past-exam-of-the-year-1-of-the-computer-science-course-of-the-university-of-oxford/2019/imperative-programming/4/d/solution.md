<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [breadth-first search](../../../../../breadth-first-search.md) with the supplied [FIFO queue](../../../../../fifo-queue.md), taking one edge to mean one permitted [prefix reversal](../../../../../prefix-reversal.md):
```
def solve(puzzle: Flip): Flip = {
  val pending = scala.collection.mutable.Queue[Flip]()
  pending.enqueue(puzzle)
  while (!pending.isEmpty) {
    val current = pending.dequeue()
    if (current.isIdentity) return current
    var k = 2L
    while (k <= current.game.length.toLong) {
      pending.enqueue(current.flip(k.toInt))
      k += 1L
    }
  }
  throw new IllegalStateException("No solution")
}

val puzzle = new Flip(n)
println("Solving:")
println(puzzle)
val answer = solve(puzzle)
println("Solved:")
println(answer)
```
The [FIFO queue](../../../../../fifo-queue.md) holds pending paths in nondecreasing history length. Initially it holds only the zero-move path. Removing a path at depth $d$ and appending its children at depth $d+1$ preserves that order. The inner [loop invariant](../../../../../loop-invariant.md) says that precisely moves $2,\ldots,k-1$ of the removed state have been appended; its [loop variant](../../../../../loop-variant.md) is $n-k+1$ while the guard holds. The first identity state removed therefore has **the minimum possible number of moves**. A [stack](../../../../../stack-data-structure.md)-based [depth-first search](../../../../../depth-first-search.md) does not generally have that property.

Termination does not rely on avoiding repeats in this first version. Every [permutation](../../../../../permutation.md) can be sorted by [prefix reversal sorting](../../../../../prefix-reversal-sorting.md): place the largest misplaced value at the front if necessary, flip it into its final position, and repeat on the shorter prefix. This constructs a route of at most $2(n-1)$ moves. Each search depth has finitely many paths, with at most $n-1$ children per path, so [breadth-first search](../../../../../breadth-first-search.md) reaches some solution depth after finitely many expansions. This gives a finite bound on remaining expansions before the first solution even though the repeated-state path tree is infinite. The one-element game is already solved. Repeated paths can nevertheless make time and storage enormous; part (e) removes that waste.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
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
