<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume first that the finite [relator](../../../../../../relator.md) set $R$ is nonempty and put

$$
M=\max_{r\in R}(|r|/2+2).
$$

For every nonidentity finite-order element choose a [shortest conjugacy representative](../../../../../../shortest-conjugacy-representative.md). The preceding parts give a word representing its conjugacy class of length at most $M$. The identity class has the empty representative.

There are only finitely many such words because the generating alphabet is finite. If it has $q=2|A|$ formal letters and $N=\lfloor M\rfloor$, a sufficient upper bound for the number of words is

$$
\sum_{j=0}^{N}q^j.
$$

Distinct classes cannot require more representatives than there are words; different words may of course represent the same class. Consequently

$$
\boxed{G\text{ has finitely many conjugacy classes of finite-order elements}.}
$$

This is the [torsion conjugacy bound for a Dehn presentation](../../../../../../torsion-conjugacy-bound-for-a-dehn-presentation.md). It does not claim that there are only finitely many finite-order elements.

If $R$ is empty, the maximum in the PDF is undefined. Handle this case separately: the group is a [free group](../../../../../../free-group.md) on the finite alphabet, and a nonempty [cyclically reduced word](../../../../../../cyclically-reduced-word.md) has no freely trivial positive power. Thus there is no nonidentity torsion and only the identity conjugacy class. If the alphabet is empty, the group is trivial and the same conclusion holds.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
