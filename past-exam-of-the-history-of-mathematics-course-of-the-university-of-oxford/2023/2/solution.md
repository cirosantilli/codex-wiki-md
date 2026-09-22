<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The figure illustrates [Pierre de Fermat](../../../pierre-de-fermat.md)'s use of [adequality](../../../adequality.md) to construct a [tangent](../../../tangent.md) to a [parabola](../../../parabola.md). Reading the local exam image is decisive: $D$ is the [vertex of a parabola](../../../vertex-of-a-parabola.md), $DC$ lies on its [axis of symmetry](../../../axis-of-symmetry.md), $B$ lies on the [parabola](../../../parabola.md), and the proposed [tangent](../../../tangent.md) $BE$ meets the extended axis at $E$. The horizontal through the auxiliary point $O$ meets the axis at $I$; $O$ lies on $BE$, outside the [parabola](../../../parabola.md). In particular, $O$ must not be treated as a second point of the [parabola](../../../parabola.md). The target is the [subtangent](../../../subtangent.md) $CE$. The diagram and this construction occur in the tangent discussion associated with [Varia opera mathematica by Pierre de Fermat](../../../varia-opera-mathematica-by-pierre-de-fermat.md). The 1679 book was posthumous: its date does not date the invention of the method.[1679 title page and bibliographical record, ETH-Bibliothek](../../../varia-opera-mathematica-by-pierre-de-fermat.md)[Tangent construction, with the same B, C, D, E, I, O labels; the method circulated in the 1630s](../../../fermat-s-rule-for-maxima-and-minima-by-the-garden-of-archimedes.md)

Write $d=CD>0$, $a=CE>0$, and $e=CI$, with $I$ between $C$ and $D$. These are lengths, and the increment $e$ is distinct from the labelled point $E$. Then $DI=d-e$ and $EI=a-e$. The [parabola](../../../parabola.md)'s characteristic relation makes the square of an ordinate proportional to its distance from the [vertex of a parabola](../../../vertex-of-a-parabola.md). At height $I$, the actual ordinate of the [parabola](../../../parabola.md) is shorter than $OI$. Hence

$$
\frac{d}{d-e}>\frac{BC^2}{OI^2}
=\frac{a^2}{(a-e)^2},
$$

where the equality follows from [similar triangles](../../../similar-triangle.md) $BCE$ and $OIE$.

The method of [adequality](../../../adequality.md) replaces the comparison by a relation used to extract the condition of contact:

$$
d(a-e)^2\mathrel{\sim}a^2(d-e).
$$

Expanding and cancelling $da^2$ gives $-2dae+de^2\mathrel{\sim}-a^2e$. Divide by the nonzero increment $e$, then suppress the remaining term containing $e$. The result is $a^2=2da$, so, since $a>0$,

$$
\boxed{CE=2CD.}
$$

Thus $DE=DC$: the intersection with the axis lies as far above the [vertex of a parabola](../../../vertex-of-a-parabola.md) as $C$ lies below it. This is a concrete construction, not just a rule for computing a numerical slope.

A modern check clarifies why the calculation succeeds without pretending that [Pierre de Fermat](../../../pierre-de-fermat.md) used a modern [limit](../../../limit-of-a-function.md). Put $D=(0,0)$, let $y$ increase down the axis, and write the [parabola](../../../parabola.md) as $x^2=ky$, $k>0$. For $B=(b,d)$, with $b^2=kd$, the proposed [tangent](../../../tangent.md) through $E=(0,-d)$ is $y=2bx/k-d$. Substitution gives

$$
x^2-ky=(x-b)^2.
$$

It meets the [parabola](../../../parabola.md) with a [double root](../../../double-root.md) at $B$, and for every other point its $y$ coordinate is less than that of the [parabola](../../../parabola.md). This also verifies the strict comparison used for $O$.

The significance is **a systematic algebraic condition for geometric contact**. Subtracting neighbouring expressions, dividing by an increment, and discarding its remaining terms anticipates [differentiation](../../../differentiation.md). But the historical question is precisely what licenses the last step. The symbol $\sim$ above marks [adequality](../../../adequality.md), not ordinary equality at a finite displacement. Treating the construction as an already stated [epsilon-delta definition of a limit](../../../epsilon-delta-definition-of-a-limit.md) would conceal the methodological innovation and its unresolved explanatory burden.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2023](../../2023-split.md)
3. [Past exam of the history of mathematics course of the University of Oxford](../../split.md)
4. [History of mathematics course of the University of Oxford](../../../history-of-mathematics-course-of-the-university-of-oxford.md)
5. [Year 3 of the mathematics course of the University of Oxford](../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
