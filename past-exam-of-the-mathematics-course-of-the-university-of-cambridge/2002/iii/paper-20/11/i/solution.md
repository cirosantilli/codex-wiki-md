<h1 id="11/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $G:\mathcal D\to\mathcal C$, a [functor-split coequalizer pair](../../../../../../functor-split-coequalizer-pair.md) is a parallel pair $f,g:Y\rightrightarrows Z$ such that its image admits a [split coequalizer](../../../../../../split-coequalizer.md) in $\mathcal C$. In one orientation this means [morphisms](../../../../../../morphism.md) $q:GZ\to Q$, $s:Q\to GZ$ and $t:GZ\to GY$ satisfy

$$
qGf=qGg,\quad qs=1_Q,\quad (Gf)t=1_{GZ},\quad(Gg)t=sq.
$$

These equations prove that $q$ is a [coequalizer](../../../../../../coequalizer.md): if $hGf=hGg$, then $h=hGf\,t=hGg\,t=hsq$, so $hs$ factors $h$; uniqueness follows from $qs=1$. They remain true under every [functor](../../../../../../functor.md), making a [split coequalizer](../../../../../../split-coequalizer.md) an absolute [colimit](../../../../../../colimit.md).

To say that $G$ reflects such [coequalizers](../../../../../../coequalizer.md) means that any fork $Y\rightrightarrows Z\xrightarrow{p}W$ in $\mathcal D$ whose image is a [split coequalizer](../../../../../../split-coequalizer.md) is itself a [coequalizer](../../../../../../coequalizer.md) in $\mathcal D$. This is a reflection assertion about an existing fork; it does not by itself require lifting every split fork from $\mathcal C$, or creating its splitting maps in $\mathcal D$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11](../../11.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
