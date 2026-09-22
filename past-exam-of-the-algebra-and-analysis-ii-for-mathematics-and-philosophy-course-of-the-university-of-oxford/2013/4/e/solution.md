<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First take $z\in U_-$ and put $w=\bar z\in U_+$. Reflection symmetry of the function gives

$$
\frac{f(z+h)-f(z)}h
=\overline{\frac{f(w+\bar h)-f(w)}{\bar h}}
\longrightarrow\overline{f'(w)}.
$$

Hence $f$ is [holomorphic](../../../../holomorphic-function-split.md) on $U_-$, with $f'(z)=\overline{f'(\bar z)}$ there.

It remains to cross the real axis. Fix a real point $p\in U$ and a small disk about $p$ with closure in $U$. Consider a [triangle](../../../../triangle.md) in a still smaller disk. Intersect its filled interior with the closed upper and lower half-planes and triangulate the resulting [convex](../../../../convex-function.md) polygons. This gives finitely many [triangles](../../../../triangle.md) lying on one side of the real axis, possibly with edges on that axis. Degenerate pieces contribute zero.

For an upper piece, translate its three vertices by $i\varepsilon$ with $\varepsilon>0$. For sufficiently small $\varepsilon$ the translated [triangle](../../../../triangle.md) lies entirely in $U_+$ and remains in $U$, so its boundary [integral](../../../../integral-split.md) is zero by Cauchy's theorem. Part (d), or its segment-integral proof, shows that the [integral](../../../../integral-split.md) converges to that around the untranslated piece as $\varepsilon\downarrow0$. Thus the original piece has zero [integral](../../../../integral-split.md). Translate lower pieces by $-i\varepsilon$ to obtain the same conclusion in $U_-$.

When all the oriented [triangle](../../../../triangle.md) integrals are added, their internal edges cancel, including the segments on the real axis. The original [triangle](../../../../triangle.md) therefore has zero boundary [integral](../../../../integral-split.md). [Continuity](../../../../continuous-function.md) of $f$ on $U$ now allows [Morera's theorem](../../../../morera-s-theorem.md) in the disk, proving holomorphicity near $p$. Together with the two half-plane arguments this gives

$$
\boxed{f\text{ is holomorphic throughout }U.}
$$

This is a [Morera gluing lemma across a straight line](../../../../morera-gluing-lemma-across-a-straight-line.md); the original [continuity](../../../../continuous-function.md) hypothesis is essential to the limiting step.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the algebra and analysis II for mathematics and philosophy course of the University of Oxford](../../../split.md)
5. [Algebra and analysis II for mathematics and philosophy course of the University of Oxford](../../../../algebra-and-analysis-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Mathematics and philosophy course of the University of Oxford](../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
