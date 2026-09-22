<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $B(x)=\bar\psi(x)\psi(x)$, a Grassmann-even [Dirac scalar bilinear](../../../../dirac-scalar-bilinear.md). Completing the square gives

$$
-\frac12\sigma^2+g\sigma B
=-\frac12(\sigma-gB)^2+\frac{g^2}{2}B^2.
$$

Introduce external Grassmann [sources](../../../../source-quantum-field-theory.md) $\eta,\bar\eta$ for the [Dirac field](../../../../dirac-field.md), but no source for $\sigma$. The [generating functional](../../../../generating-functional.md) is

$$
Z[\eta,\bar\eta]=\int\mathcal D\bar\psi\,\mathcal D\psi\,\mathcal D\sigma\,
\exp\left\{i\int d^4x\left[\bar\psi(i\not\partial-m)\psi
-\frac12(\sigma-gB)^2+\frac{g^2}{2}B^2
+\bar\eta\psi+\bar\psi\eta\right]\right\}.
$$

At a finite regulator the change of variable $\sigma'=\sigma-gB$ has unit Jacobian: it translates a bosonic integration variable by a Grassmann-even expression independent of that variable. Its oscillatory [Gaussian integral](../../../../gaussian-integral.md) can be defined with a convergence prescription and then continued. It is a constant $\mathcal N$ independent of $\psi,\eta,\bar\eta$. Thus

$$
Z[\eta,\bar\eta]=\mathcal N\int\mathcal D\bar\psi\,\mathcal D\psi\,
\exp\left\{i\int d^4x\left[\bar\psi(i\not\partial-m)\psi
+\frac{g^2}{2}(\bar\psi\psi)^2+\bar\eta\psi+\bar\psi\eta\right]\right\}.
$$

The factor $\mathcal N$ cancels in $Z[\eta,\bar\eta]/Z[0,0]$. Every normalized [Green function](../../../../green-s-function-split.md) with only external [fermion](../../../../fermion.md) lines is a Grassmann source derivative of this same normalized [generating functional](../../../../generating-functional.md), so

$$
\boxed{G_{\mathrm{auxiliary}}^{(n)}=G_{\mathrm{four\text{-}fermion}}^{(n)}.}
$$

This is an exact [Hubbard–Stratonovich transformation](../../../../hubbard-stratonovich-transformation.md) in reverse, rather than just an approximation based on [tree-level Feynman diagrams](../../../../tree-level-feynman-diagram.md). At the diagrammatic level the contact [auxiliary-field propagator](../../../../auxiliary-field-propagator.md) $-i\delta^{(4)}(x-y)$ collapses each exchanged line into the same local [four-fermion interaction](../../../../four-fermion-interaction.md). The equality uses a common regulator and does not assert perturbative [renormalizability](../../../../renormalizable-quantum-field-theory.md) of that four-dimensional [four-fermion interaction](../../../../four-fermion-interaction.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
