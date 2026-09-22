<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $h=|\Phi|^2$, $D_i=\partial_i-iA_i$, $j_i=\operatorname{Im}(\bar\Phi D_i\Phi)$, and $W(h)=h(1-h)^2/4$. Because the [inverse-density Abelian Higgs model](../../../../../inverse-density-abelian-higgs-model.md) contains $B^2/h$, its finite-energy admissible class matters at zeros of the [Higgs field](../../../../../higgs-field.md). First derive the formal equations on the open set where $h>0$; on the first-order solutions below the potentially singular quotients extend across the zeros.

For variations $\psi=\delta\Phi$ and $a_i=\delta A_i$,

$$
\delta h=2\operatorname{Re}(\bar\Phi\psi),\qquad
\delta B=\partial_1a_2-\partial_2a_1,\qquad
\delta(D_i\Phi)=D_i\psi-ia_i\Phi.
$$

Covariant integration by parts in the scalar term, and ordinary integration by parts in the magnetic term, give

$$
\delta V=\int\operatorname{Re}\left[
\overline{\left(-D_iD_i\Phi-\frac{B^2}{h^2}\Phi+W'(h)\Phi\right)}
\,\psi\right]d^2x
+\int\left[\epsilon_{ij}\partial_j(B/h)-j_i\right]a_i\,d^2x,
$$

where $\epsilon_{12}=1$. Here

$$
W'(h)=\frac14(1-h)(1-3h).
$$

Thus the [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md) are

$$
\boxed{D_iD_i\Phi+
\left[\frac{B^2}{h^2}-\frac14(1-h)(1-3h)\right]\Phi=0,}
$$



$$
\boxed{\partial_2(B/h)=j_1,\qquad-\partial_1(B/h)=j_2.}
$$

Equivalently the gauge equation is $\partial_j(F_{ji}/h)+j_i=0$. The current sign follows from the explicit choice $D=\partial-iA$.

For the [Bogomolny bound for the inverse-density Abelian Higgs model](../../../../../bogomolny-bound-for-the-inverse-density-abelian-higgs-model.md), compute

$$
\partial_1j_2-\partial_2j_1
=2\operatorname{Im}(\overline{D_1\Phi}D_2\Phi)-Bh,
$$

using $[D_1,D_2]\Phi=-iB\Phi$. Expanding the first square gives

$$
|(D_1+iD_2)\Phi|^2
=|D\Phi|^2-2\operatorname{Im}(\overline{D_1\Phi}D_2\Phi),
$$

so

$$
|D\Phi|^2=|(D_1+iD_2)\Phi|^2+Bh+
\partial_1j_2-\partial_2j_1.
$$

Also,

$$
\frac{B^2}{h}+\frac h4(1-h)^2
=\frac{[B-\tfrac12h(1-h)]^2}{h}+B(1-h).
$$

The current boundary integral vanishes by the assumed rapid decay. Combining the identities therefore gives

$$
\boxed{V=\frac12\int_{\mathbb R^2}
\left[|(D_1+iD_2)\Phi|^2+
\frac{[B-\tfrac12h(1-h)]^2}{h}\right]d^2x+\pi N.}
$$

For fixed positive flux the minimum is $\boxed{V_{\min}=\pi N}$, attained when the [Bogomolny equations](../../../../../bogomolny-equations.md) are

$$
\boxed{(D_1+iD_2)\Phi=0,\qquad B=\frac12h(1-h).}
$$

The quotient at a zero is understood through the finite-energy limit, not by dividing a literal nonzero numerator by zero.

These equations imply the second-order equations directly. Applying $D_1-iD_2$ to the first gives $(D_iD_i+B)\Phi=0$. On the second equation,

$$
-\frac{B^2}{h^2}+W'(h)
=-\frac14(1-h)^2+\frac14(1-h)(1-3h)
=-\frac12h(1-h)=-B,
$$

which is exactly the scalar equation. The first equation also implies $j_1=-\tfrac12\partial_2h$ and $j_2=\tfrac12\partial_1h$. Since $B/h=(1-h)/2$, the gauge equations follow too. All these coefficients are regular across zeros for smooth first-order fields.

For the scalar reduction, write $\Phi=e^{u/2+i\chi}$ away from its zeros. Separating the real and imaginary parts of the first [Bogomolny equation](../../../../../bogomolny-equations.md) gives

$$
A_1=\partial_1\chi+\frac12\partial_2u,\qquad
A_2=\partial_2\chi-\frac12\partial_1u.
$$

Thus, with the oriented planar [Hodge star](../../../../../hodge-star-operator.md) $*dx^1=dx^2$, $*dx^2=-dx^1$,

$$
A=d\chi-\frac12*du,\qquad B=-\frac12\Delta u
$$

away from the zeros. A zero $p_j$ of multiplicity $n_j$ has $u=2n_j\log|x-p_j|+\text{smooth}$ and phase winding $2\pi n_j$. The multiplicities are positive: locally the first-order equation is a covariant Cauchy–Riemann equation, and a nonvanishing integrating factor turns its solutions into holomorphic functions. Distributionally,

$$
B=2\pi\sum_jn_j\delta_{p_j}-\frac12\Delta u.
$$

Consequently the [logarithmic equation for inverse-density Abelian Higgs vortices](../../../../../logarithmic-equation-for-inverse-density-abelian-higgs-vortices.md) is

$$
\boxed{\Delta u+e^u(1-e^u)=4\pi\sum_jn_j\delta_{p_j},
\qquad u(x)\to0\text{ as }|x|\to\infty,\quad\sum_jn_j=N.}
$$

The delta terms are essential for multi-vortex reconstruction; omitting them would lose the specified zeros and flux.

Here is an explicit regular reconstruction, which also removes all artificial singularities. Given distinct locations $p_j$ and integer multiplicities, put

$$
u_0(x)=\sum_jn_j\log\frac{|x-p_j|^2}{1+|x-p_j|^2},
\qquad
g(x)=4\sum_j\frac{n_j}{(1+|x-p_j|^2)^2}.
$$

Since $\Delta u_0=4\pi\sum_jn_j\delta_{p_j}-g$, solving the smooth nonlinear elliptic problem for $v=u-u_0$ amounts to

$$
\boxed{\Delta v=g-e^{u_0+v}(1-e^{u_0+v}),\qquad v\to0.}
$$

Let $z=x^1+ix^2$ and let $z_j$ represent $p_j$. A smooth solution with the topological decay reconstructs

$$
\boxed{\Phi(z)=e^{v(z)/2}\prod_j
\left(\frac{z-z_j}{\sqrt{1+|z-z_j|^2}}\right)^{n_j},}
$$



$$
\boxed{A=\frac12\sum_jn_j*d\log(1+|x-p_j|^2)-\frac12*dv.}
$$

These formulas are smooth at every prescribed zero and agree with the phase formula off the zeros. Taking a curl and using the equation for $v$ verifies $B=e^u(1-e^u)/2$; substitution verifies the other first-order equation. At infinity the phase winds $N$ times, producing flux $2\pi N$. Thus multi-vortex construction reduces to solving one scalar elliptic boundary-value problem for specified positions and multiplicities, followed by these explicit formulas.

For the topological branch, $u\le0$: a positive interior maximum would have $\Delta u\le0$, whereas the equation there gives $\Delta u=e^u(e^u-1)>0$. At infinity, the linearized scalar equation is $\Delta u-u=0$. Comparison barriers and elliptic estimates give the decaying tail for regular topological solutions, and hence the required decay of $B,D\Phi$ and $1-h$. The nonlinear elliptic problem determines $v$; the reconstruction formulas do not constitute an arbitrary superposition of single-vortex profiles.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
