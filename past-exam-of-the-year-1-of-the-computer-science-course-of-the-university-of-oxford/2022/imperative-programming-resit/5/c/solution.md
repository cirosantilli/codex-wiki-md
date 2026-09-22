<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Retry invalid inputs without switching players; after a legal move, check whether the board has become empty:

```
val game = new Chomps(6)
var player = 1
while (game.Count() > 0) {
  game.Display()
  var accepted = false
  var x = 0
  var y = 0
  while (!accepted) {
    try {
      println("Player " + player + ": enter x, then y")
      x = scala.io.StdIn.readInt()
      y = scala.io.StdIn.readInt()
      accepted = game.Legal(x, y)
      if (!accepted) println("That cell is not a legal move; try again.")
    } catch {
      case _: NumberFormatException => println("Please enter integer coordinates.")
    }
  }
  game.Move(x, y)
  if (game.Count() == 0)
    println("Player " + player + " loses; player " + (3 - player) + " wins.")
  else player = 3 - player
}
```

Only a move at $(0,0)$ can remove the poisoned bottom-left token, and that move removes the entire remaining [order ideal](../../../../../order-ideal.md), so the empty-board test identifies the losing player correctly. Any other legal move preserves that token. Every accepted move strictly decreases the finite token count, giving at most 36 accepted moves. Invalid attempts do not change the board or the turn. As usual for this interactive fragment, the user is assumed eventually to supply another readable input rather than permanently ending the input stream or retrying forever.

## ↑ Ancestors (12)

1. [C](../c.md)
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
