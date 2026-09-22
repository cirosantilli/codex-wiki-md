<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

For a block code, the [minimum distance of a code](../../../../../minimum-distance-of-a-code.md) is the minimum [Hamming distance](../../../../../hamming-distance.md) between distinct codewords, where [Hamming distance](../../../../../hamming-distance.md) counts positions in which two equal-length binary strings differ. We use equal-length codewords, so the fact that the codomain allows arbitrary finite strings creates no ambiguity. Minimum distance $\delta$ means every two distinct codewords differ in at least $\delta$ positions and some pair differs in exactly $\delta$.

Changing at most $\delta-1$ bits cannot turn a codeword into another codeword. Testing membership therefore detects every such nonzero error. For $t=\lfloor(\delta-1)/2\rfloor$, suppose a received word lies within distance $t$ of two codewords. The [triangle inequality](../../../../../triangle-inequality.md) would put their mutual distance at most $2t<\delta$, a contradiction. Hence the radius-$t$ [Hamming balls](../../../../../hamming-ball.md) are disjoint and nearest-codeword decoding corrects all errors of weight at most $t$.

For an alphabet of size $m\geq2$, start with $0$ and the $m-1$ standard unit vectors in $\{0,1\}^{m-1}$. Their [minimum distance of a code](../../../../../minimum-distance-of-a-code.md) is one. Repeat every coordinate $\delta$ times; every distance is multiplied by $\delta$, so the resulting code has **[minimum distance of a code](../../../../../minimum-distance-of-a-code.md) exactly $\delta$**. A one-letter alphabet has no pair of distinct codewords and therefore no finite [minimum distance of a code](../../../../../minimum-distance-of-a-code.md) under this definition; the construction concerns the usual nontrivial coding situation.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
