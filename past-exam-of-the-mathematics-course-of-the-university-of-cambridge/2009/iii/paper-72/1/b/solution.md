<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take a uniform [finite element mesh](../../../../../../finite-element-mesh.md) $x_i=ih$, $0\leq i\leq J$, $h=1/J$, and interior [piecewise-linear hat functions](../../../../../../piecewise-linear-hat-function.md) $\phi_i$. Write $u_h=\sum_{i=1}^{J-1}U_i\phi_i$. The [Ritz method](../../../../../../rayleigh-ritz-method.md) gives $KU=F$ with

$$
K_{ij}=\int_0^1\phi_i'\phi_j'\,dx+\int_0^1x\phi_i\phi_j\,dx,
\qquad F_i=-\int_0^1\phi_i\,dx=-h.
$$

The derivative part has diagonal $2/h$, neighboring entries $-1/h$ and zero other entries. For the [affine-weighted hat mass matrix](../../../../../../affine-weighted-hat-mass-matrix.md), symmetry around $x_i$ gives

$$
\int x\phi_i^2\,dx=\frac{2h}{3}x_i.
$$

On $[x_i,x_{i+1}]$, the product of the two hats is symmetric about the midpoint, integrates to $h/6$, and therefore has weighted integral

$$
\int x\phi_i\phi_{i+1}\,dx=\frac h{12}(x_i+x_{i+1}).
$$

Consequently the explicit [tridiagonal](../../../../../../tridiagonal-matrix.md) equations are

$$
\boxed{\left[-\frac1h+\frac h{12}(x_{i-1}+x_i)\right]U_{i-1}
+\left[\frac2h+\frac{2h}3x_i\right]U_i
+\left[-\frac1h+\frac h{12}(x_i+x_{i+1})\right]U_{i+1}=-h,}
$$

for $1\leq i\leq J-1$, with $U_0=U_J=0$. The reaction coefficient has been integrated exactly; replacing it by an unweighted constant [mass matrix](../../../../../../mass-matrix.md) would give a different system. For a nonzero coefficient [vector](../../../../../../vector.md), the represented function is nonzero and $U^TKU=a(u_h,u_h)>0$, so the [matrix](../../../../../../matrix.md) is symmetric [positive-definite](../../../../../../positive-definite-bilinear-form.md) and the algebraic solution is unique.

Uniform spacing is a choice, not a requirement of the method. On a general [finite element mesh](../../../../../../finite-element-mesh.md) with $h_i=x_i-x_{i-1}$, the corresponding entries are

$$
K_{ii}=\frac1{h_i}+\frac1{h_{i+1}}
+\frac{h_i}{12}(x_{i-1}+3x_i)
+\frac{h_{i+1}}{12}(3x_i+x_{i+1}),
$$



$$
K_{i,i+1}=-\frac1{h_{i+1}}+
\frac{h_{i+1}}{12}(x_i+x_{i+1}),\qquad
F_i=-\frac{h_i+h_{i+1}}2,
$$

with symmetric lower entries. These reduce to the displayed uniform-grid system.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
