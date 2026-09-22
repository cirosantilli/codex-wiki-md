<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

Let each mass be $m$ and each spring constant be $k$, with the $x_i$ denoting longitudinal displacements from equilibrium. The [Lagrangian](../../../../../lagrangian.md) is

$$
L=\frac m2\sum_{i=1}^4\dot x_i^2
-\frac k2\left[(x_2-x_1)^2+(x_3-x_2)^2+(x_4-x_3)^2\right].
$$

The inverse coordinate transformation is

$$
x_1=q_1+q_3,\quad x_4=q_1-q_3,\quad
x_2=q_2+q_4,\quad x_3=q_2-q_4.
$$

Substitution gives

$$
\boxed{
L=m(\dot q_1^2+\dot q_2^2+\dot q_3^2+\dot q_4^2)
-k\left[(q_2-q_1)^2+(q_4-q_3)^2+2q_4^2\right]}.
$$

Thus the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) separate into a symmetric pair,

$$
m\ddot q_1+k(q_1-q_2)=0,
\qquad
m\ddot q_2+k(q_2-q_1)=0,
$$

and an antisymmetric pair,

$$
m\ddot q_3+k(q_3-q_4)=0,
\qquad
m\ddot q_4+k(3q_4-q_3)=0.
$$

The symmetric [normal modes](../../../../../normal-mode.md) are:


- $q_1=q_2$, corresponding to $(x_1,x_2,x_3,x_4)\propto(1,1,1,1)$ and the translational frequency


$$
\boxed{\omega_0=0};
$$


- $q_1=-q_2$, corresponding to $(1,-1,-1,1)$ and


$$
\boxed{\omega_{\rm s}=\sqrt{\frac{2k}{m}}}.
$$

For antisymmetric modes, the squared dimensionless frequencies are the eigenvalues of

$$
\begin{pmatrix}1&-1\\-1&3\end{pmatrix},
$$

namely $2\mp\sqrt2$. They give

$$
\boxed{\omega_-=\sqrt{\frac{k}{m}(2-\sqrt2)}},
\qquad
(q_3,q_4)\propto(1,\sqrt2-1),
$$

and

$$
\boxed{\omega_+=\sqrt{\frac{k}{m}(2+\sqrt2)}},
\qquad
(q_3,q_4)\propto(1,-1-\sqrt2).
$$

In the original coordinates their mode shapes are respectively

$$
(1,\sqrt2-1,1-\sqrt2,-1)
$$

and

$$
(1,-1-\sqrt2,1+\sqrt2,-1).
$$

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
