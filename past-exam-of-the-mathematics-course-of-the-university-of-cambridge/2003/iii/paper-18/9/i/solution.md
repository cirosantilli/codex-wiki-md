<h1 id="9/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [functor-split coequalizer pair](../../../../../../functor-split-coequalizer-pair.md) for $G$ is a parallel pair $f,g:A\rightrightarrows B$ in $\mathcal D$ whose image has a split [coequalizer](../../../../../../coequalizer.md) in $\mathcal C$. Explicitly there are $q:GB\to Q$, $s:Q\to GB$, $t:GB\to GA$ with

$$
qGf=qGg,\qquad qs=1_Q,\qquad(Gf)t=1_{GB},\qquad(Gg)t=sq.
$$

These equations give the [coequalizer](../../../../../../coequalizer.md) property: if $hGf=hGg$, then $h=h(Gf)t=h(Gg)t=hsq$, and $q$ is split epic so the factor through it is unique. Every [functor](../../../../../../functor.md) preserves such a split diagram, since it preserves these equations.

Reflection means that, for such a pair, any existing arrow $e:B\to D$ whose image is a [coequalizer](../../../../../../coequalizer.md) is itself a [coequalizer](../../../../../../coequalizer.md) in $\mathcal D$. A [coequalizer](../../../../../../coequalizer.md) of the image pair is isomorphic to the specified split one and inherits its splitting. This is reflection of an existing quotient, not an assertion that every base quotient has a lift.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [9](../../9.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
