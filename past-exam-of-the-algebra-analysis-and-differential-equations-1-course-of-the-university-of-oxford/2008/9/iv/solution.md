<h1 id="9/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Applying the derivative rule twice and using both zero initial data gives

$$
(p^2+1)\bar x(p)=\frac1{p^2+1},
$$

so $\bar x(p)=1/(p^2+1)^2$. By the [convolution theorem for Laplace transforms](../../../../convolution-theorem-for-laplace-transforms.md),

$$
x(t)=\int_0^t\sin s\,\sin(t-s)\,ds.
$$

Use the product-to-sum identity $\sin s\sin(t-s)=\frac12[\cos(2s-t)-\cos t]$ to integrate:

$$
\boxed{x(t)=\tfrac12(\sin t-t\cos t).}
$$

It satisfies $x(0)=x'(0)=0$, and differentiation gives $x''+x=\sin t$. The term proportional to $t\cos t$ is the resonant response of the forced [harmonic oscillator](../../../../simple-harmonic-motion.md).

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [9](../../9.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
