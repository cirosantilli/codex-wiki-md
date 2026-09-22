<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the dark, energy minimization gives $h_{xx}=-H_0$. Translation and rotation are zero-energy freedoms; one representative is $h_-(x)=-H_0x^2/2$. After illumination, choose the equivalent light-adapted equilibrium

$$
h_+(x)=\frac{H_0x^2}{2}-H_0Lx+\frac{H_0L^2}{6}.
$$

Then $u=h-h_+$ has homogeneous free-end conditions $u_{xx}=u_{xxx}=0$, and its initial value

$$
u(x,0)=-H_0\left(x^2-Lx+\frac{L^2}{6}\right)
$$

is orthogonal to the two rigid zero modes $1$ and $x$.

Let $q_n>0$ solve the [free--free biharmonic eigenvalue equation](../../../../../../free-free-biharmonic-eigenvalue-equation.md)

$$
\cos(q_nL)\cosh(q_nL)=1,
$$

and choose

$$
\phi_n(x)=\cosh(q_nx)+\cos(q_nx)
-\frac{\cosh(q_nL)-\cos(q_nL)}{\sinh(q_nL)+\sin(q_nL)}
[\sinh(q_nx)-\sin(q_nx)].
$$

These are orthogonal eigenfunctions of the [biharmonic operator](../../../../../../biharmonic-operator.md) with $\phi_n''=\phi_n'''=0$ at both ends. The shape is

$$
\boxed{h(x,t)=h_+(x)+\sum_{n=1}^{\infty}a_n\phi_n(x)
e^{-Aq_n^4t/\zeta},}
$$

where

$$
a_n=\frac{\int_0^L u(x,0)\phi_n(x)dx}
{\int_0^L\phi_n(x)^2dx}.
$$

The omitted zero modes would only translate or rotate the whole filament.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 355](../../../paper-355-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
