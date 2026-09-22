<h1 id="6b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $y<0$, the [Heaviside function](../../../../../../heaviside-step-function.md) vanishes, so $w=Ay+B$. For $y>0$, $w''=-1$, giving $w=-y^2/2+Cy+D$. Continuity of $w$ and $w'$ at zero requires $D=B$ and $C=A$. Consequently the general continuously differentiable profile is

$$
\boxed{w(y)=Ay+B-\frac12(y_+)^2,\qquad y_+=\max(y,0).}
$$

Its second derivative jumps from zero to minus one. The equation is satisfied classically away from zero and in the weak, or distributional, sense across it; no globally twice-differentiable function can have the prescribed step as its second derivative. There is no [Dirac delta](../../../../../../dirac-delta-function.md) contribution because $w'$ is continuous. The value assigned to the [Heaviside function](../../../../../../heaviside-step-function.md) at a single point does not change this weak solution.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6B](../../6b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
