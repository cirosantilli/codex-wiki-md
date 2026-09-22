<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Take the constant speed parameter $v\ne0$, so $r=x+vt$ and $s=x-vt$ are independent [characteristic coordinates](../../../characteristic-coordinate.md). The [chain rule](../../../chain-rule.md) gives

$$
\partial_x=\partial_r+\partial_s,\qquad\partial_t=v(\partial_r-\partial_s).
$$

Applying these operators twice to a twice differentiable [function](../../../function-split.md) yields

$$
F_{xx}=F_{rr}+2F_{rs}+F_{ss},\qquad F_{tt}=v^2(F_{rr}-2F_{rs}+F_{ss}).
$$

Consequently the [wave equation](../../../wave-equation-split.md) reduces to $4F_{rs}=0$. Integrate first with respect to $s$, obtaining $F_r=A(r)$, and then with respect to $r$, allowing a separate integration [function](../../../function-split.md) of $s$. The general local solution is

$$
\boxed{F(x,t)=G(x+vt)+H(x-vt)},
$$

with arbitrary sufficiently differentiable [functions](../../../function-split.md) $G$ and $H$. For $v>0$, the first profile travels towards negative $x$ and the second towards positive $x$. Substitution directly checks the equation. Initial or boundary conditions select the two profiles; none are specified here. This is [D'Alembert's formula](../../../d-alembert-s-formula.md) in characteristic form.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2015](../../2015-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
