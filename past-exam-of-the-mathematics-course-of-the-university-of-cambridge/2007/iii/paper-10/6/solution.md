<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

On the [torus](../../../../../torus.md) $\mathbb T^n=(\mathbb R/2\pi\mathbb Z)^n$, choose normalized [Haar measure](../../../../../haar-measure.md), so that $e_k(x)=e^{ik\cdot x}$, $k\in\mathbb Z^n$, is an [orthonormal basis](../../../../../orthonormal-basis.md) of $L^2$. A [periodic Sobolev space](../../../../../periodic-sobolev-space.md) is defined, for any real $s$, by

$$
H^s(\mathbb T^n)=\left\{u:\sum_{k\in\mathbb Z^n}(1+|k|^2)^s|\widehat u(k)|^2<\infty\right\},\qquad
\|u\|_{H^s}^2=\sum_k(1+|k|^2)^s|\widehat u(k)|^2.
$$

For negative $s$, the coefficients describe [distributions](../../../../../distribution-mathematical-analysis.md) rather than necessarily functions. For a nonnegative integer $s$, the weight is comparable to $\sum_{|\alpha|\leq s}|k^\alpha|^2$, so this [norm](../../../../../norm.md) is equivalent to the sum of the squared $L^2$ [norms](../../../../../norm.md) of all [weak derivatives](../../../../../weak-derivative.md) through order $s$. Fourier truncation proves that smooth [trigonometric polynomials](../../../../../trigonometric-polynomial.md) are dense. The $L^2$ pairing identifies the continuous dual of $H^s$ with $H^{-s}$, giving [Sobolev duality](../../../../../sobolev-duality.md).

Two Fourier estimates explain the usefulness of these spaces. If $s>m+n/2$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
\sum_k |k|^m|\widehat u(k)|
\leq\|u\|_{H^s}\left(\sum_k\frac{|k|^{2m}}{(1+|k|^2)^s}\right)^{1/2}<\infty.
$$

[Uniform convergence](../../../../../uniform-convergence.md) of the differentiated [Fourier series](../../../../../fourier-series-split.md) proves the [Sobolev embedding](../../../../../failure-of-first-order-sobolev-embedding-into-linfinity-in-two-dimensions.md) $H^s\hookrightarrow C^m$. If $\delta>0$, a bounded subset of $H^{s+\delta}$ has uniformly small high-frequency tails in $H^s$:

$$
\sum_{|k|>R}(1+|k|^2)^s|\widehat u(k)|^2
\leq(1+R^2)^{-\delta}\|u\|_{H^{s+\delta}}^2.
$$

