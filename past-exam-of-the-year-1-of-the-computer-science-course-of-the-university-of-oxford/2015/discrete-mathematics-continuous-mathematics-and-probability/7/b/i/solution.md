<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\tau$ be the [absorption time](../../../../../../absorption-time.md). Its [expectation](../../../../../../expected-value-split.md) is finite: from every interior state, a string of at most $n$ successive left moves reaches $0$, and the [probability](../../../../../../probability.md) of such a string is at least $p=3^{-n}$. Hence the [Markov property](../../../../../../markov-property.md) gives $\mathbb P_k(\tau>jn)\le(1-p)^j$, a geometric tail bound, and $\mathbb E_k[\tau]<\infty$.

For $1\le k\le n-1$, one step is always spent before absorption or the remaining walk. Apply [first-step analysis](../../../../../../first-step-analysis.md) and the [law of total expectation](../../../../../../law-of-total-expectation.md) to the three possible first moves. The [conditional expectations](../../../../../../conditional-expectation.md) of the remaining [absorption time](../../../../../../absorption-time.md) are $e_{k+1},e_k,e_{k-1}$, respectively; independence of future moves gives the same law as a fresh [random walk](../../../../../../random-walk-split.md) from the new position. Thus

$$
e_k=1+\frac13e_{k+1}+\frac13e_k+\frac13e_{k-1},
$$

which rearranges to

$$
\boxed{\frac13e_{k+1}-\frac23e_k+\frac13e_{k-1}=-1.}
$$

The term $1$ also appears when the walk stays at $k$, because staying still consumes a step.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
