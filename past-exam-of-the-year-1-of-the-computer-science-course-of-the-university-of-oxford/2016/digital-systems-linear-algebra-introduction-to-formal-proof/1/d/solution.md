<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use **an eight-[bit](../../../../../bit.md) modulo-256 [binary counter](../../../../../binary-counter.md), eight 256:1 [multiplexers](../../../../../multiplexer.md), eight data lines and eight address lines**. Thus there are **sixteen signal lines**, apart from clock and reset, and a full scan takes 256 [clock periods](../../../../../clock-period.md). The counter next-state equations generalize to

$$
D_0=\neg q_0,\qquad D_i=q_i\oplus\bigwedge_{j=0}^{i-1}q_j\quad(1\leq i\leq7).
$$

A 256:1 [multiplexer](../../../../../multiplexer.md) for one data [bit](../../../../../bit.md) can be made hierarchically: 32 first-stage 8:1 [multiplexers](../../../../../multiplexer.md) select within eight-sensor groups using $q_2q_1q_0$; four second-stage 8:1 [multiplexers](../../../../../multiplexer.md) select groups using $q_5q_4q_3$; one final 4:1 [multiplexer](../../../../../multiplexer.md) selects using $q_7q_6$. A final 8:1 [multiplexer](../../../../../multiplexer.md) also works if one select input is fixed to zero and only four data inputs are used. Repeat this network eight times, sharing all selection lines. Allow for the extra [propagation delay](../../../../../propagation-delay.md) when choosing the [clock period](../../../../../clock-period.md).

## ↑ Ancestors (12)

1. [D](../d.md)
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
