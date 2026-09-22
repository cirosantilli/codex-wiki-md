<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $A_N=\begin{pmatrix}0&-1\\N&0\end{pmatrix}$. All calculations here use the [Hecke-normalized rational slash operator](../../../../../hecke-normalized-rational-slash-operator.md) of the PDF. Its [automorphy factor](../../../../../automorphy-factor.md) identity gives $(f[\alpha]_k)[\beta]_k=f[\alpha\beta]_k$. For $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma_1(N)$,

$$
A_N\gamma A_N^{-1}=\begin{pmatrix}d&-c/N\\-Nb&a\end{pmatrix}\in\Gamma_1(N).
$$

This proves that $A_N$ normalizes the [Gamma 1 congruence subgroup](../../../../../gamma-1-congruence-subgroup.md). Right-action associativity shows $f[A_N]_k$ has the same transformation law as $f$. It is holomorphic in the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md); at each [modular cusp](../../../../../cusp-of-a-modular-group.md), the rational change of variable preserves cusp decay by the upper-triangular factorization used in 2(i). Consequently $W_N$ maps the [cusp form](../../../../../cusp-form.md) space to itself.

For a scalar matrix $-NI$, the printed slash normalization gives

$$
f[-NI]_k=(-1)^kN^{k-2}f.
$$

Since $A_N^2=-NI$, the two phase and determinant factors cancel:

$$
\boxed{W_N^2f=i^{2k}N^{2-k}f[-NI]_k=f.}
$$

Explicitly, the [Fricke involution](../../../../../fricke-involution.md) in the question is

$$
W_Nf(\tau)=i^kN^{-k/2}\tau^{-k}f\left(-\frac1{N\tau}\right).
$$

Its phase is essential for the involution and the functional-equation sign.

Suppose $W_Nf=\varepsilon f$. Define $F(y)=f(iy/\sqrt N)$ for $y>0$. Substitution at $\tau=iy/\sqrt N$ gives

$$
\boxed{F(1/y)=\varepsilon y^kF(y).}
$$

At infinity $F$ decays exponentially because $f$ is a [cusp form](../../../../../cusp-form.md). This identity gives $F(y)=O(y^{-k}e^{-c/y})$ near zero for some $c>0$. Thus its [Mellin transform](../../../../../mellin-transform.md) converges for every complex $s$, locally uniformly with all $s$ derivatives.

Initially, in a right half-plane where the [Dirichlet series](../../../../../dirichlet-series.md) converges absolutely, termwise integration and the [gamma function](../../../../../gamma-function.md) integral give

$$
\int_0^\infty F(y)y^{s-1}dy
=N^{s/2}(2\pi)^{-s}\Gamma(s)\sum_{n\geq1}\frac{a_n}{n^s}
=\Lambda_N(f,s).
$$

Such a half-plane exists without any eigenform hypothesis. Indeed the invariant quantity $(\operatorname{Im}\tau)^{k/2}|f(\tau)|$ is bounded on the modular quotient, by cusp decay and compactness away from the cusps. Fourier coefficient extraction on the line $\operatorname{Im}\tau=1/n$ gives $a_n=O(n^{k/2})$, so $\operatorname{Re}s>1+k/2$ suffices for the interchange.

Split the integral at one and change $y$ to $1/y$ in its lower part. The [phase-normalized Fricke functional equation](../../../../../phase-normalized-fricke-functional-equation.md) becomes transparent:

$$
\boxed{\Lambda_N(f,s)=\int_1^\infty F(y)\left(y^{s-1}+\varepsilon y^{k-s-1}\right)dy.}
$$

The integral defines an [entire function](../../../../../entire-function.md): exponential decay dominates every power and every logarithmic derivative uniformly on compact $s$ sets. Replacing $s$ by $k-s$ and using $\varepsilon^2=1$ now proves

$$
\boxed{\Lambda_N(f,k-s)=\varepsilon\Lambda_N(f,s).}
$$

This gives the full analytic continuation of the completed [L-function of a cusp form](../../../../../l-function-of-a-cusp-form.md), not merely a formal identity in its initial convergence region.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 88](../../paper-88-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
