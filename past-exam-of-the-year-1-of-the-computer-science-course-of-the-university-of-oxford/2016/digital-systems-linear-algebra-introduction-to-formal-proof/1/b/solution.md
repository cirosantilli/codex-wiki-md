<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For data inputs $d_0,\ldots,d_7$ and selection [bits](../../../../../bit.md) $s_2s_1s_0$, use a three-to-eight [binary decoder](../../../../../binary-decoder.md). Its output $e_i$ is the [minterm](../../../../../minterm.md) that is one exactly when the selection equals the three-[bit](../../../../../bit.md) [binary representation](../../../../../binary-number.md) of $i$. For example,

$$
e_0=\neg s_2\land\neg s_1\land\neg s_0,\quad e_1=\neg s_2\land\neg s_1\land s_0,\quad e_7=s_2\land s_1\land s_0.
$$

Gate each data input with its decoded selection using an [AND gate](../../../../../and-gate.md), then combine all eight results with an [OR gate](../../../../../or-gate.md):

$$
\boxed{z=\bigvee_{i=0}^7(e_i\land d_i).}
$$

Exactly one $e_i$ is asserted, so $z=d_i$ for the selected $i$, regardless of the other data inputs. A direct implementation uses three shared [NOT gates](../../../../../not-gate.md), eight three-input [AND gates](../../../../../and-gate.md) for the [binary decoder](../../../../../binary-decoder.md), eight two-input [AND gates](../../../../../and-gate.md) for the data, and one eight-input [OR gate](../../../../../or-gate.md). Equivalently, combine each decoder term with its data input in one four-input [AND gate](../../../../../and-gate.md). Larger [logic gates](../../../../../logic-gate.md) may be built from two-input ones.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
