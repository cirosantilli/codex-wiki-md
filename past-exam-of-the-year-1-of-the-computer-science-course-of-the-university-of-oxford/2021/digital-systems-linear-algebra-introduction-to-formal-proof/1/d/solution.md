<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Each stage has $J=K=1$ and therefore toggles. The printed clock symbols have no inversion bubble, so they are positive-edge triggered; each later clock is driven by the previous uncomplemented $Q$ output. Consequently the circuit is a [ripple counter](../../../../../ripple-counter.md) that **counts down modulo eight**. A zero [least significant bit](../../../../../least-significant-bit.md) rises to one and propagates the transition; a one falls to zero and stops it. For example, the settled transition from $001$ is $000$, whereas $000$ is followed by $111$.

After $N$ input pulses the settled value is $(1-N)\bmod 8$, giving

$$
\begin{array}{c|c|ccc}
N&Q_2Q_1Q_0&Q_0&Q_1&Q_2\\\hline
20&101&1&0&1\\
101&100&0&0&1\\
257&000&0&0&0
\end{array}
$$

**The answers are $101$, $100$, and $000$**, respectively, in most-significant-first order. Treating these as falling-edge stages would reverse the counting direction and would not follow the drawn clock symbols.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
