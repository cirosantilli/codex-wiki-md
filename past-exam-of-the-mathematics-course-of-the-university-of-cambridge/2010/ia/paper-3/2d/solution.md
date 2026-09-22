<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

Compose [permutations](../../../../../permutation.md) from right to left. Tracking the images gives $1\mapsto2\mapsto1$, $3\mapsto4\mapsto3$, and $5\mapsto5$, so

$$
\boxed{(123)(234)=(12)(34).}
$$

Two [transpositions](../../../../../transposition-permutation.md) give [sign of a permutation](../../../../../sign-of-a-permutation.md) $+1$, proving that this element belongs to the [alternating group](../../../../../alternating-group.md) $A_5$.

Its [conjugacy class](../../../../../conjugacy-class.md) consists of all double transpositions. Conjugation merely relabels the letters, so no other cycle type can occur. Conversely, choose a permutation $h\in S_5$ relabelling the two pairs into any desired two pairs. If $h$ is odd, replace it by $h(12)$: the transposition $(12)$ centralizes $(12)(34)$, so this replacement is even and gives the same conjugate. Thus every double transposition is reached by conjugation inside $A_5$.

The complete list of fifteen elements, grouped by their fixed letter, is

$$
\begin{aligned}
&(12)(34),\ (13)(24),\ (14)(23),\\
&(12)(35),\ (13)(25),\ (15)(23),\\
&(12)(45),\ (14)(25),\ (15)(24),\\
&(13)(45),\ (14)(35),\ (15)(34),\\
&(23)(45),\ (24)(35),\ (25)(34).
\end{aligned}
$$

There are five choices of fixed letter and three pairings of the other four letters, confirming the [conjugacy class](../../../../../conjugacy-class.md) size $15$.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
