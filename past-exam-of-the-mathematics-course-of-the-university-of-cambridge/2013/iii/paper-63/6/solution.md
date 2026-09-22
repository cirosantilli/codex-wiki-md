<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [Engquist-Osher method](../../../../../engquist-osher-method.md) is a conservative [finite volume method](../../../../../finite-volume-method.md) built by separating positive and negative characteristic speeds. Take $f\in C^1$, a uniform cell width $d$, a time step $k$, and cell averages $U_j^n$. Write $\lambda=k/d$ and define the [numerical flux](../../../../../numerical-flux.md)

$$
F(a,b)=f(0)+\int_0^a\max(f'(s),0)\,ds
+\int_0^b\min(f'(s),0)\,ds.
$$

The [Engquist-Osher flux](../../../../../engquist-osher-flux.md) uses the left state for right-going transport and the right state for left-going transport. Its conservative update is

$$
U_j^{n+1}=U_j^n-\lambda\bigl(F(U_j^n,U_{j+1}^n)-F(U_{j-1}^n,U_j^n)\bigr).
$$

It is consistent because $F(u,u)=f(u)$. The integrals have their ordinary oriented meaning even for negative states. For the [Inviscid Burgers equation](../../../../../inviscid-burgers-equation.md), $f(u)=u^2/2$ gives the useful example

$$
F(a,b)=\frac12\max(a,0)^2+\frac12\min(b,0)^2.
$$

In a region where all characteristic speeds have one sign, the flux reduces to the corresponding upwind flux. In smooth regions, this basic piecewise-constant, forward-time version is first order in space and time; its main virtue is robust nonlinear [stability](../../../../../stability-of-a-numerical-method.md) across shocks.

Here is a precise [stability](../../../../../stability-of-a-numerical-method.md) proof. Assume the data lie in a bounded interval $J=[m,M]$ and choose

$$
\boxed{\lambda\sup_{s\in J}|f'(s)|\leq1.}
$$

Work on a periodic grid, or on the infinite grid with summable differences; on a finite interval the inflow boundary data and boundary fluxes must be treated monotonically as well. Define the three-point update map

$$
H(a,b,c)=b-\lambda\bigl(F(b,c)-F(a,b)\bigr).
$$

Writing $f'_+=\max(f',0)$ and $f'_- =\min(f',0)$, its three partial derivatives are

$$
H_a=\lambda f'_+(a)\geq0,\qquad
H_b=1-\lambda|f'(b)|\geq0,\qquad
H_c=-\lambda f'_-(c)\geq0.
$$

Thus it is a [monotone conservative scheme](../../../../../monotone-conservative-scheme.md). Since $H(s,s,s)=s$, comparison with the constant states proves

$$
m\leq U_j^n\leq M\quad\hbox{for all }j,n.
$$

The interval is invariant, so the same [Courant–Friedrichs–Lewy condition](../../../../../courant-friedrichs-lewy-condition.md) remains valid at every step. This is an $L^\infty$ bound relative to constant states, not a claim that arbitrary pairs of solutions are contractive in $L^\infty$.

For a stronger perturbation estimate, let $\mathcal T$ denote the global update and use componentwise maxima. Monotonicity gives $\mathcal T(U\vee V)\geq\mathcal TU,\mathcal TV$. Therefore

$$
(\mathcal TU-\mathcal TV)_+\leq\mathcal T(U\vee V)-\mathcal TV.
$$

Sum over the grid. The shared interface flux cancels telescopically, so conservation gives

$$
\sum_j(\mathcal TU_j-\mathcal TV_j)_+
\leq\sum_j(U_j-V_j)_+.
$$

Interchanging $U,V$ and adding yields the [L1 contraction of a monotone conservative scheme](../../../../../l1-contraction-of-a-monotone-conservative-scheme.md):

$$
\boxed{d\sum_j|U_j^n-V_j^n|\leq d\sum_j|U_j^0-V_j^0|.}
$$

This is a mesh-independent nonlinear [stability](../../../../../stability-of-a-numerical-method.md) estimate. On an infinite grid the telescoping argument is justified by summability of the differences and the bounded characteristic-speed range, or by truncation followed by a limit. For unequal prescribed boundary data, additional boundary flux terms enter the estimate.

The method is also a [total variation diminishing scheme](../../../../../total-variation-diminishing-scheme.md). Let $\mathcal S$ shift a grid sequence by one cell. Translation invariance gives $\mathcal T\mathcal S=\mathcal S\mathcal T$. Applying the preceding $L^1$ contraction to $U$ and $\mathcal SU$ shows

$$
\sum_j|U_{j+1}^{n+1}-U_j^{n+1}|
\leq\sum_j|U_{j+1}^{n}-U_j^{n}|.
$$

Hence initially finite discrete [total variation](../../../../../total-variation.md) cannot grow.

Finally, monotonicity supplies a [discrete entropy inequality](../../../../../discrete-entropy-inequality.md), explaining why the [stability](../../../../../stability-of-a-numerical-method.md) is compatible with the physically admissible [entropy solution](../../../../../entropy-solution.md). For a constant $c\in J$, define

$$
Q(a,b;c)=F(a\vee c,b\vee c)-F(a\wedge c,b\wedge c).
$$

Comparison of $H$ with the clipped triples above and below $c$ gives

$$
|U_j^{n+1}-c|\leq|U_j^n-c|
-\lambda\bigl(Q(U_j^n,U_{j+1}^n;c)-Q(U_{j-1}^n,U_j^n;c)\bigr).
$$

Indeed $H(U\vee c)\geq\max(H(U),c)$ and $H(U\wedge c)\leq\min(H(U),c)$, and subtracting these two update formulas yields exactly the right side. Also $Q(u,u;c)=\operatorname{sgn}(u-c)(f(u)-f(c))$, the [Kruzhkov entropy flux](../../../../../kruzhkov-entropy-flux.md). Under the displayed CFL condition the method therefore has an invariant state range, $L^1$ contraction, decreasing discrete [total variation](../../../../../total-variation.md) and entropy dissipation. These estimates remain meaningful at discontinuities, where linearized [Fourier analysis](../../../../../fourier-analysis-split.md) alone cannot establish the corresponding nonlinear [stability](../../../../../stability-of-a-numerical-method.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
