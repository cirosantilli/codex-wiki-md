<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the [minimal surface equation for a graph](../../../../../../minimal-surface-equation-for-a-graph.md) as $\operatorname{div}F(Du)=0$ in its [weak formulation](../../../../../../weak-formulation.md), where $F(p)=p/\sqrt{1+|p|^2}$. For negative increments use the same [difference quotient](../../../../../../difference-quotient.md) convention, so

$$
w_h=\delta_{\ell,-h}u=\frac{u(x)-u(x-he_\ell)}h.
$$

For $\zeta\in C_c^1(\Omega'')$, the function $\delta_{\ell,h}\zeta$ is an admissible [test function](../../../../../../test-function.md) in $\Omega$. Commuting the first [partial derivative](../../../../../../partial-derivative.md) with translation, then applying [discrete integration by parts](../../../../../../discrete-integration-by-parts.md), gives

$$
0=\int_\Omega F_i(Du)\delta_{\ell,h}(D_i\zeta)
=-\int_{\Omega''}\delta_{\ell,-h}(F_i(Du))D_i\zeta.
$$

The [fundamental theorem of calculus along a line segment](../../../../../../fundamental-theorem-of-calculus-along-a-line-segment.md) gives the [averaged linearization of a nonlinear divergence-form equation](../../../../../../averaged-linearization-of-a-nonlinear-divergence-form-equation.md)

$$
\delta_{\ell,-h}(F_i(Du))=A_h^{ij}(x)D_jw_h,
\qquad
A_h(x)=\int_0^1DF\bigl((1-t)Du(x-he_\ell)+tDu(x)\bigr)\,dt.
$$

Thus **the backward difference quotient solves a linear equation in divergence form**:

$$
\boxed{D_i(A_h^{ij}D_jw_h)=0\quad\text{weakly on }\Omega''.}
$$

To verify the [ellipticity of the minimal surface flux](../../../../../../ellipticity-of-the-minimal-surface-flux.md), compute

$$
DF(p)=\frac{I}{\sqrt{1+|p|^2}}-\frac{p\otimes p}{(1+|p|^2)^{3/2}},
$$

and hence

$$
\frac{|\xi|^2}{(1+|p|^2)^{3/2}}
\leq \xi\cdot DF(p)\xi
\leq |\xi|^2.
$$

The [eigenvalue](../../../../../../eigenvalue.md) parallel to $p$ is $(1+|p|^2)^{-3/2}$; every orthogonal [eigenvalue](../../../../../../eigenvalue.md) is $(1+|p|^2)^{-1/2}$. The same lower and upper bounds pass to the averaged [symmetric matrix](../../../../../../symmetric-matrix.md) $A_h$ whenever both endpoint [gradients](../../../../../../gradient.md) have norm at most $M$:

$$
\boxed{(1+M^2)^{-3/2}|\xi|^2\leq A_h^{ij}\xi_i\xi_j\leq|\xi|^2.}
$$

The printed $C^1(\Omega)$ hypothesis supplies such an $M$ on each [relatively compact subset](../../../../../../relatively-compact-subset.md), uniformly for sufficiently small $h$. It therefore establishes a locally [uniformly elliptic operator](../../../../../../uniformly-elliptic-operator.md). A single lower bound on all of $\Omega''$ additionally requires bounded [gradients](../../../../../../gradient.md) there and at the shifted points; this is automatic for bounded $\Omega$ and fixed $h$, but is not supplied on an arbitrary open set.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
