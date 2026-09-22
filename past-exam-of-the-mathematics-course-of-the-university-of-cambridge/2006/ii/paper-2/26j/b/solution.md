<h1 id="26j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

One complete cycle consists of ten stops of mean one minute and ten journeys of mean four minutes, so its mean duration is fifty minutes. Over the eight-hour shift, the elementary renewal approximation gives **$480/50=9.6$ completed circuits on average**.

For the end-of-shift calculation use the long-run occupation [probabilities](../../../../../../probability.md) of the twenty successive phases. Each stop phase has [probability](../../../../../../probability.md) $1/50$, and each travel phase [probability](../../../../../../probability.md) $4/50$. Alighting stop $j$ is therefore selected with [probability](../../../../../../probability.md) $1/50+4/50=1/10$, from either stopping there or travelling toward it. If that stop is the station, no further stops are passed. If it is stop $j\ge2$, the intermediate stops are $j+1,\ldots,10$, numbering $10-j$. Thus the requested approximate mean is

$$
\boxed{\frac1{10}\left(0+8+7+\cdots+1+0\right)=3.6.}
$$

The approximation treats eight hours as long compared with a cycle and ignores the initial-phase transient. Exponential [holding times](../../../../../../holding-time.md) justify the twenty-phase Markov description; independent cycle times justify the renewal rate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26J](../../26j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
