<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Inside the supplied `MainFrame`, after both buttons and the label are defined, add:
```
private var clickCount = BigInt(0)
listenTo(button1, button2)
reactions += {
  case ButtonClicked(source) if (source eq button1) || (source eq button2) =>
    clickCount += 1
    label.text = "Total button clicks: " + clickCount.toString
}
```
The [invariant](../../../../../invariant-mathematics.md) is that `clickCount` equals the total number of handled click events from the two buttons. It starts at zero; each matching event increments it exactly once and refreshes the label. The buttons' existing self-listeners can still change their own text independently. **Listening to both publishers is necessary**: their `listenTo(this)` calls subscribe each button to itself, not the frame to both buttons. Updating the label is not another button click, so it does not recursively increment the counter. An [arbitrary-precision integer](../../../../../arbitrary-precision-integer.md) keeps the count exact without a lifetime overflow bound.[Publisher/Reactor subscriptions, listenTo, and reactions; ButtonClicked source event](../../../../../scala-swing-event-system-documentation.md)

The supplied layout already contains the label, so no additional component is needed. Before any click it retains its initial zero-click message; afterwards it displays the cumulative count across both buttons.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
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
