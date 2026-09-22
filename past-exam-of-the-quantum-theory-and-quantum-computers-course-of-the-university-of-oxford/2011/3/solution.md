<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [Dirac notation](../../../bra-ket-notation.md) convention that the [inner product](../../../inner-product-split.md) is linear in the ket. Orthonormality of the computational [basis](../../../basis.md) gives

$$
\langle k|f\rangle=\sum_{\ell\in\mathbb Z_N}f(\ell)\langle k|\ell\rangle=f(k).
$$

The finite geometric sum satisfies $\sum_{k=0}^{N-1}\lambda^{rk}=N$ if $r=0$ in $\mathbb Z_N$, and zero otherwise: in the second case it equals $(1-\lambda^{rN})/(1-\lambda^r)=0$. Therefore

$$
\langle\widehat m|\widehat n\rangle=\frac1N\sum_k\lambda^{(n-m)k}=\delta_{mn}.
$$

There are $N$ such orthonormal [vectors](../../../vector.md) in an $N$-dimensional space, so they form a [basis](../../../basis.md). The inverse expansion is verified by the same sum:

$$
\boxed{\frac1{\sqrt N}\sum_j\lambda^{-jk}|\widehat j\rangle
=\frac1N\sum_{j,\ell}\lambda^{j(\ell-k)}|\ell\rangle=|k\rangle.}
$$

This is the [unitary](../../../unitary-connection.md) [discrete Fourier transform](../../../discrete-fourier-transform-split.md) and its inverse.

For the [basis-copying isometry](../../../basis-copying-isometry.md), the images $|k\rangle|k\rangle$ are orthonormal, so $C$ is a linear [isometry](../../../isometry.md), with $C^*C=I$. Its [matrix](../../../matrix.md) elements give

$$
\langle Ck|\,|f\rangle|g\rangle
=\langle k|f\rangle\langle k|g\rangle=f(k)g(k)=\langle k|f.g\rangle.
$$

Applying the definition of the [adjoint operator](../../../adjoint-operator.md), the coefficient of $|k\rangle$ in $C^*|f\rangle|g\rangle$ is exactly this expression. Thus

$$
\boxed{C^*|f\rangle|g\rangle=|f.g\rangle.}
$$

Equivalently $C^*|k\rangle|\ell\rangle=\delta_{k\ell}|k\rangle$. The adjoint of [basis](../../../basis.md) copying acts as pointwise multiplication of coefficient [functions](../../../function-split.md).

For the [Fourier transform of a basis-copying isometry](../../../fourier-transform-of-a-basis-copying-isometry.md), the [normalization](../../../normalization.md) matters:

$$
f_m(k)f_n(k)=\frac{\lambda^{(m+n)k}}N=\frac1{\sqrt N}f_{m+n}(k).
$$

Hence $C^*|\widehat m\rangle|\widehat n\rangle=N^{-1/2}|\widehat{m+n}\rangle$. Taking adjoint [matrix](../../../matrix.md) elements, or expanding both output factors in the inverse Fourier [basis](../../../basis.md), yields

$$
\boxed{C|\widehat j\rangle=\frac1{\sqrt N}\sum_{m+n=j}|\widehat m\rangle|\widehat n\rangle.}
$$

**The printed formula is missing the factor $1/\sqrt N$.** There are $N$ mutually [orthogonal](../../../orthogonal-vectors.md) terms in its sum, so without that factor its right side has [norm](../../../norm.md) $\sqrt N$, whereas its left side has [norm](../../../norm.md) one because $C$ is an [isometry](../../../isometry.md). The formula above is the normalized identity consistent with all the preceding definitions. For $N=1$ the distinction disappears, but the no-cloning assertion is substantive for $N\geq2$.

The normalized output is not $|\widehat j\rangle|\widehat j\rangle$. Its coefficient [matrix](../../../matrix.md) pairs every Fourier label $m$ with $j-m$; tracing out either factor gives $I/N$. Thus it is a [maximally entangled state](../../../maximally-entangled-state.md), while two clones of a pure Fourier [quantum state](../../../quantum-state.md) would have pure reduced [quantum states](../../../quantum-state.md). A copier for the computational [basis](../../../basis.md) therefore does not copy the Fourier [basis](../../../basis.md).

More generally, suppose a linear [isometry](../../../isometry.md) with a fixed blank input could clone every normalized [quantum state](../../../quantum-state.md). Its restriction to $|\psi\rangle|\mathrm{blank}\rangle$ would define a linear map $D$ with $D|k\rangle=|k\rangle|k\rangle$ on every computational [basis](../../../basis.md) [quantum state](../../../quantum-state.md). Linearity forces $D=C$, which has just been shown to fail on Fourier [quantum states](../../../quantum-state.md). This proves the [no-cloning theorem](../../../no-cloning-theorem.md) in the pure-[quantum state](../../../quantum-state.md) isometric setting.

The inner-product proof makes the obstruction independent of the chosen [basis](../../../basis.md). If an [isometry](../../../isometry.md) cloned two [quantum states](../../../quantum-state.md) with overlap $s=\langle\psi|\phi\rangle$, preservation of inner products would give $s=s^2$, or, allowing irrelevant output phases, $|s|=|s|^2$. Distinct nonorthogonal rays have $0<|s|<1$, which is impossible. Even allowing an output environment does not help: [unitary](../../../unitary-connection.md) evolution would give $|s|=|s|^2|\langle e_\psi|e_\phi\rangle|\leq|s|^2$, the same contradiction. **Arbitrary unknown [quantum states](../../../quantum-state.md) cannot be cloned**, although any fixed [orthonormal basis](../../../orthonormal-basis.md) can be copied and a one-dimensional [quantum state](../../../quantum-state.md) space is trivial.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2011](../../2011-split.md)
3. [Past exam of the quantum theory and quantum computers course of the University of Oxford](../../split.md)
4. [Quantum theory and quantum computers course of the University of Oxford](../../../quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
