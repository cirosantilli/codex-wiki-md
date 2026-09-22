<h1 id="a/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [Stone-Čech extension property](../../../../../stone-cech-extension-property.md): a discrete [topological space](../../../../../topological-space.md) $X$ embeds densely into a [compact](../../../../../compact-space.md) [Hausdorff space](../../../../../hausdorff-space.md) $\beta X$, and every [continuous map](../../../../../continuous-map.md) from $X$ to a [compact](../../../../../compact-space.md) [Hausdorff space](../../../../../hausdorff-space.md) extends continuously to $\beta X$. Apply it to the [characteristic function](../../../../../characteristic-function-split.md) $\chi_A:X\to\{0,1\}$ of an arbitrary [subset](../../../../../subset.md) $A$; discreteness makes it [continuous](../../../../../continuous-function.md). Its extension $\widetilde\chi_A$ has [clopen](../../../../../clopen-set.md) fibers, and

$$
\overline A^{\,\beta X}=\widetilde\chi_A^{-1}(1).
$$

Indeed that fiber is [closed](../../../../../closed-set.md) and contains $A$, while its openness and density of $X$ show that every point in the fiber is approached by points of $A$.

If $A$ and $B$ are disjoint, the extension of $\chi_A$ is one on $\overline A$ and zero on $\overline B$, so these [closures](../../../../../closure-topology.md) are disjoint. The inclusion $X\to\beta X$ therefore satisfies the criterion from part (b), and its ultrafilter-limit map is both [surjective](../../../../../surjective-function.md) and [injective](../../../../../injective-function.md). Thus

$$
\boxed{\Upsilon(X)\longleftrightarrow\beta X,\qquad
\mathcal H\longmapsto\text{the unique limit of its image filter}.}
$$

This is a [bijection](../../../../../bijection.md) of underlying [sets](../../../../../set-split.md); identifying the compatible [topology](../../../../../topology-split.md) on the [ultrafilter](../../../../../ultrafilter.md) [topological space](../../../../../topological-space.md) would give the familiar stronger [homeomorphism](../../../../../homeomorphism.md) statement, but is not needed for the requested conclusion.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
