<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $h=1/(N+1)$ and $x_i=ih$. The interior [piecewise-linear hat functions](../../../../../../piecewise-linear-hat-function.md) are

$$
\phi_i(x)=
\begin{cases}
(x-x_{i-1})/h,&x_{i-1}\leq x\leq x_i,\\
(x_{i+1}-x)/h,&x_i\leq x\leq x_{i+1},\\
0,&\text{otherwise}.
\end{cases}
$$

They are a [basis](../../../../../../basis.md) of the continuous piecewise-affine functions vanishing at both endpoints. The [support of a function](../../../../../../support.md) for each hat only overlaps those of neighbouring hats, so the [stiffness matrix](../../../../../../stiffness-matrix.md) is a [tridiagonal matrix](../../../../../../tridiagonal-matrix.md). Direct [integration](../../../../../../integral.md) gives the [derivative](../../../../../../derivative.md) contribution $2/h$ on the diagonal and $-1/h$ on adjacent diagonals.

For the potential contribution, symmetry about $x_i$ gives $\int x\phi_i^2\,dx=x_i\int\phi_i^2\,dx=2hx_i/3$. On the overlap of $\phi_i$ and $\phi_{i+1}$, their product is symmetric about $(x_i+x_{i+1})/2$, and its [integral](../../../../../../integral.md) is $h/6$. This is the [affine-weighted hat mass matrix](../../../../../../affine-weighted-hat-mass-matrix.md) calculation. Consequently,

$$
\boxed{
A_{ii}=\frac2h+\frac{2hx_i}{3},\qquad
A_{i,i+1}=A_{i+1,i}=-\frac1h+\frac{h(x_i+x_{i+1})}{12}
}
$$

and all other entries vanish. The exact right-hand side is

$$
b_i=\frac1h\int_{x_{i-1}}^{x_i}(x-x_{i-1})f(x)\,dx
+\frac1h\int_{x_i}^{x_{i+1}}(x_{i+1}-x)f(x)\,dx.
$$

Thus, with $c_0=c_{N+1}=0$, the requested scalar equations are

$$
\begin{aligned}
\left(-\frac1h+\frac{h(x_{i-1}+x_i)}{12}\right)c_{i-1}
+\left(\frac2h+\frac{2hx_i}{3}\right)c_i
+\left(-\frac1h+\frac{h(x_i+x_{i+1})}{12}\right)c_{i+1}
=b_i,\quad 1\leq i\leq N.
\end{aligned}
$$

At the endpoints the coefficient multiplying the zero boundary value is simply omitted. Since $f\in L^2$, its point values are not even well defined; replacing $b_i$ by $hf(x_i)$ would require an additional [quadrature rule](../../../../../../quadrature-rule.md) convention and regularity hypothesis, not present here. The exact [Ritz method](../../../../../../rayleigh-ritz-method.md) uses the displayed [integrals](../../../../../../integral.md). The [finite element interpolation estimate](../../../../../../finite-element-interpolation-estimate.md) and [Céa lemma](../../../../../../cea-s-lemma.md), using $y\in H^2$, give an $O(h)$ [energy norm](../../../../../../energy-norm.md) error; the [Aubin–Nitsche duality argument](../../../../../../aubin-nitsche-duality-argument.md) gives $O(h^2)$ in the [L2 norm](../../../../../../l2-norm.md) on this interval.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
