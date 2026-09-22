<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [linear system of differential equations](../../../../linear-system-of-differential-equations.md) has [matrix](../../../../matrix.md)

$$
M=\begin{pmatrix}0&\alpha\\-\alpha&0\end{pmatrix},\qquad
C=\begin{pmatrix}1&1\\i&-i\end{pmatrix},\qquad C^{-1}MC=\begin{pmatrix}i\alpha&0\\0&-i\alpha\end{pmatrix}.
$$

The columns of $C$ are [eigenvectors](../../../../eigenvector.md) of $M$. The [change of basis](../../../../change-of-basis.md) $v'=C^{-1}v$ therefore gives $v'_1=(v_1-iv_2)/2$, $v'_2=(v_1+iv_2)/2$, with independent [first-order linear differential equations](../../../../first-order-linear-differential-equation.md)

$$
\dot v'_1=i\alpha v'_1,\quad \dot v'_2=-i\alpha v'_2,\qquad
v'_1(t)=K_+e^{i\alpha t},\quad v'_2(t)=K_-e^{-i\alpha t}.
$$

The initial [velocity](../../../../velocity.md) gives $K_+=-iv_0/2$, $K_-=iv_0/2$. Transforming back, $v=Cv'$, yields the real [velocity](../../../../velocity.md) [vector components](../../../../coordinate-linear-algebra.md)

$$
\boxed{v_1(t)=v_0\sin\alpha t,\qquad v_2(t)=v_0\cos\alpha t.}
$$

These also cover $\alpha=0$. Complex [coordinates](../../../../coordinate-linear-algebra.md) have decoupled a real rotation without making the physical [velocity](../../../../velocity.md) complex.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
