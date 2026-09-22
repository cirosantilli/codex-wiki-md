<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $J$ equal intervals, $h=1/J$, and the interior [piecewise-linear hat functions](../../../../../../piecewise-linear-hat-function.md) $\phi_j$, which equal one at node $j$, vanish at all other nodes and vanish outside the two adjacent intervals. Write $u_h(x,t)=\sum_{j=1}^{J-1}U_j(t)\phi_j(x)$. Testing with $\phi_i$ and integrating the second [derivative](../../../../../../derivative.md) by parts gives

$$
\sum_j\left(\int_0^1\phi_i\phi_jdx\right)\dot U_j
=-\sum_j\left(\int_0^1\phi_i'\phi_j'dx\right)U_j.
$$

The integrals are local: $\int\phi_i^2=2h/3$, $\int\phi_i\phi_{i+1}=h/6$, $\int(\phi_i')^2=2/h$ and $\int\phi_i'\phi_{i+1}'=-1/h$. Nonadjacent functions do not overlap. Thus the consistent [mass matrix](../../../../../../mass-matrix.md) and [stiffness matrix](../../../../../../stiffness-matrix.md) are

$$
M=\frac h6\operatorname{tridiag}(1,4,1),\qquad
K=\frac1h\operatorname{tridiag}(-1,2,-1),\qquad \boxed{M\dot U+KU=0.}
$$

Equivalently the explicit nodal equations are

$$
\boxed{\dot U_{j-1}+4\dot U_j+\dot U_{j+1}
=\frac6{h^2}(U_{j-1}-2U_j+U_{j+1}),\quad U_0=U_J=0.}
$$

For merely L2 initial data a natural choice is the Galerkin projection $MU(0)=((v,\phi_i))_i$; nodal interpolation is also possible for suitably smooth data. The relation $U^TMU=\|u_h\|_{L^2}^2$ identifies the natural finite-element energy. Differentiating gives $d(U^TMU)/dt=-2U^TKU\leq0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
