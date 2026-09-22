<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $d=\operatorname{dist}(x,Z)$. If $d=0$, the zero functional works. If $d>0$, then $x\notin\overline Z$, and on $M=Z+\operatorname{span}\{x\}$ define

$$
f_0(z+ax)=ad.
$$

The representation is unique, so this is linear. For $a\ne0$,

$$
|f_0(z+ax)|=|a|d=\operatorname{dist}(ax,Z)\leq\|z+ax\|,
$$

and the bound also holds for $a=0$. Thus $\|f_0\|\leq1$. The [Hahn-Banach theorem](../../../../hahn-banach-theorem.md) extends it to $f\in X'$ with the same bound, proving

$$
\boxed{f|_Z=0,\qquad f(x)=d,\qquad\|f\|\leq1.}
$$

No closedness assumption on $Z$ was required; [distance](../../../../distance.md) is unchanged on taking its [closure](../../../../closure-topology.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
