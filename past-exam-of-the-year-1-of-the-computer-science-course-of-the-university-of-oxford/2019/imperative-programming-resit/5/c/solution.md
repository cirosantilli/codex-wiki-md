<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep the same player until an occupied, in-range cell is supplied:
```
val board = new Chomps(6)
var player = 1
while (board.Count() > 0) {
  board.Display()
  var x = -1
  var y = -1
  while (!board.Legal(x, y)) {
    println("Player " + player + ": enter x, then y")
    try {
      x = scala.io.StdIn.readInt()
      y = scala.io.StdIn.readInt()
    } catch {
      case _: NumberFormatException =>
        x = -1
        y = -1
    }
    if (!board.Legal(x, y)) println("Choose an occupied cell")
  }
  board.Move(x, y)
  if (board.Count() == 0)
    println("Player " + player + " loses; player " + (3 - player) + " wins")
  else player = 3 - player
}
```
The outer [loop invariant](../../../../../loop-invariant.md) is that `player` is the next player's number, either one or two, and the board is the result of the accepted moves. The inner [loop invariant](../../../../../loop-invariant.md) says that the board and player have not changed; rejected inputs do not consume a turn. Assuming the input source continues and eventually supplies a legal coordinate pair, the inner loop finishes. No program can guarantee that a user stops entering illegal moves, so that interaction assumption is necessary.

Every accepted move removes at least its selected token, so the outer [loop variant](../../../../../loop-variant.md) is `Count()`, a decreasing nonnegative [integer](../../../../../integer-split.md). In a nonempty [order ideal](../../../../../order-ideal.md), $(0,0)$ is occupied. Removing it removes the entire board, whereas a move at any other cell leaves it. Therefore **the player making the final move is exactly the loser**; the code reports that player before changing the turn. At most $36$ legal moves occur.

## ↑ Ancestors (12)

1. [C](../c.md)
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
