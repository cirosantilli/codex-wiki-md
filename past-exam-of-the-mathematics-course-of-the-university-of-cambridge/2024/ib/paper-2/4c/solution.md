<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

Vanishing net [charge density](../../../../../charge-density.md) does not require vanishing current. Positive and negative charge carriers can cancel in [charge density](../../../../../charge-density.md) while their oppositely directed motions add to a nonzero current. Charge conservation only requires

$$
\partial_t\rho+\nabla\cdot J=0;
$$

for magnetostatics this becomes $\nabla\cdot J=0$.

Because $\nabla\cdot B=0$, one may introduce a [magnetic vector potential](../../../../../magnetic-vector-potential.md) with

$$
B=\nabla\times A.
$$

It is not unique: $A+\nabla\chi$ gives the same field for any [scalar](../../../../../scalar.md) $\chi$.

For the stated current,

$$
\nabla\cdot J=0,
$$

so it is consistent with stationary charge conservation. Direct calculation gives

$$
\nabla\times J
=\lambda J_0(\sin\lambda z,\cos\lambda z,0)
=\lambda J.
$$

Thus $J$ is a [Beltrami field](../../../../../beltrami-field.md). For $\lambda\ne0$, choose

$$
\boxed{B=\frac{\mu_0}{\lambda}J}.
$$

Then $\nabla\cdot B=0$ and $\nabla\times B=\mu_0J$. A convenient Coulomb-gauge potential is

$$
\boxed{A=\frac{\mu_0}{\lambda^2}J},
$$

since $\nabla\times A=B$ and $\nabla\cdot A=0$. [Gradient](../../../../../gradient.md) gauge terms may of course be added.

If $\lambda=0$, the current is the constant field $J=(0,J_0,0)$. The formulas involving $1/\lambda$ do not apply; one valid choice is

$$
\boxed{B=(0,0,-\mu_0J_0x),
\qquad
A=\left(0,-\frac12\mu_0J_0x^2,0\right).}
$$

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
