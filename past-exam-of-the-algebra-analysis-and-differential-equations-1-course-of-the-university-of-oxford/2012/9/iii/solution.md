<h1 id="9/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $I_n(p)=\int_0^\infty e^{-pt}t^n\,dt$. For $\operatorname{Re}p>0$, [exponential decay](../../../../exponential-decay.md) dominates every fixed power of $t$, so the [improper integral](../../../../improper-integral.md) converges absolutely and $e^{-pT}T^n\to0$. For $n\geq1$, [integration by parts](../../../../integration-by-parts.md) gives

$$
I_n(p)=\left[-\frac{e^{-pt}t^n}p\right]_0^\infty
+\frac np\int_0^\infty e^{-pt}t^{n-1}\,dt
=\frac np I_{n-1}(p).
$$

The preceding part gives the base case $I_0(p)=1/p$. Repeated application, or [mathematical induction](../../../../mathematical-induction.md), yields

$$
\boxed{\mathcal L\{t^n\}(p)=\frac{n!}{p^{n+1}},\qquad \operatorname{Re}p>0.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [9](../../9.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
