<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [characteristic equation](../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) of the homogeneous [ordinary differential equation](../../../../ordinary-differential-equation.md) is $r^2-2r+5=0$, with roots $1\pm2i$. Therefore $y_h=e^x(C\cos2x+D\sin2x)$. For the forcing term, try the [particular solution](../../../../particular-solution.md) $y_p=e^{-x}(ax+b)$. Substitution gives $8a=1$, $8b-4a=0$, so $a=1/8$, $b=1/16$. The two initial conditions give $C=-1/16$ and $D=0$. Consequently

$$
\boxed{y(x)=\frac{(2x+1)e^{-x}-e^x\cos2x}{16}.}
$$

Both the value and the first derivative vanish at zero; direct differentiation verifies the inhomogeneous equation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
