<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $g=\dot\gamma$ and

$$
\mathbf L=\nabla\mathbf u
=\begin{pmatrix}0&g&0\\0&0&0\\0&0&0\end{pmatrix},
\qquad
\boldsymbol\tau=
\begin{pmatrix}
\tau_{xx}&\tau_{xy}&0\\
\tau_{xy}&\tau_{yy}&0\\
0&0&\tau_{zz}
\end{pmatrix}.
$$

The flow and stresses are steady and homogeneous, so the material derivative vanishes. Direct multiplication gives

$$
\boxed{
\overset{\triangledown}{\boldsymbol\tau}
=-\mathbf L\boldsymbol\tau
-\boldsymbol\tau\mathbf L^T
=\begin{pmatrix}
-2g\tau_{xy}&-g\tau_{yy}&0\\
-g\tau_{yy}&0&0\\
0&0&0
\end{pmatrix}}
$$

and

$$
\boxed{
\boldsymbol\tau^2=
\begin{pmatrix}
\tau_{xx}^2+\tau_{xy}^2&
\tau_{xy}(\tau_{xx}+\tau_{yy})&0\\
\tau_{xy}(\tau_{xx}+\tau_{yy})&
\tau_{xy}^2+\tau_{yy}^2&0\\
0&0&\tau_{zz}^2
\end{pmatrix}}.
$$

Since $\dot\gamma_{xy}=\dot\gamma_{yx}=g$, the four independent component equations are

$$
\boxed{\tau_{xx}-2\lambda g\tau_{xy}
+\frac{\alpha\lambda}{\eta}(\tau_{xx}^2+\tau_{xy}^2)=0},
$$



$$
\boxed{\tau_{xy}-\lambda g\tau_{yy}
+\frac{\alpha\lambda}{\eta}
\tau_{xy}(\tau_{xx}+\tau_{yy})=\eta g},
$$



$$
\boxed{\tau_{yy}
+\frac{\alpha\lambda}{\eta}
(\tau_{xy}^2+\tau_{yy}^2)=0},
\qquad
\boxed{\tau_{zz}
+\frac{\alpha\lambda}{\eta}\tau_{zz}^2=0}.
$$

The branch continuous from equilibrium has $\tau_{zz}=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
