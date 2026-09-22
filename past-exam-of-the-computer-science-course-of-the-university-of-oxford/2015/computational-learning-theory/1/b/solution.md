<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix an $m$-point [set](../../../../../set-split.md) $S$. The restriction of an [intersection](../../../../../set-intersection.md) $c_1\cap c_2$ to $S$ is determined by the ordered pair of restrictions $c_1|_S,c_2|_S$. Some pairs can yield the same [intersection](../../../../../set-intersection.md), so the [growth function of a hypothesis class](../../../../../shattering-coefficient.md) satisfies

$$
\Pi_{H_2}(m)\leq\Pi_H(m)^2.
$$

Assume first that $d\geq1$. If $12d$ points were shattered by $H_2$, the [Sauer-Shelah lemma](../../../../../sauer-shelah-lemma.md) would imply

$$
2^{12d}=\Pi_{H_2}(12d)\leq\Pi_H(12d)^2\leq(12e)^{2d}.
$$

But $e<3$, so $(12e)^2<36^2=1296<4096=2^{12}$. Raising this strict inequality to the positive integer power $d$ gives a contradiction. No $12d$-point [set](../../../../../set-split.md) can therefore be shattered; neither can any larger [set](../../../../../set-split.md), since shattering passes to subsets. Consequently

$$
\boxed{\operatorname{VC}(H_2)<12d\qquad(d\geq1).}
$$

**The printed strict inequality needs $d\geq1$.** For example, on a nonempty domain let $H$ contain only the identically zero [classifier](../../../../../classifier.md). Then $\operatorname{VC}(H)=\operatorname{VC}(H_2)=0$, whereas the stated conclusion would require $0<0$. More generally, a nonempty [hypothesis class](../../../../../concept-class.md) of [VC dimension](../../../../../vc-dimension.md) zero has only one distinct labelling [function](../../../../../function-split.md), since two different [functions](../../../../../function-split.md) would shatter a point on which they differ. Its self-[intersection](../../../../../set-intersection.md) class also has [VC dimension](../../../../../vc-dimension.md) zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Computational learning theory](../../../computational-learning-theory-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
