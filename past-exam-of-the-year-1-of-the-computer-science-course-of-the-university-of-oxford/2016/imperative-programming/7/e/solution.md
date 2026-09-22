<h1 id="7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use a [Scala](../../../../../scala.md) `object` for the [singleton pattern](../../../../../singleton-pattern.md), and replace `Performance` with a version that reports to it. This code plugs into the source's `Equipment`, `GymEquipment`, and `Functionality` definitions; `Prediction` can remain an independent observer once its displayed string line break is made executable.
```
object GymStandings {
  private var scores = Map.empty[GymEquipment, Int]

  def record(e: GymEquipment, calories: Int): Unit = {
    scores = scores.updated(e, calories)
  }

  def remove(e: GymEquipment): Unit = {
    scores = scores - e
  }

  def leaders: List[(GymEquipment, Int)] = {
    if (scores.isEmpty) Nil
    else {
      val best = scores.values.max
      scores.toList.filter { case (_, score) => score == best }
        .sortBy { case (equipment, _) => equipment.name }
    }
  }
}

class Performance(e: GymEquipment) extends Functionality {
  private def calories: Int =
    ((e.age - e.weight + e.heartRate) * e.time) / 10

  e.addFunctionality(this)
  GymStandings.record(e, calories)

  def update(): Unit = {
    val current = calories
    GymStandings.record(e, current)
    println("Your current performance is: " + current + " calories burned.")
  }
}
```
For example, `new Performance(treadmill)` and `new Performance(bike)` attach two observers; later `GymStandings.leaders` returns the leading equipment/score pairs. Initial registration records the equipment's present score, even before its first subsequent update. Recording replaces the same equipment's previous score, so repeated notifications do not multiply its contribution. The explicit `remove` supports taking an equipment object out of the comparison; detaching its observer when its session ends also prevents later re-registration through another notification. In the original single-threaded event model no extra synchronization is needed.

**All equipment observers report to the same standings [software object](../../../../../software-object.md), and `leaders` returns every maximum or `Nil` if empty.** The query takes $O(s)$ to find/filter scores for $s$ active equipment objects, plus sorting the tied names for deterministic presentation by name; equal names may remain in either order and still denote distinct equipment. This uses the exact supplied [integer](../../../../../integer-split.md) score formula and its [integer division](../../../../../integer-division.md); it does not substitute a different performance metric. A functioning unsubscribe operation, if required, must explicitly correct the source to `_functionalities = _functionalities diff List(f)`.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [7](../../7.md)
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
