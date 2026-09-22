<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Lp norm](../../../../../lp-norm.md) of the forcing at the critical exponent is constant:

$$
\|f_m\|_{L^{6/5}(B)}^{6/5}
=|E_m|^{-1}\int_B\chi_{E_m}\,dx=1.
$$

To prove [weak convergence](../../../../../weak-convergence.md) in $L^{6/5}(B)$, the [duality of Lp spaces](../../../../../duality-of-lp-spaces.md) says that we must test against an arbitrary $g\in L^6(B)$. [Holder inequality](../../../../../holder-inequality.md), restricted to the shrinking [measurable set](../../../../../measurable-set.md) $E_m$, gives

$$
\begin{aligned}
\left|\int_B f_mg\,dx\right|
&\leq |E_m|^{-5/6}\int_{E_m}|g|\,dx\\
&\leq |E_m|^{-5/6}|E_m|^{5/6}
\left(\int_{E_m}|g|^6\,dx\right)^{1/6}
=\left(\int_{E_m}|g|^6\,dx\right)^{1/6}\longrightarrow0.
\end{aligned}
$$

The last step is [absolute continuity of the Lebesgue integral](../../../../../absolute-continuity-of-the-lebesgue-integral.md), since $|E_m|=r_m^3|E|\to0$ and $|g|^6$ is integrable. Thus

$$
\boxed{f_m\rightharpoonup0\text{ in }L^{6/5}(B),\qquad\|f_m\|_{6/5}=1.}
$$

Testing only bounded or smooth functions would not by itself establish this [weak convergence](../../../../../weak-convergence.md); the restricted [Holder inequality](../../../../../holder-inequality.md) handles every member of the full dual space.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../../split.md)
6. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
