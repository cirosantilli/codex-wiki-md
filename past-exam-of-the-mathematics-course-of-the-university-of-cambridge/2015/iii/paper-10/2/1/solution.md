<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

One version of the [Klainerman-Sobolev inequality](../../../../../../klainerman-sobolev-inequality.md), for a sufficiently decaying [smooth function](../../../../../../smooth-function.md) $\psi$ on $\mathbb R^{1+3}$, is

$$
\boxed{|\psi(t,x)|\leq
\frac{C}{(1+t+|x|)(1+|t-|x||)^{1/2}}
\sum_{|I|\leq2}\|Z^I\psi(t,\cdot)\|_{L^2(\mathbb R^3)}},\qquad t\geq0.
$$

Here $I$ denotes a word of length $|I|$ in the following eleven [commutation vector fields for the wave equation](../../../../../../commutation-vector-field-for-the-wave-equation.md):

$$
\begin{aligned}
&\partial_t,\ \partial_1,\ \partial_2,\ \partial_3, &&\text{spacetime translations},\\
&\Omega_{ij}=x_i\partial_j-x_j\partial_i\quad(1\leq i<j\leq3), &&\text{spatial rotations},\\
&L_i=t\partial_i+x_i\partial_t\quad(1\leq i\leq3), &&\text{Lorentz boosts},\\
&S=t\partial_t+\sum_{i=1}^3x_i\partial_i, &&\text{scaling}.
\end{aligned}
$$

The first four are [spacetime translation vector fields](../../../../../../spacetime-translation-vector-field.md); the next three are [spatial rotation vector fields](../../../../../../spatial-rotation-vector-field.md); the next three are [Lorentz boost vector fields](../../../../../../lorentz-boost-vector-field.md); and $S$ is the [scaling vector field](../../../../../../scaling-vector-field.md). The [vector field method for wave equations](../../../../../../vector-field-method-for-wave-equations.md) uses these [vector fields](../../../../../../vector-field.md) because their [commutators](../../../../../../commutator.md) with the [d'Alembert operator](../../../../../../d-alembert-operator.md) obey

$$
[\Box,Z]=0\quad(Z\ne S),\qquad [\Box,S]=2\Box.
$$

In particular the [Klainerman-Sobolev inequality](../../../../../../klainerman-sobolev-inequality.md) implies

$$
\|\psi(t,\cdot)\|_\infty\leq\frac{C}{1+t}\sum_{|I|\leq2}\|Z^I\psi(t,\cdot)\|_2.
$$

The displayed [L2 norms](../../../../../../l2-norm.md) are spatial norms at fixed time; the spacetime [vector fields](../../../../../../vector-field.md) can contain time derivatives. No [wave equation](../../../../../../wave-equation-split.md) assumption is needed for the [Klainerman-Sobolev inequality](../../../../../../klainerman-sobolev-inequality.md) itself.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
