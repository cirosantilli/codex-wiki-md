<h1 id="differential-equations/7/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [vector field](../../../../../vector-field.md) is continuous on the cube. Part (b) gives $M=1$, and part (c) supplies a uniform [Lipschitz constant](../../../../../lipschitz-constant.md) $L=1$. In the quantitative [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md), the independent-variable half-width and the dependent-variable radius are both one, so

$$
h=\min\{1,1/1\}=1.
$$

Therefore

$$
\boxed{\text{There is a unique solution for every }x\in[-1,1].}
$$

The global derivative bound also makes the cube condition explicit. Along any solution segment starting at the initial point,

$$
\|Y(x)-B\|_\infty
=\left\|\int_0^xF(s,Y(s))\,ds\right\|_\infty\leq|x|.
$$

Thus it cannot leave the dependent-variable ball before $|x|=1$. Bounded derivatives give limiting endpoint values, and local existence extends to them because $F$ is defined continuously on all space. Uniform Lipschitz continuity ensures that all such local pieces agree on overlaps, proving uniqueness throughout the closed interval.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [7](../../7.md)
3. [Differential Equations](../../../differential-equations.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
