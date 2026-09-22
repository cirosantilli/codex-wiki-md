<h1 id="b/8/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Test with $v_h=u_h^{m+1}$ and apply $2(a-b,a)=\|a\|^2-\|b\|^2+\|a-b\|^2$. The exact energy identity is

$$
\frac{\|u_h^{m+1}\|_2^2-\|u_h^m\|_2^2+\|u_h^{m+1}-u_h^m\|_2^2}{2\Delta t}
+\|(u_h^{m+1})'\|_2^2+\|u_h^{m+1}\|_2^2=0.
$$

The printed identity omits the last reaction contribution while explicitly describing its last term as the $H^1$ seminorm. **It requires the full $H^1$ [norm](../../../../../norm.md) instead of that seminorm.** With the printed seminorm its left side equals $-\|u_h^{m+1}\|_2^2$, rather than zero. The source reaction term forces this correction.

All terms other than the difference of successive squared [norms](../../../../../norm.md) are nonnegative. Consequently

$$
\boxed{\|u_h^m\|_2\leq\|u_h^0\|_2\leq\|u_0\|_2.}
$$

The second inequality uses contractivity of the initial [orthogonal projection](../../../../../orthogonal-projection.md). No restriction relates $\Delta t$ to $h$, giving unconditional stability. The retained reaction term strengthens dissipation.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
