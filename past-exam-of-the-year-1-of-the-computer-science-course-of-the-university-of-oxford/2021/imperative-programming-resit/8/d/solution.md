<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose the following explicit policy: an edit of pounds recomputes euros; an edit of euros recomputes pounds; an edit of the rate keeps pounds fixed and recomputes euros. Amounts may be any finite signed values, while a rate must be finite and strictly positive. Invalid text, non-finite numbers and overflowing conversions leave the last accepted state intact and restore its display.
```
import scala.swing._
import scala.swing.event.EditDone
import scala.util.Try

object CurrencyConverter extends SimpleSwingApplication {
  def top: Frame = new MainFrame {
    title = "Currency converter"
    val pounds = new TextField(8)
    val euros = new TextField(8)
    val rate = new TextField(8)
    private var poundsValue = 10.0
    private var rateValue = 1.15
    private var updating = false

    private def finite(x: Double): Boolean =
      java.lang.Double.isFinite(x)

    private def money(x: Double): String =
      java.lang.String.format(java.util.Locale.ROOT, "%.2f",
                              java.lang.Double.valueOf(x))

    private def showValues(): Unit = {
      updating = true
      try {
        pounds.text = money(poundsValue)
        euros.text = money(poundsValue * rateValue)
        rate.text = java.lang.Double.toString(rateValue)
      } finally updating = false
    }

    private def commit(field: TextField): Unit = {
      if (!updating) {
        val proposed = Try(field.text.trim.toDouble).toOption
          .filter(finite).map { value =>
            if (field eq pounds) (value, rateValue)
            else if (field eq euros) (value / rateValue, rateValue)
            else (poundsValue, value)
          }
        proposed.foreach { case (newPounds, newRate) =>
          if (finite(newPounds) && finite(newRate) && newRate > 0.0 &&
              finite(newPounds * newRate)) {
            poundsValue = newPounds
            rateValue = newRate
          }
        }
        showValues()
      }
    }

    contents = new FlowPanel {
      contents += new Label("Pounds")
      contents += pounds
      contents += new Label("Euros")
      contents += euros
      contents += new Label("Euros per pound")
      contents += rate
    }
    listenTo(pounds, euros, rate)
    reactions += {
      case EditDone(source) if source eq pounds => commit(pounds)
      case EditDone(source) if source eq euros => commit(euros)
      case EditDone(source) if source eq rate => commit(rate)
    }
    showValues()
  }
}
```
The numeric state has the [invariant](../../../../../invariant-mathematics.md) $eurosValue=poundsValue\cdot rateValue$ and $rateValue>0$; euros are derived instead of being stored independently. A proposal is validated before either stored value changes. The update flag prevents a synchronous programmatic display update from recursively committing another edit. Currency amounts display two decimal places, while the rate retains its parsed precision; display rounding is not repeatedly fed back into the numeric model. `Locale.ROOT` ensures that formatted decimal points match the input parser.

The code handles the `EditDone` events used by the paper rather than trying to parse every intermediate keystroke. It uses [Scala](../../../../../scala.md) 2 style and [Java](../../../../../java-programming-language.md) 8-or-newer numeric helpers. No [Scala](../../../../../scala.md) compiler or Swing runtime execution was available in the checking environment; the state transitions were checked independently, and the API usage was compared with the supplied contract and official [Scala](../../../../../scala.md)/Swing documentation.[isFinite(double), parseDouble(String) and toString(double)](../../../../../java-8-double-api-documentation.md)

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
