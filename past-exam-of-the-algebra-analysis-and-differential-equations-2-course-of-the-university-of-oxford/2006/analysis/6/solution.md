<h1 id="analysis/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

At a zero $a$, [Taylor's theorem](../../../../taylor-s-theorem.md) gives $f(z)=\sum_{n\geq0}c_n(z-a)^n$ near $a$. If some [coefficient](../../../../coefficient.md) is nonzero, let $m$ be the least such index. Then $f(z)=(z-a)^mq(z)$ with $q(a)\ne0$, and [continuity](../../../../continuous-function.md) makes $q$ nonzero on a smaller disc. Thus $a$ is an isolated zero. A [limit point](../../../../limit-point.md) of zeros is also a zero by [continuity](../../../../continuous-function.md) and cannot be isolated, so all Taylor [coefficients](../../../../coefficient.md) there vanish and $f$ vanishes on a nonempty open disc.

Let $A$ be the set of points having a neighborhood on which $f$ vanishes. It is nonempty and open. A point in its relative closure either already belongs to $A$ or is a [limit point](../../../../limit-point.md) of distinct zeros; the preceding argument puts it in $A$ in either case. Thus $A$ is also relatively closed. [Connectedness](../../../../connected-space.md) of $D$ gives $A=D$, proving **$f$ is identically zero**.

For conjugate reflection, the disc is invariant under conjugation, and

$$
\frac{h(z+w)-h(z)}w=\overline{\frac{g(\bar z+\bar w)-g(\bar z)}{\bar w}}\longrightarrow\overline{g'(\bar z)}.
$$

Hence **$h$ is [holomorphic](../../../../holomorphic-function-split.md)**, with [derivative](../../../../derivative.md) $\overline{g'(\bar z)}$. If $g$ is real on the real diameter, then for real $x\in(-1,1)$, $h(x)=\overline{g(x)}=g(x)$. The [holomorphic](../../../../holomorphic-function-split.md) difference $g-h$ therefore has zeros accumulating at zero, and the [identity theorem](../../../../identity-theorem.md) just proved gives **$g=h$ on the entire disc**.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Analysis](../../analysis.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
