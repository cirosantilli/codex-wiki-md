<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In [differential Manchester encoding](../../../../../differential-manchester-encoding.md), every data [bit](../../../../../bit.md) still has a compulsory transition at its midpoint for [clock recovery](../../../../../clock-recovery.md). The data value is specified by whether a transition occurs at the beginning of the [bit](../../../../../bit.md), rather than by the direction of the midpoint transition. One convention is beginning transition for zero and no beginning transition for one; interchanging the meanings consistently also works.

Reversing the signal polarity exchanges high and low everywhere, but preserves both the presence and the absence of transitions. A receiver using [differential Manchester encoding](../../../../../differential-manchester-encoding.md) therefore decodes the same data after a polarity reversal, provided it has acquired the timing and boundary reference. Ordinary [Manchester encoding](../../../../../manchester-code.md) with a fixed low–high/high–low interpretation would exchange the two data values. The advantage is

$$
\boxed{\text{self-clocking transmission insensitive to a global polarity reversal}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Computer networks](../../../computer-networks-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
