<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate the constraint to obtain $z'=2t-x'-y'$ and eliminate $z'$ from the other equations. Adding the resulting equations gives $y'=t-x+y/2$, and substitution then gives $x'+x=2t$. Its [integrating factor](../../../../integrating-factor.md) is $e^t$, so $x=2t-2+C_1e^{-t}$; the initial value fixes $C_1=4$.

The remaining equation is $y'-y/2=-t+2-4e^{-t}$. Its integrating factor is $e^{-t/2}$, giving $y=2t+(8/3)e^{-t}+C_2e^{t/2}$; the initial value fixes $C_2=0$. Finally use the constraint:

$$
\boxed{\begin{aligned}
x(t)&=2t-2+4e^{-t},\\
y(t)&=2t+\frac83e^{-t},\\
z(t)&=t^2-4t+2-\frac{20}3e^{-t}.
\end{aligned}}
$$

The [acceleration](../../../../acceleration.md) is $(4e^{-t},(8/3)e^{-t},2-(20/3)e^{-t})$, which is not constant. Thus **a constant net force cannot maintain this motion for a particle of constant mass**, by [Newton's second law](../../../../newton-s-second-law.md). This conclusion concerns the net force in the stated inertial-coordinate interpretation; a time-dependent force can produce it.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [11](../../11.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
