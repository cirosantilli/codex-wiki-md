<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let the committed model be amounts $p,e$ and an exchange rate $r$, with [invariant](../../../../../invariant-mathematics.md) $e=pr$. Editing pounds keeps the rate and computes euros; editing euros keeps the rate and computes pounds; editing the rate keeps pounds and computes euros. A usable rate must be strictly positive, and every accepted [floating-point number](../../../../../floating-point-number.md) and derived result must be finite. Negative amounts are allowed. Rejecting invalid text preserves the last committed model.

Insert the following members inside the supplied `MainFrame`, after the three fields have been initialized. Its existing layout can remain as written:
```
private var p = 10.0
private var e = 11.5
private var r = 1.15
private var refreshing = false

private def finite(x: Double): Boolean = !x.isNaN && !x.isInfinity

private def showModel(): Unit = {
  refreshing = true
  try {
    pounds.text = java.lang.String.format(java.util.Locale.ROOT, "%.2f", Double.box(p))
    euros.text = java.lang.String.format(java.util.Locale.ROOT, "%.2f", Double.box(e))
    rate.text = r.toString
  } finally {
    refreshing = false
  }
}

private def edit(source: TextField): Unit = {
  try {
    val v = source.text.trim.toDouble
    if (finite(v)) {
      var nextP = p
      var nextE = e
      var nextR = r
      if (source eq pounds) {
        nextP = v
        nextE = v * r
      } else if (source eq euros) {
        nextE = v
        nextP = v / r
      } else if (source eq rate) {
        nextR = v
        nextE = p * v
      }
      if (nextR > 0.0 && finite(nextP) && finite(nextE) && finite(nextR)) {
        p = nextP
        e = nextE
        r = nextR
      }
    }
  } catch {
    case _: NumberFormatException => ()
  }
  showModel()
}

listenTo(pounds, euros, rate)
reactions += {
  case EditDone(source) if !refreshing => edit(source)
}
```
The [invariant](../../../../../invariant-mathematics.md) is interpreted with the usual [floating-point rounding](../../../../../floating-point-rounding.md) in multiplication and division. All candidate values are calculated before committing any of them, so invalid text, zero/negative rates, NaN, infinity and [floating-point overflow](../../../../../floating-point-overflow.md) leave the old model intact. The committed `r` remains positive, so euro-to-pound division is defined. Using a fixed formatting locale keeps the decimal separator compatible with `toDouble`. The displayed amounts are rounded to two decimal places, while the model retains their full available precision. The rate is not forcibly rounded to two places, which could otherwise turn a valid small positive rate into displayed zero.

The `refreshing` guard prevents synchronous derived-field notifications from recursively committing another edit. `EditDone` is an edit-completion event, not a request to react to every partial keystroke; pressing the field's completion action is enough to trigger the conversion. If a particular UI additionally needs live updates, it can subscribe to the appropriate text-change events with the same validation and authoritative-source policy. The supplied API and archived [Scala Swing](../../../../../scala-swing.md) documentation suffice for the requested completion-event implementation; no unidentified practical library is required.[Publisher/Reactor subscription design; archived Swing event API: EditDone carries its source TextField](../../../../../scala-swing-event-system-documentation.md)

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
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
