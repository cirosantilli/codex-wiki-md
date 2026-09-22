<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Reflection symmetry makes the two outer free tails identical. Their combined energy is

$$
E_o=\frac{k_c\delta_o^2}{\xi R^2}.
$$

Between the cylinders the free profile is even. Up to an irrelevant additive height it has the form

$$
h_i(x)=C\cosh(x/\xi),
\qquad |x|\leq L-\delta_i.
$$

Slope matching at $x=L-\delta_i$ gives

$$
C=\frac{\xi\delta_i}{R\sinh[(L-\delta_i)/\xi]}.
$$

Direct integration, or the boundary expression from part (a), yields

$$
E_i=\frac{k_c\delta_i^2}{\xi R^2}
\coth\frac{L-\delta_i}{\xi}.
$$

At the retained order $\delta_i/\xi\ll1$, replace the argument by $L/\xi$. The four contact halves contribute bending plus adhesion energy

$$
E_c=\frac{k_c}{R^2}(1-2U)(\delta_o+\delta_i).
$$

Thus

$$
E_2=\frac{k_c}{\xi R^2}
\left[\delta_o^2+\delta_i^2\coth(L/\xi)
-2\xi\left(U-\frac12\right)(\delta_o+\delta_i)
\right].
$$

Independent minimization gives

$$
\delta_o=\xi\left(U-\frac12\right),
\qquad
\delta_i=\xi\left(U-\frac12\right)\tanh(L/\xi),
$$

and hence

$$
E_2(L)=-\frac{k_c\xi}{R^2}
\left(U-\frac12\right)^2
\left[1+\tanh(L/\xi)\right].
$$

At infinite separation the energy is twice the one-cylinder minimum. The [membrane-mediated interaction potential](../../../../../../membrane-mediated-interaction-potential.md) is therefore

$$
\boxed{
V(L)=E_2(L)-E_2(\infty)
=\frac{k_c\xi}{R^2}
\left(U-\frac12\right)^2
\left[1-\tanh(L/\xi)\right]
}.
$$

It is positive and decreases monotonically to zero, so the two cylinders repel. The physical cause is the overlap of their exponentially relaxing membrane deformations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 355](../../../paper-355-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
