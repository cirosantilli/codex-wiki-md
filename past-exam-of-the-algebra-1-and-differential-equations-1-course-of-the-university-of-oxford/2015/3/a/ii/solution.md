<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define the [bidual evaluation map](../../../../../bidual-evaluation-map.md) by evaluation:

$$
\boxed{J:V\longrightarrow V'',\qquad J(v)(\ell)=\ell(v).}
$$

For fixed $v$, this is a [linear functional](../../../../../linear-functional.md) of $\ell$, so it belongs to the [double dual](../../../../../double-dual.md). It is also linear as a function of $v$. If $v\ne0$, some coordinate of $v$ in a [basis](../../../../../basis.md) is nonzero, and the corresponding [dual basis](../../../../../dual-basis.md) functional detects it. Hence $J(v)\ne0$, proving [injectivity](../../../../../injective-function.md).

The spaces $V,V',V''$ all have the same finite [dimension](../../../../../dimension-vector-space.md). Therefore an [injective](../../../../../injective-function.md) [linear map](../../../../../linear-map.md) $J:V\to V''$ is [surjective](../../../../../surjective-function.md), proving the required [linear isomorphism](../../../../../linear-isomorphism.md).

This [linear isomorphism](../../../../../linear-isomorphism.md) is natural because evaluation requires no [basis](../../../../../basis.md). More explicitly, for any [linear map](../../../../../linear-map.md) $A:V\to W$, its [dual map](../../../../../transpose-of-a-linear-map.md) satisfies

$$
\bigl(A''J_V(v)\bigr)(\ell)=J_V(v)(\ell\circ A)=\ell(Av)=J_W(Av)(\ell),
$$

so $A''J_V=J_WA$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
