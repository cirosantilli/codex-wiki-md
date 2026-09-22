<h1 id="1/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the displayed network, the first $k$ cells retain values and cell $k+1$ is still in its initial $\mathrm{Cell}$ state. It accepts only a value in $T$, so it cannot accept the incoming [sentinel value](../../../../../../sentinel-value.md). For $k=0$ the first cell blocks the external [sentinel value](../../../../../../sentinel-value.md); for $0<k<n$ a stored cell blocks while trying to pass it to an empty neighbour. Thus

$$
\boxed{k<n\quad\Longrightarrow\quad\text{deadlock before any reversed output}.}
$$

To handle shorter inputs, add an empty-cell branch $l.\mathit{end}\to u.\mathit{end}\to\mathrm{STOP}$ to the initial state. An empty cell then terminates the downward scan and immediately returns an empty sequence. Earlier occupied cells append their retained values exactly as before; later cells need not participate. This works for every $0\leq k\leq n$, because the occupied prefix of the chain alone produces the required output. For $k=n$, the original sentinel-only tail still supplies the empty suffix. Every cell receives the same modification.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Concurrency](../../../../concurrency-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
