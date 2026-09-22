<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [split coequalizer](../../../../../../split-coequalizer.md) consists of $f,g:A\rightrightarrows B$, $q:B\to Q$, $s:Q\to B$ and $t:B\to A$ with $qf=qg$, $qs=1_Q$, $ft=1_B$ and $gt=sq$. If $hf=hg$, then $h=hft=hgt=hsq$. Thus $hs$ factors $h$ through $q$, and the factor is unique because $q$ has the right inverse $s$. This proves the [coequalizer](../../../../../../coequalizer.md) property directly. Every [functor](../../../../../../functor.md) preserves the diagram, since all these equations are preserved.

For [idempotent splitting through a coequalizer](../../../../../../idempotent-splitting-through-a-coequalizer.md), first suppose $e=ir$ with $ri=1_Q$. Then $re=r$. Any $h:E\to Z$ satisfying $he=h$ factors as $h=(hi)r$, uniquely since $r$ is a [split epimorphism](../../../../../../split-epimorphism.md). Hence $r$ coequalizes $(e,1_E)$.

Conversely, let $q:E\to Q$ coequalize $(e,1_E)$. Since $e^2=e$, the arrow $e:E\to E$ itself equalizes the pair, so there is a unique $i:Q\to E$ with $iq=e$. Then $qi q=qe=q$, and every [coequalizer](../../../../../../coequalizer.md) is an [epimorphism](../../../../../../epimorphism.md), so $qi=1_Q$. Thus $e=iq$ is a [splitting of an idempotent morphism](../../../../../../splitting-of-an-idempotent-morphism.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
