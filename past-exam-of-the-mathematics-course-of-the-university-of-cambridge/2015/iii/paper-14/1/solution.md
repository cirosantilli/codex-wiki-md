<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use probability [measure-preserving systems](../../../../../measure-preserving-system.md): $T:X\to X$ is measurable and $\mu(T^{-1}A)=\mu(A)$. Its [invariant sigma-algebra](../../../../../invariant-sigma-algebra.md) is

$$
\mathcal I=\{A\in\mathcal B:\mu(T^{-1}A\mathbin\triangle A)=0\}.
$$

**[Ergodicity](../../../../../ergodicity.md) means that every invariant measurable set has measure zero or one**:

$$
\boxed{A\in\mathcal I\ \Longrightarrow\ \mu(A)\in\{0,1\}.}
$$

Equivalently, every invariant measurable function is constant [almost everywhere](../../../../../almost-everywhere.md). Indeed all rational sublevel sets of a real invariant function belong to $\mathcal I$, so the zero-or-one alternative forces its distribution to concentrate at one value. Apply this to real and imaginary parts for complex functions. Conversely, an invariant set has an invariant indicator, so the function criterion implies the set criterion. This is the [invariant-function characterization of ergodicity](../../../../../invariant-function-characterization-of-ergodicity.md).

For an [irrational rotation of the circle](../../../../../irrational-rotation.md), $T(x)=x+\alpha\pmod1$ with $\alpha\notin\mathbb Q$, an invariant $g\in L^2(m)$ has [Fourier coefficients](../../../../../fourier-coefficient.md) satisfying

$$
(e^{2\pi i k\alpha}-1)\widehat g(k)=0.
$$

For $k\ne0$ the multiplier is nonzero. Completeness of the [Fourier series](../../../../../fourier-series-split.md) basis therefore makes $g$ constant. Apply this to an invariant indicator to prove **the irrational rotation is [ergodic](../../../../../ergodicity.md)**. A second example is the cyclic permutation of $q$ points with equal masses: a nonempty invariant set contains the whole cycle and hence has measure one.

The identity on $[0,1]$ with [Lebesgue measure](../../../../../lebesgue-measure.md) is not [ergodic](../../../../../ergodicity.md), since $[0,1/2]$ is invariant and has measure $1/2$. Nor is rotation by $1/5$ on the circle: the set

$$
A=\{x\in\mathbb R/\mathbb Z:5x\pmod1\in[0,1/2)\}
$$

is invariant and has measure $1/2$. These examples also show why preservation of measure does not imply [ergodicity](../../../../../ergodicity.md).

Let $U=U_T$ be the [Koopman operator](../../../../../koopman-operator.md), $Uf=f\circ T$, and set

$$
A_Nf=\frac1N\sum_{n=0}^{N-1}U^nf.
$$

The [Von Neumann mean ergodic theorem](../../../../../von-neumann-mean-ergodic-theorem.md) says that, for $f\in L^2(\mu)$, these [Cesaro averages](../../../../../cesaro-mean.md) converge in $L^2$ to the [orthogonal projection](../../../../../orthogonal-projection.md) onto the invariant functions:

$$
\boxed{A_Nf\longrightarrow P_{\operatorname{Fix}U}f
=\mathbb E_\mu[f\mid\mathcal I]\quad\text{in }L^2.}
$$

For an invertible system, $U$ is a [unitary operator](../../../../../unitary-operator.md). The Hilbert-space theorem states more generally that the [Cesaro averages](../../../../../cesaro-mean.md) of any [unitary operator](../../../../../unitary-operator.md) converge strongly to its fixed-space projection.

Here is the requested invertible-case proof. Since $U^*=U^{-1}$,

$$
\bigl(\operatorname{Ran}(I-U)\bigr)^\perp
=\ker(I-U^*)=\ker(I-U).
$$

Thus the [orthogonal decomposition for unitary ergodic averages](../../../../../orthogonal-decomposition-for-unitary-ergodic-averages.md) is

$$
L^2(\mu)=\operatorname{Fix}U\oplus
\overline{\operatorname{Ran}(I-U)}.
$$

On the first summand, $A_Nf=f$. On a vector $(I-U)g$, telescoping gives

$$
A_N(I-U)g=\frac{g-U^Ng}{N},
\qquad
\|A_N(I-U)g\|_2\leq\frac{2\|g\|_2}{N}\longrightarrow0.
$$

Because $\|A_N\|\leq1$, approximation extends this convergence to the closure of the range. The [orthogonal decomposition](../../../../../orthogonal-decomposition-by-a-closed-subspace.md) now proves the theorem for every $f$. An invariant $L^2$ function is $\mathcal I$-measurable, and an $\mathcal I$-measurable function is invariant by approximation with indicators; hence the projection is the stated [conditional expectation](../../../../../conditional-expectation.md).

In an [ergodic system](../../../../../ergodicity.md), invariant functions are constants by the criterion already proved. Their [orthogonal projection](../../../../../orthogonal-projection.md) is obtained by taking the inner product with $1$, whose norm is one. Therefore **the [ergodic](../../../../../ergodicity.md) limit is the space average**:

$$
\boxed{A_Nf\longrightarrow\left(\int_Xf\,d\mu\right)1
\quad\text{in }L^2.}
$$

The [Birkhoff ergodic theorem](../../../../../birkhoff-ergodic-theorem.md) states that, for $f\in L^1(\mu)$,

$$
\boxed{\frac1N\sum_{n=0}^{N-1}f(T^nx)
\longrightarrow\mathbb E_\mu[f\mid\mathcal I](x)
\quad\text{for }\mu\text{-almost every }x.}
$$

The limit is invariant, integrable, and has the same integral as $f$. On a probability space convergence also holds in $L^1$. In an [ergodic system](../../../../../ergodicity.md) the limit is $\int f\,d\mu$ [almost everywhere](../../../../../almost-everywhere.md).

For the topological sharpening, take a continuous map $T$ on a compact [metric space](../../../../../metric-space.md). **[Unique ergodicity](../../../../../unique-ergodicity.md) means there is exactly one invariant [Borel probability measure](../../../../../borel-probability-measure.md) $\mu$**. The [uniform ergodic convergence for uniquely ergodic systems](../../../../../uniform-ergodic-convergence-for-uniquely-ergodic-systems.md) says that every continuous real or complex $f$ satisfies

$$
\boxed{\sup_{x\in X}\left|
\frac1N\sum_{n=0}^{N-1}f(T^nx)-\int_Xf\,d\mu
\right|\longrightarrow0.}
$$

Thus convergence holds at every point and uniformly in that point. The continuity, compactness and continuous-observable hypotheses belong to this theorem; it is not a claim of uniform convergence for all measurable $L^1$ functions.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
