<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The curvature of $D=d+A$ is

$$
\boxed{F=D^2=dA+A\wedge A},
$$

or $F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu]$. The covariant exterior derivative and the [Jacobi identity](../../../../../jacobi-identity.md) give the [Bianchi identity](../../../../../bianchi-identity.md)

$$
\boxed{D_AF=dF+A\wedge F-F\wedge A=0},
\qquad D_{[\mu}F_{\nu\rho]}=0.
$$

Since the [Hodge star operator](../../../../../hodge-star-operator.md) satisfies $*^2=1$ on Euclidean two-forms,

$$
0\leq\int_{\mathbb R^4}-\operatorname{Tr}[(F\mp*F)\wedge*(F\mp*F)]
=S_E\mp16\pi^2k.
$$

Using the opposite choice of sign as well gives

$$
\boxed{S_E\geq16\pi^2|k|}.
$$

Equality holds precisely for a self-dual or anti-self-dual [Yang-Mills instanton](../../../../../yang-mills-instanton.md), with the sign selected by that of $k$.

Now assume $\partial_0A_\mu=0$ and write $\Phi=A_0$. Then

$$
F_{0i}=-D_i\Phi,
\qquad
B_i=\frac12\epsilon_{ijk}F_{jk}.
$$

The spatial Bianchi identity and the self-duality equations become

$$
\boxed{D_iB_i=0,
\qquad B_i=\mp D_i\Phi},
$$

where the upper four-dimensional sign gives the first displayed reduced sign under the orientation used here. Consequently

$$
\boxed{\sum_{i=1}^3D_i^2\Phi=0}.
$$

Gauge invariance of the inner product gives

$$
\Delta|\Phi|^2
=2\sum_i|D_i\Phi|^2
+2\left\langle\Phi,\sum_iD_i^2\Phi\right\rangle
=2\sum_i|D_i\Phi|^2.
$$

For $w=1-|\Phi|^2$,

$$
\boxed{\Delta w=-2\sum_i|D_i\Phi|^2\leq0}.
$$

Since $w\to0$ at infinity, the [weak maximum principle for elliptic operators](../../../../../weak-maximum-principle-for-elliptic-operators.md) excludes a negative interior minimum. Hence

$$
\boxed{|\Phi|\leq1\quad\text{everywhere}}.
$$

With $d^4x=dx^0d^3x$, direct decomposition gives

$$
\boxed{-2\operatorname{Tr}(F\wedge*F)
=(|D\Phi|^2+|B|^2)d^4x},
$$



$$
\boxed{\operatorname{Tr}(F\wedge F)
=\langle D_i\Phi,B_i\rangle d^4x}.
$$

Because $D_iB_i=0$,

$$
\langle D_i\Phi,B_i\rangle
=\partial_i\langle\Phi,B_i\rangle,
$$

so the Pontryagin density reduces to the surface charge $4\pi N$ per unit $x^0$. The conventional three-dimensional energy

$$
E_3=\frac12\int_{\mathbb R^3}(|D\Phi|^2+|B|^2)d^3x
$$

obeys the [Bogomolny bound](../../../../../bogomolny-bound.md) $E_3\geq4\pi|N|$, saturated by the [Bogomolny-Prasad-Sommerfield monopole](../../../../../bogomolny-prasad-sommerfield-monopole.md) equation. The four-dimensional action density per unit $x^0$ is $2E_3$; signs relating $k$ and $N$ depend on the self-duality and orientation convention.

For the [hedgehog ansatz for a monopole](../../../../../hedgehog-ansatz-for-a-monopole.md) in the question, direct differentiation with $[T_a,T_b]=-\epsilon_{abc}T_c$ gives

$$
\boxed{B_i^a=(2\alpha+r\alpha')\delta_{ia}
-\left(\frac{\alpha'}r+\alpha^2\right)x_ix_a}.
$$

On a sphere of radius $r$,

$$
B_i^an_i=(2\alpha-r^2\alpha^2)n_a,
\qquad
\Phi^a=f(r)n_a.
$$

Therefore

$$
N=\lim_{r\to\infty}\frac1{4\pi}
\int_{S_r^2}f(r)(2\alpha-r^2\alpha^2)dS.
$$

The boundary conditions $f\to1$ and $r^2\alpha\to1$ make the integrand equal to $r^{-2}+o(r^{-2})$. Thus

$$
\boxed{N=1}.
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 313](../../paper-313-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
