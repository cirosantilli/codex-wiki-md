<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The right-handed [material frame of a rod](../../../../../material-frame-of-a-rod.md) has $\mathbf d_2\times\mathbf d_1=-\mathbf d_3$ and $\mathbf d_2\times\mathbf d_3=\mathbf d_1$. Hence the [director kinematics of a rod](../../../../../director-kinematics-of-a-rod.md) reduce to

$$
\mathbf d_1'=-\hat u\mathbf d_3,\qquad
\mathbf d_3'=\hat u\mathbf d_1,\qquad \mathbf d_2=\mathbf e_2.
$$

Solving these constant-coefficient [ordinary differential equations](../../../../../ordinary-differential-equation.md) with the given initial frame gives

$$
\boxed{\begin{aligned}
\mathbf d_1(S)&=\cos(\hat u S)\mathbf e_1-\sin(\hat u S)\mathbf e_3,\\
\mathbf d_3(S)&=\sin(\hat u S)\mathbf e_1+\cos(\hat u S)\mathbf e_3.
\end{aligned}}
$$

The [inextensible rod](../../../../../inextensible-rod.md) has $\mathbf r'=\mathbf d_3$. An [integration](../../../../../integral-split.md) using $\mathbf r(0)=\mathbf0$ yields, for $\hat u\ne0$,

$$
\boxed{\mathbf r(S)=\frac{1-\cos(\hat u S)}{\hat u}\mathbf e_1
+\frac{\sin(\hat u S)}{\hat u}\mathbf e_3.}
$$

Indeed,

$$
\left|\mathbf r(S)-\frac{\mathbf e_1}{\hat u}\right|^2=\frac1{\hat u^2},
$$

so the centreline is a [circular arc](../../../../../circular-arc.md) of radius $1/|\hat u|$ in the plane perpendicular to $\mathbf e_2$. The continuous $\hat u\to0$ limit is $\mathbf d_1=\mathbf e_1$, $\mathbf d_3=\mathbf e_3$, and $\mathbf r=S\mathbf e_3$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the mathematical mechanical biology course of the University of Oxford](../../../../split.md)
6. [Mathematical mechanical biology course of the University of Oxford](../../../../../mathematical-mechanical-biology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
