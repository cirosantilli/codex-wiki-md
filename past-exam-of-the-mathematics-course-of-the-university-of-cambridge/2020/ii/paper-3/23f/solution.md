<h1 id="23f/solution">Solution</h1>

↑ **Parent:** [23F](../23f.md)

For the [period lattice](../../../../../period-lattice.md) $\Lambda=\langle\lambda,\mu\rangle$, define the [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) by

$$
\wp(z)=\frac1{z^2}
+\sum_{\omega\in\Lambda\setminus\{0\}}
\left(\frac1{(z-\omega)^2}-\frac1{\omega^2}\right).
$$

To prove [Normal convergence of the Weierstrass elliptic-function series](../../../../../normal-convergence-of-the-weierstrass-elliptic-function-series.md), let $K\subset\mathbb C\setminus\Lambda$ be compact and choose $R$ with $|z|\leq R$ on $K$. For $|\omega|>2R$,

$$
\left|\frac1{(z-\omega)^2}-\frac1{\omega^2}\right|
=\left|\frac{2\omega z-z^2}{\omega^2(z-\omega)^2}\right|
\leq\frac{C_K}{|\omega|^3}.
$$

The comparison series $\sum_{\omega\ne0}|\omega|^{-3}$ converges by the stated lattice-sum criterion. The [Weierstrass M-test](../../../../../weierstrass-m-test.md) gives uniform convergence on $K$; since $K$ was arbitrary, the series converges locally uniformly away from $\Lambda$. The [locally uniform convergence of holomorphic functions](../../../../../locally-uniform-convergence-of-holomorphic-functions.md) makes its sum holomorphic there, and the displayed principal term gives a double pole at every lattice point.

The function $\wp$ is even and satisfies

$$
\wp(z)=\wp(w)
\quad\Longleftrightarrow\quad
z\equiv\pm w\pmod\Lambda.
$$

The three nonzero [two-torsion points](../../../../../two-torsion-point-of-a-complex-torus.md) $z_1,z_2,z_3$ are distinct modulo $\Lambda$ and each equals its own negative modulo $\Lambda$. Therefore no two can have the same $\wp$-value, so $e_1,e_2,e_3$ are distinct. Equivalently, $\wp$ is a degree-two branched map and each half-lattice point already occupies its fiber with multiplicity two.

For a transitive example, take the [equianharmonic lattice](../../../../../equianharmonic-lattice.md)

$$
\Lambda=\mathbb Z+\mathbb Z\omega,
\qquad \omega=e^{2\pi i/3},
$$

and define $\theta([z])=[\omega z]$. Multiplication by $\omega$ preserves $\Lambda$, so $\theta:\mathbb C/\Lambda\to\mathbb C/\Lambda$ is a [conformal equivalence](../../../../../conformal-equivalence.md). On the nonzero half-lattice points it acts by

$$
\left[\frac12\right]
\longmapsto\left[\frac\omega2\right]
\longmapsto\left[\frac{1+\omega}{2}\right]
\longmapsto\left[\frac12\right],
$$

because $\omega^2=-1-\omega$. Thus it acts transitively.

## ↑ Ancestors (10)

1. [23F](../23f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
