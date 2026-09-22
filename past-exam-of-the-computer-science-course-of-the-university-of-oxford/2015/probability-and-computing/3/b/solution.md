<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Betty's scheme is biased for every $n\geq2$.** The output $H^nT^n$ occurs precisely when the first $n$ tosses are heads: the algorithm stops there and appends $n$ tails. Thus

$$
\mathbb P(H^nT^n)=2^{-n}.
$$

For comparison, take the output $(HT)^n$. Its first $2n-2$ symbols contain $n-1$ heads and $n-1$ tails, so neither stopping threshold has been reached. The next symbol is the $n$th head, at which point the last tail is appended. Its unique generating prefix has length $2n-1$, giving

$$
\mathbb P((HT)^n)=2^{-(2n-1)}.
$$

Therefore

$$
\boxed{\frac{\mathbb P(H^nT^n)}{\mathbb P((HT)^n)}=2^{n-1}>1\quad(n\geq2).}
$$

The faster stopping rule does not produce a [uniform distribution on a finite set](../../../../../discrete-uniform-distribution.md) of balanced [binary sequences](../../../../../bitstream.md). For example, at $n=2$ the six outputs have the following exact [probabilities](../../../../../probability.md):

| Output | Betty | Uniform target |
| --- | --- | --- |
| `HHTT` | $1/4$ | $1/6$ |
| `HTHT` | $1/8$ | $1/6$ |
| `HTTH` | $1/8$ | $1/6$ |
| `THHT` | $1/8$ | $1/6$ |
| `THTH` | $1/8$ | $1/6$ |
| `TTHH` | $1/4$ | $1/6$ |

For $n=1$, the two possible outputs each have [probability](../../../../../probability.md) $1/2$, so that special case is uniform. For $n=0$, simply return the empty output.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
