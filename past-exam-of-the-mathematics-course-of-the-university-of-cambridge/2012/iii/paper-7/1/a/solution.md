<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $(y,w)$ to label the initial point in [phase space](../../../../../../phase-space.md). The [characteristic equations for a transport equation](../../../../../../characteristic-equations-for-a-transport-equation.md) are $\dot X=a(V)$ and $\dot V=0$, with $X(s)=y$ and $V(s)=w$. Since the [velocity](../../../../../../velocity.md) remains fixed, the [ordinary differential equations](../../../../../../ordinary-differential-equation.md) integrate directly:

$$
\boxed{S_{s,t}(y,w)=(y+(t-s)a(w),w).}
$$

This [characteristic flow map](../../../../../../characteristic-flow-map.md) exists for all real times, even if $a$ grows rapidly at infinity: each trajectory samples just one fixed velocity. Its inverse is $S_{t,s}$, and its [Jacobian matrix](../../../../../../jacobian-matrix.md) is the block triangular matrix

$$
D S_{s,t}=
\begin{pmatrix}I&(t-s)Da(w)\\0&I\end{pmatrix}.
$$

Consequently its [Jacobian determinant](../../../../../../jacobian-determinant.md) is one. The nonzero [Jacobian determinant](../../../../../../jacobian-determinant.md) of $a$ is unnecessary for this construction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
