<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Each `play` call should make at most one hit and return `true` exactly when it did so; the supplied `while` loop invokes it again to decide whether another hit is needed. Add these accessors inside `Player`:
```
def cards: List[Int] = _cards
def cards_=(cs: List[Int]): Unit = { _cards = cs }
def visibleValue: Int = _visibleValue
def visibleValue_=(v: Int): Unit = { _visibleValue = v }
```
The [Scala](../../../../../scala.md) assignment `temp.cards = cs` calls the setter, and `visibleValue += cards.head` uses the getter followed by the setter. The [list](../../../../../list-abstract-data-type.md) getter exposes an immutable list value; updating the player's field still goes through the setter. The supplied initialization and `hit` maintain the hidden card at the last list position and `visibleValue == cards.init.sum` for each nonempty dealt hand.

The concrete [software classes](../../../../../class-programming.md) implement the supplied strategies literally:
```
class Regular extends Player {
  def play(visibleCards: List[Int]): Boolean = {
    require(visibleCards.length == 1)
    val total = value
    if (total < 21 && total <= 21 - visibleCards.head) {
      hit
      true
    } else false
  }
}

class Optimistic extends Player {
  def play(visibleCards: List[Int]): Boolean = {
    if (value != 21) {
      hit
      true
    } else false
  }
}

class House extends Player {
  def play(visibleCards: List[Int]): Boolean = {
    val total = value
    if (total < 21 && visibleCards.forall(v => total <= 21 - v)) {
      hit
      true
    } else false
  }
}
```
`House` receives all other players' final visible totals, whereas a non-house player receives the singleton containing the house's first visible card. The universal test implements “for each other player,” including the vacuously true case of no other players. [Subtype polymorphism](../../../../../subtype-polymorphism.md) gives the common player [list](../../../../../list-abstract-data-type.md) a `Player` interface, and [dynamic dispatch](../../../../../dynamic-dispatch.md) chooses the appropriate `play` implementation.

**These are the literal missing methods, but the printed specification does not guarantee a terminating game.** An optimistic player with total $20$ who draws $2$ reaches $22$; every further positive card keeps the total above $21$, so `value != 21` remains true. The claim that only finitely many further cards are requested is therefore inconsistent with the optimistic strategy on such executions, in the intended arithmetic model without overflow. If the intended rule is “stop on reaching or exceeding 21,” the necessary correction is to replace its test by `value < 21`; that changes the printed strategy and is not silently made here.

There is a second printed mismatch: `nextInt(10)` yields $0,\ldots,9$, so `1 + nextInt(10)` yields **$1,\ldots,10$**, not $1,\ldots,11$. Preserve the supplied `hit` when filling its missing pieces; generating every value from $1$ through $11$ would require an explicit change to `nextInt(11)` in both dealing and hitting.[Scala 2.11.12 Random.nextInt, upper bound is exclusive](https://www.scala-lang.org/api/2.11.12/scala/util/Random.html#nextInt(n:Int):Int) No winner-computation code is requested; the supplied loop only deals and requests cards.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
