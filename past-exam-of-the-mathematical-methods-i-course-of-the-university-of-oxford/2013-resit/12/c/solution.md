<h1 id="12/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [characteristic polynomial](../../../../characteristic-polynomial.md) of the homogeneous constant-coefficient equation is $r^2+2r+2$, with roots $-1\pm i$. Its real [complementary function](../../../../homogeneous-solution.md) is therefore $e^{-x}(C_1\cos x+C_2\sin x)$. The forcing $e^{-x}$ is not resonant because $r=-1$ is not a root. Substituting $y_p=Ae^{-x}$ into the differential operator gives $Ae^{-x}$, so $A=1$. Hence

$$
\boxed{y=e^{-x}\left(C_1\cos x+C_2\sin x+1\right).}
$$

A useful independent check is the substitution $y=e^{-x}v$: the equation becomes $v''+v=1$, whose general solution is $v=C_1\cos x+C_2\sin x+1$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [12](../../12.md)
3. [2013 resit](../../../2013-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
