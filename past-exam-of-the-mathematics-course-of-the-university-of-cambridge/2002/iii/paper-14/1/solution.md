<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [Lie group](../../../../../lie-group.md) is a group which is a finite-dimensional smooth Hausdorff second-countable manifold, with smooth multiplication and inversion. For the [special unitary group](../../../../../special-unitary-group.md), consider the real [vector space](../../../../../vector-space-split.md)

$$
\mathfrak{su}(n)=\{X\in M_n(\mathbb C):X^*=-X,\ \operatorname{tr}X=0\}.
$$

The diagonal entries of a skew-Hermitian [matrix](../../../../../matrix.md) supply $n$ real parameters, and the entries above the diagonal supply $2\binom n2$; the trace-zero condition removes one real parameter. Thus $\dim_{\mathbb R}\mathfrak{su}(n)=n^2-1$.

The [matrix](../../../../../matrix.md) facts used to construct charts are these: the [matrix exponential](../../../../../matrix-exponential.md) is analytic, its derivative at zero is the identity, and it has an analytic inverse [matrix logarithm](../../../../../matrix-logarithm.md) on a sufficiently small neighborhood of the identity. On those neighborhoods $\log(e^X)=X$, $e^{\log U}=U$, and $\det(e^X)=e^{\operatorname{tr}X}$. For a unitary [matrix](../../../../../matrix.md) in that neighborhood, the [spectral theorem](../../../../../spectral-theorem.md) writes $U=W\operatorname{diag}(e^{i\theta_j})W^*$ with principal angles close to zero, and $\log U=W\operatorname{diag}(i\theta_j)W^*$ is skew-Hermitian.

Choose a norm ball of radius $\varepsilon<\pi/n$ small enough to lie in the exponential's inverse domain. If $U$ is unitary, $\det U=1$ and $\|\log U\|<\varepsilon$ in operator norm, then

$$
\operatorname{tr}\log U\in2\pi i\mathbb Z,\qquad
|\operatorname{tr}\log U|\le n\|\log U\|<\pi,
$$

so its trace is zero. Conversely $X\in\mathfrak{su}(n)$ gives $(e^X)^*e^X=I$ and $\det(e^X)=1$. Thus the logarithm identifies an open neighborhood $V$ of $I$ in $SU(n)$, with its [matrix](../../../../../matrix.md) subspace topology, with the open ball $B_\varepsilon\subset\mathfrak{su}(n)$. Choosing a real linear identification $\mathfrak{su}(n)\cong\mathbb R^{n^2-1}$ turns this into a chart.

For every $A\in SU(n)$ take the translated chart

$$
\boxed{\phi_A:AV\longrightarrow B_\varepsilon,\qquad \phi_A(U)=\log(A^{-1}U)}.
$$

Their overlap maps are $X\mapsto\log(B^{-1}A e^X)$ wherever both charts are defined, so they are real analytic. They cover the group; the [matrix](../../../../../matrix.md) topology is Hausdorff and second-countable. This constructs the real manifold directly, rather than merely counting equations. [Matrix](../../../../../matrix.md) multiplication is polynomial in real/imaginary entries and inversion here is $U\mapsto U^*$; in the logarithm charts both are smooth. The [logarithm charts for the special unitary group](../../../../../logarithm-charts-for-the-special-unitary-group.md) therefore prove

$$
\boxed{SU(n)\text{ is a Lie group of real dimension }n^2-1}.
$$

For $n=1$ it is the one-point group of dimension zero.

For $n=2$, let the first column be $(a,b)$, of unit norm. Every unit vector orthogonal to it is a scalar of modulus one times $(-\bar b,\bar a)$. The [determinant](../../../../../determinant.md) of the resulting [matrix](../../../../../matrix.md) is that scalar, so [determinant](../../../../../determinant.md) one fixes it to $1$. Hence

$$
\boxed{\Phi:S^3\subset\mathbb C^2\longrightarrow SU(2),\qquad
(a,b)\longmapsto\begin{pmatrix}a&-\bar b\\b&\bar a\end{pmatrix}}
$$

is bijective, with inverse given by taking the first column. The forward map is real polynomial in the four coordinates; composing with the local logarithm charts verifies smoothness into the constructed manifold. The inverse is a smooth [matrix](../../../../../matrix.md)-coordinate projection and, in the usual embedded sphere charts, is smooth into $S^3$. Thus $\boxed{SU(2)\cong S^3\text{ by a diffeomorphism}}$, the explicit realization of [SU(2) as the three-sphere](../../../../../su-2-as-the-three-sphere.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
