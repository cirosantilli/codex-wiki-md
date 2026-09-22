<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [serial-in parallel-out shift register](../../../../../serial-in-parallel-out-shift-register.md) is a chain of [digital registers](../../../../../digital-register.md) driven by the same [clock signal](../../../../../clock-signal.md). At each active [clock edge](../../../../../clock-edge.md), the first stage captures the input and every later stage captures the preceding stage's old value. Its parallel outputs expose the successive delayed samples simultaneously.

Let $a_n$ be the current sample and, immediately before its sampling edge, let $h_1=a_{n-1},\ldots,h_{k-1}=a_{n-k+1}$. Feed these signals to [combinational logic](../../../../../combinational-logic.md) implementing $f$. Then

$$
\boxed{z_n=f(a_n,h_1,\ldots,h_{k-1})=f(a_n,a_{n-1},\ldots,a_{n-k+1}).}
$$

Only $k-1$ stored history stages are needed if the current input is used directly. Alternatively, a $k$-stage [shift register](../../../../../shift-register.md) exposes all $k$ samples after the edge. A separate output [digital register](../../../../../digital-register.md) can capture the first arrangement at the edge, giving a fully sampled output. Initialize the history, or regard the first $k-1$ cycles as a filling interval.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
