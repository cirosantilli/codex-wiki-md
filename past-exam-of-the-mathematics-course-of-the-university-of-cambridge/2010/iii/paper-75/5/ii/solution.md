<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $d$ is a [retract in a category](../../../../../../retract-in-a-category.md) of $Tc$, write $i:d\to Tc$, $r:Tc\to d$ with $ri=1_d$. For a [natural transformation](../../../../../../natural-transformation.md) $\alpha:P\to Q$ of [categorical presheaves](../../../../../../presheaf-category-theory.md), naturality gives

$$
\alpha_d=Q(i)\,\alpha_{Tc}\,P(r).
$$

Consequently transformations agreeing at all $Tc$ agree at every retract of such an object. If every $d$ is such a retract, restriction $f^*$ is faithful, and the [geometric morphism](../../../../../../geometric-morphism.md) is surjective.

Conversely suppose $f^*$ is faithful. Inside the [representable presheaf](../../../../../../representable-functor.md) $yd=\mathbb D(-,d)$, define $S_d(e)$ to consist of arrows $e\to d$ that factor through some $Tc$. Precomposition preserves this condition, so $S_d$ is a subpresheaf. At $e=Tc$, every arrow factors through that very object, so $f^*S_d=f^*yd$. A faithful geometric inverse image reflects an inclusion becoming invertible, as proved in Question 4(iii). Hence $S_d=yd$, and $1_d\in S_d(d)$ factors as $d\to Tc\to d$. This is the required retraction. We have proved the [retract criterion for surjective presheaf geometric morphisms](../../../../../../retract-criterion-for-surjective-presheaf-geometric-morphisms.md):

$$
\boxed{f\text{ surjective}\Longleftrightarrow
\text{every }d\in\mathbb D\text{ is a retract of some }Tc.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
