<h1 id="e/e4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The claim is false for an arbitrary codomain $Y$.** Let $X=[0,1]$ with its usual topology, let $Y$ be the [Sierpiński space](../../../../../sierpinski-space.md) with open sets $\varnothing,\{1\},Y$, and define $f(0)=0$, $f(x)=1$ for $x>0$. This is a [continuous map](../../../../../continuous-map.md): the only nontrivial open-set preimage is $f^{-1}(\{1\})=(0,1]$, which is relatively open in $X$.

The sets $K_n=[0,1/n]$ are nonempty, nested and compact. But

$$
\boxed{f\!\left(\bigcap_nK_n\right)=\{0\}\ne\{0,1\}=\bigcap_nf(K_n).}
$$

Thus the extra generality in the printed codomain changes the assertion materially. This is the [failure of nested compact image intersection without closed fibers](../../../../../failure-of-nested-compact-image-intersection-without-closed-fibers.md).

If the codomain is a [T1 space](../../../../../t1-space.md), the [continuous images of nested compact intersections](../../../../../continuous-images-of-nested-compact-intersections.md) theorem does give the desired equality. The forward inclusion holds for every map. For the reverse, take $y\in\bigcap_nf(K_n)$ and set $F_n=K_n\cap f^{-1}(\{y\})$. The fibers are closed by continuity and the T1 property, so the $F_n$ are nested nonempty closed subsets of the compact set $K_1$. The [finite intersection property](../../../../../finite-intersection-property.md) gives $x\in\bigcap_nF_n$, with $f(x)=y$. It is enough that these particular fibers be closed in $K_1$; a Hausdorff codomain, as in the native self-map formulation, is a familiar sufficient assumption.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [E4](../../e4.md)
3. [E](../../../e.md)
4. [2008 printed variant](../../../../2008-printed-variant-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
