<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Euclidean algorithm](../../../../../euclidean-algorithm.md) gives

$$
\begin{aligned}
2392&=1748+644,\\
1748&=2\cdot644+460,\\
644&=460+184,\\
460&=2\cdot184+92,\\
184&=2\cdot92.
\end{aligned}
$$

The last nonzero remainder is **$g=92$**. Back-substitution produces its [Bézout coefficients](../../../../../bezout-coefficient.md):

$$
\begin{aligned}
92&=460-2\cdot184\\
&=3\cdot460-2\cdot644\\
&=3\cdot1748-8\cdot644\\
&=-8\cdot2392+11\cdot1748.
\end{aligned}
$$

Thus **$(m,n)=(-8,11)$** is a requested pair. The final equality independently checks the calculation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Discrete mathematics, continuous mathematics and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
