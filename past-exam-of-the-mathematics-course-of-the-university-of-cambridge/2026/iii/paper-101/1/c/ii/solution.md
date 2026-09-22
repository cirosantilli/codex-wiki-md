<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the nonsplit [short exact sequence](../../../../../../../short-exact-sequence.md)

$$
0\longrightarrow L\xrightarrow{j}M\xrightarrow{q}N\longrightarrow0.
$$

For an endomorphism $g:M\to M$, the composite $qgj:L\to N$ vanishes because $\operatorname{Hom}_R(L,N)=0$. Hence $g$ restricts to an endomorphism $f$ of $L$ and induces an endomorphism $h$ of $N$, giving a [commutative diagram](../../../../../../../commutative-diagram.md) of short exact sequences.

Because $L$ and $N$ are [brick modules](../../../../../../../brick-module.md), each of $f,h$ is either zero or an isomorphism. If both are isomorphisms, the [short five lemma](../../../../../../../short-five-lemma.md) makes $g$ an isomorphism. If both vanish, $g$ factors successively through $N$ and through $L$, hence through a map $N\to L$; this map is zero, so $g=0$.

The mixed cases would split the sequence. If $f$ is invertible and $h=0$, then $qg=0$, so $g=j\alpha$ for some $\alpha:M\to L$; the identity $\alpha j=f$ makes $f^{-1}\alpha$ a retraction of $j$. If $f=0$ and $h$ is invertible, then $gj=0$, so $g=\beta q$; the identity $q\beta=h$ makes $\beta h^{-1}$ a section of $q$. Both contradict nonsplitting. Thus every endomorphism of $M$ is zero or invertible, and $M$ is a brick.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 101](../../../../paper-101-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
