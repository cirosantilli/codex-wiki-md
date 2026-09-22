<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use [Minkowski spacetime](../../../../../minkowski-spacetime.md) with signature $(+,-,\ldots,-)$ and $\hbar=1$, with a vacuum time-ordering prescription. At a regulator, define the normalized [generating functional](../../../../../generating-functional.md)

$$
Z[J]=\frac{\int\mathcal D\phi\;e^{i(S[\phi]+\int J\phi)}}{\int\mathcal D\phi\;e^{iS[\phi]}},\qquad Z[0]=1.
$$

The normalized vacuum [correlation functions](../../../../../correlation-function.md) of a [time-ordered product](../../../../../time-ordered-product.md) are

$$
G_n(x_1,\ldots,x_n)=\left.\frac1{i^n}\frac{\delta^n Z}{\delta J(x_1)\cdots\delta J(x_n)}\right|_{J=0}.
$$

The [connected generating functional](../../../../../connected-generating-functional.md) is

$$
\boxed{W[J]=-i\log Z[J],\qquad
C_n=\left.i^{1-n}\frac{\delta^n W}{\delta J(x_1)\cdots\delta J(x_n)}\right|_{J=0}.}
$$

The logarithm selects connected source diagrams, or equivalently [cumulants](../../../../../cumulant.md). With the assumed vanishing [one-point function](../../../../../one-point-correlation-function.md), [derivatives](../../../../../derivative.md) of $Z=e^{iW}$ give the [centered four-point cumulant decomposition](../../../../../centered-four-point-cumulant-decomposition.md):

$$
\boxed{G_{1234}=C_{1234}+C_{12}C_{34}+C_{13}C_{24}+C_{14}C_{23}.}
$$

In detail, four differentiations either act on one connected block or form one of three pair partitions. Contributions with blocks of size one vanish. If $W_{ij}$ and $W_{1234}$ denote source [derivatives](../../../../../derivative.md) at zero, the same relation is $G_{1234}=iW_{1234}-W_{12}W_{34}-W_{13}W_{24}-W_{14}W_{23}$, since $C_2=-iW_2$ and $C_4=iW_4$.

Let $\varphi(x)=\delta W/\delta J(x)$ be the source-dependent mean field. On a locally invertible source-to-field branch, define the [quantum effective action](../../../../../effective-action.md) by the Minkowski [Legendre transform](../../../../../convex-conjugate.md)

$$
\boxed{\Gamma[\varphi]=W[J]-\int d^dx\,J(x)\varphi(x).}
$$

Its variation is $\delta\Gamma=-\int J\delta\varphi$, so $\delta\Gamma/\delta\varphi=-J$. Differentiating the two inverse source-field maps yields the [Minkowski inverse-Hessian relation for an effective action](../../../../../minkowski-inverse-hessian-relation-for-an-effective-action.md):

$$
\boxed{\int d^dz\,\frac{\delta^2\Gamma}{\delta\varphi(x)\delta\varphi(z)}
\frac{\delta^2W}{\delta J(z)\delta J(y)}=-\delta^{(d)}(x-y).}
$$

Thus $\Gamma^{(2)}=-(W^{(2)})^{-1}$. The inverse is understood at the regulator and on a nonsingular fluctuation sector; it is not an assertion that every source-field map is globally invertible.

For a free [real scalar field](../../../../../real-scalar-field.md), integrate by parts to write

$$
S[\phi]=\frac12\phi A\phi,\qquad A=-\Box-m^2,
\qquad A_\epsilon=A+i\epsilon,
$$

where repeated spacetime variables are integrated. Specify the [propagator](../../../../../propagator.md) convention explicitly:

$$
\Delta_F(x-y)=\int\frac{d^dp}{(2\pi)^d}\frac{i\,e^{-ip(x-y)}}{p^2-m^2+i0},\qquad \Delta_F=iA_\epsilon^{-1}.
$$

Completing the [Gaussian path integral](../../../../../gaussian-path-integral.md) around $\phi=-A_\epsilon^{-1}J$ cancels the source-independent [determinant](../../../../../determinant.md) between numerator and denominator. Therefore

$$
Z[J]=\exp\left[-\frac i2JA_\epsilon^{-1}J\right],\qquad
\boxed{W[J]=-\frac12JA_\epsilon^{-1}J=\frac i2J\Delta_FJ.}
$$

The positive imaginary term in $A_\epsilon$ damps the oscillatory Gaussian. Together with vacuum projection at the time boundaries, it selects the Feynman poles and the time-ordered, in-out [correlation function](../../../../../correlation-function.md) rather than a retarded inverse. It can also be obtained by continuation from the Euclidean vacuum integral. A denominator convention without the numerator $i$ redistributes the displayed factors of $i$.

Finally $\varphi=-A_\epsilon^{-1}J$, hence $J=-A_\epsilon\varphi$. Substitution into the [Legendre transform](../../../../../convex-conjugate.md) gives the [vacuum-normalized effective action of a free scalar field](../../../../../vacuum-normalized-effective-action-of-a-free-scalar-field.md):

$$
\boxed{\Gamma[\varphi]=\frac12\varphi A_\epsilon\varphi\longrightarrow S[\varphi]\quad(\epsilon\downarrow0).}
$$

All connected functions beyond order two vanish and all proper vertices beyond the classical quadratic kernel vanish. Vacuum normalization fixes the additive constant; without it, the [quantum effective action](../../../../../effective-action.md) equals the classical action up to a field-independent [determinant](../../../../../determinant.md) contribution.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