Finite-dimensional Fourier truncation therefore proves the compact embedding $H^{s+\delta}\hookrightarrow H^s$, the periodic version of [Rellich-Kondrachov compactness theorem](../../../../../rellich-kondrachov-theorem.md). In addition, for $s>n/2$ multiplication is continuous $H^s\times H^s\to H^s$, making it a [Sobolev algebra](../../../../../sobolev-algebra.md). Indeed the weighted coefficient of a product is bounded by the sum of the convolutions of $\langle k\rangle^s|\widehat u(k)|$ with $|\widehat v(k)|$ and of $|\widehat u(k)|$ with $\langle k\rangle^s|\widehat v(k)|$; Cauchy-Schwarz puts unweighted coefficients in $\ell^1$, and the $\ell^1*\ell^2\to\ell^2$ case of [Young's convolution inequality](../../../../../young-s-convolution-inequality.md) finishes the estimate.

For [eigenfunction expansions](../../../../../eigenfunction-expansion.md), distinguish ellipticity from [self-adjointness](../../../../../self-adjoint-operator.md). An arbitrary non-self-adjoint elliptic operator need not have an [orthonormal basis](../../../../../orthonormal-basis.md) of [eigenfunctions](../../../../../eigenfunction.md). A useful definite setting is

$$
L u=-\sum_{i,j}\partial_i(a_{ij}(x)\partial_j u)+V(x)u,
$$

with smooth real periodic coefficients, $a_{ij}=a_{ji}$, real $V$, and [uniform ellipticity](../../../../../uniformly-elliptic-operator.md)

$$
\sum_{i,j}a_{ij}(x)\xi_i\xi_j\geq c|\xi|^2\qquad(c>0).
$$

Take the [self-adjoint](../../../../../self-adjoint-operator.md) realization in $L^2$ with domain $H^2$. Its construction and spectral properties can be seen from the associated form on $H^1$,

$$
b(u,v)=\int\left(\sum_{i,j}a_{ij}\partial_j u\,\overline{\partial_i v}+V u\overline v\right).
$$

For a sufficiently large constant $C$, $b_C=b+C(\cdot,\cdot)$ is a positive [coercive](../../../../../coercive-bilinear-form.md) form: $b_C(u,u)\geq c_1\|u\|_{H^1}^2$, and $L+C\geq I$. The [Lax-Milgram theorem](../../../../../lax-milgram-theorem.md) supplies the unique weak solution of $(L+C)u=f$ for $f\in H^{-1}$; the form is Hermitian, which gives symmetry of its inverse on $L^2$.

The regularity input is the [periodic elliptic estimate](../../../../../periodic-elliptic-estimate.md)

$$
\|u\|_{H^{s+2}}\leq C_s\bigl(\|Lu\|_{H^s}+\|u\|_{H^s}\bigr).
$$

Here is why an elliptic operator gains two [derivatives](../../../../../derivative.md). With coefficients frozen at a point, its principal symbol $\sum a_{ij}\xi_i\xi_j$ dominates $c|\xi|^2$, and the estimate follows by multiplying [Fourier coefficients](../../../../../fourier-coefficient.md) by that symbol. On a sufficiently small coordinate patch, the difference of the leading coefficients from these constants has arbitrarily small supremum [norm](../../../../../norm.md). In the integer-order differentiated estimate, this absorbs the highest [derivatives](../../../../../derivative.md) into the left side; [derivatives](../../../../../derivative.md) falling on coefficients contribute only lower-order terms. A [partition of unity](../../../../../partition-of-unity.md) reduces the variable-coefficient problem to such patches. Its [commutators](../../../../../commutator.md) with $L$ have order one, controlled by

$$
\|u\|_{H^{s+1}}\leq\varepsilon\|u\|_{H^{s+2}}+C_\varepsilon\|u\|_{H^s},
$$

which follows by splitting low and high [Fourier modes](../../../../../fourier-mode.md). Absorbing these terms gives the displayed estimate. For a weak $H^1$ solution, the same localization with difference quotients first bounds its second [weak derivatives](../../../../../weak-derivative.md) for $f\in L^2$; differentiating and repeating then gives $f\in H^s\Rightarrow u\in H^{s+2}$ for nonnegative integer $s$. Interpolation and duality extend the scale to real orders. In particular $(L+C)^{-1}:L^2\to H^2$ is bounded.

Let $R=(L+C)^{-1}$. [Compactness](../../../../../compact-space.md) of $H^2\hookrightarrow L^2$ makes $R$ a [compact operator](../../../../../compact-operator-split.md). Symmetry of the form makes $R$ [self-adjoint](../../../../../self-adjoint-operator.md), and positivity of $L+C$ makes $R$ positive and [injective](../../../../../injective-function.md). Its range is dense because $\ker R^*=\ker R=0$. The [spectral theorem for compact self-adjoint operators](../../../../../spectral-theorem-for-compact-hermitian-operators.md) consequently gives an [orthonormal basis](../../../../../orthonormal-basis.md) $\phi_j$ with

$$
R\phi_j=\mu_j\phi_j,\quad\mu_j>0,\quad\mu_j\longrightarrow0,\qquad
L\phi_j=\lambda_j\phi_j,\quad\lambda_j=\mu_j^{-1}-C\longrightarrow+\infty.
$$

[Elliptic regularity](../../../../../elliptic-regularity.md) bootstraps every $\phi_j$ to a [smooth function](../../../../../smooth-function.md). Each [eigenvalue](../../../../../eigenvalue.md) has finite multiplicity. Thus **a [self-adjoint](../../../../../self-adjoint-operator.md) uniformly elliptic second-order operator on the [torus](../../../../../torus.md) has a complete smooth [orthonormal](../../../../../orthonormal-set.md) [eigenfunction expansion](../../../../../eigenfunction-expansion.md) with discrete [eigenvalues](../../../../../eigenvalue.md) tending to infinity**.

Writing $u_j=(u,\phi_j)$, every $u\in L^2$ has $u=\sum_j u_j\phi_j$ in $L^2$, with $\|u\|_2^2=\sum_j|u_j|^2$. Iterating the elliptic estimate shows that the graph [norm](../../../../../norm.md) of $(L+C)^m$ is equivalent to the $H^{2m}$ [norm](../../../../../norm.md). Interpolation and duality give the more general spectral description

$$
\boxed{\|u\|_{H^s}^2\asymp\sum_j(\lambda_j+C)^s|u_j|^2.}
$$

The comparison constants depend on the operator and $s$. In particular [smooth function](../../../../../smooth-function.md)s have coefficients decaying faster than every power of $\lambda_j+C$, and their expansions converge in every [Sobolev norm](../../../../../sobolev-norm.md) and hence in every $C^m$ [norm](../../../../../norm.md).

This gives a practical way to solve elliptic equations. The equation $Lu=f$ is solvable if and only if $f_j=0$ whenever $\lambda_j=0$; then one may take $u_j=f_j/\lambda_j$ on the other [eigenspaces](../../../../../eigenspace.md) and add an arbitrary [vector](../../../../../vector.md) in $\ker L$. The Sobolev description proves the two-derivative gain and the [Fredholm alternative](../../../../../fredholm-alternative.md), rather than leaving them as formal [series](../../../../../series-mathematics.md) manipulations. Similarly the solution of the [heat equation](../../../../../heat-equation.md) $\partial_tu+Lu=0$ is

$$
u(t)=\sum_j e^{-t\lambda_j}u_j(0)\phi_j.
$$

For every $t>0$ the exponential decay at high [eigenvalues](../../../../../eigenvalue.md) places this solution in every [Sobolev space](../../../../../sobolev-space-split.md), hence it is smooth.

For the [Laplacian](../../../../../laplacian.md) $-\Delta$ the [eigenfunctions](../../../../../eigenfunction.md) are precisely $e^{ik\cdot x}$ with [eigenvalues](../../../../../eigenvalue.md) $|k|^2$. The number with $|k|^2\leq R$ is the number of lattice points in a radius-$\sqrt R$ ball, asymptotic to its volume by comparison with unit cubes. For the general [self-adjoint](../../../../../self-adjoint-operator.md) operator above, bounds on its form above and below by positive multiples of $\|\nabla u\|_2^2$ plus constants, together with the [Courant–Fischer min-max principle](../../../../../courant-fischer-min-max-principle.md), imply $\lambda_j+C\asymp j^{2/n}$. Thus the growth reflects [dimension](../../../../../dimension-vector-space.md) and the two-derivative order. [Compactness](../../../../../compact-space.md) of the [torus](../../../../../torus.md) is essential: on $\mathbb R^n$, translated bumps prevent the compact embedding, and the [Laplacian](../../../../../laplacian.md) instead has continuous [spectrum](../../../../../spectrum-functional-analysis.md) described by the [Fourier transform](../../../../../fourier-transform.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
