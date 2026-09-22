<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a deterministic editing policy: editing pounds or the exchange rate preserves the pounds amount and recalculates euros; editing euros preserves the rate and recalculates pounds. A valid rate must be finite and positive; amounts may be any finite signed number. Keep an unrounded numeric model, so repeatedly refreshing a two-decimal display does not feed rounded text back into the computation. Place the following members inside the supplied `MainFrame`, after its fields are created:
```
private var poundsValue = 10.0
private var eurosValue = 11.5
private var rateValue = 1.15
private var refreshing = false

private def finite(x: Double): Boolean =
  !java.lang.Double.isNaN(x) && !java.lang.Double.isInfinite(x)

private def number(s: String): Option[Double] =
  scala.util.Try(s.trim.toDouble).toOption.filter(finite)

private def money(x: Double): String =
  java.lang.String.format(java.util.Locale.ROOT, "%.2f",
                          java.lang.Double.valueOf(x))

private def refresh(): Unit = {
  refreshing = true
  try {
    pounds.text = money(poundsValue)
    euros.text = money(eurosValue)
    rate.text = money(rateValue)
  } finally {
    refreshing = false
  }
}

private def commit(p: Double, e: Double, r: Double): Unit = {
  if (finite(p) && finite(e) && finite(r) && r > 0.0) {
    poundsValue = p
    eurosValue = e
    rateValue = r
    refresh()
  }
}

listenTo(pounds, euros, rate)
reactions += {
  case EditDone(source) if !refreshing =>
    number(source.text).foreach { value =>
      if (source eq pounds)
        commit(value, value * rateValue, rateValue)
      else if (source eq euros)
        commit(value / rateValue, value, rateValue)
      else if ((source eq rate) && value > 0.0)
        commit(poundsValue, poundsValue * value, value)
    }
}
```
The mathematical model [invariant](../../../../../invariant-mathematics.md) is $eurosValue=poundsValue\,rateValue$ with a positive rate. In [floating-point arithmetic](../../../../../floating-point-arithmetic-split.md), each update establishes the corresponding rounded multiplication or division; a division followed by multiplication need not recover bitwise identical values. Pounds and rate edits calculate a matching euro amount, while euro edits calculate its matching pound amount. An invalid parse, a nonpositive rate, or a nonfinite calculated result leaves the last valid numeric model unchanged. An invalid text entry may remain visible until corrected or a subsequent valid refresh; a production interface could add a validation message.

Every accepted edit refreshes the fields from that model. `Locale.ROOT` makes the decimal separator match the `toDouble` parser, independently of the machine's locale. The guard prevents a synchronous [reentrant event handler](../../../../../reentrant-event-handler.md) from interpreting a refresh as another user commit. The displayed values are rounded to two decimal places, including the rate, while the stored values retain full `Double` precision. Very small positive rates can therefore display as `0.00`; using more rate digits is a reasonable presentation refinement. **Pounds, euros and rate edits all propagate by the stated policy**, with no parsing exception or division by zero.

`EditDone` handles completion of an edit, such as an action or focus-change notification, using the event type supplied in the paper. It is not a promise of recalculation after every keystroke. A character-by-character interface would subscribe to the corresponding text-change event instead. The publisher/reactor interaction follows the supplied contract and official [Scala Swing](../../../../../scala-swing.md) documentation; no exact course library build or native graphical execution is presumed.[Publisher/Reactor subscriptions and reactions; the paper supplies the EditDone event contract](../../../../../scala-swing-event-system-documentation.md)

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
