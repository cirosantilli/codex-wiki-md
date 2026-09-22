# Positive definiteness of degree on elliptic-curve homomorphisms

↑ **Parent:** [Degree of an isogeny](degree-of-an-isogeny.md)

Let $q(\phi)=\deg\phi$ for nonzero elements of the [homomorphism group of elliptic curves](homomorphism-group-of-elliptic-curves.md), and $q(0)=0$. For an [elliptic curve](elliptic-curve.md) $E$, the degree-two coordinate $x$ on a [Weierstrass model](weierstrass-equation-of-an-elliptic-curve.md) has a double pole at its identity and identifies a generic point only with its inverse. Thus on $E\times E$,

$$
\operatorname{div}(x(P)-x(Q))=\Delta+\Delta_- -2(\{O\}\times E)-2(E\times\{O\}),
$$

where the two diagonals are $P=Q$ and $P=-Q$. The resulting [line bundle](line-bundle.md) isomorphism is $a^*\mathcal O_E(O)\otimes s^*\mathcal O_E(O)\cong\operatorname{pr}_1^*\mathcal O_E(O)^{\otimes2}\otimes\operatorname{pr}_2^*\mathcal O_E(O)^{\otimes2}$, for the sum and difference maps $a,s$. Pull it back along $(\phi,\psi)$ and take degrees. This gives the [degree parallelogram law](divisor-proof-of-the-degree-parallelogram-law.md), even when one homomorphism equals plus or minus the other: bundle restriction remains valid in these cases.

It implies $q(n\phi)=n^2q(\phi)$ by the second-difference recursion, and polarization gives the symmetric bilinear form $B(\phi,\psi)=(q(\phi+\psi)-q(\phi-\psi))/4$. To check additivity, the parallelogram law gives $B(x+z,y)+B(x-z,y)=2B(x,y)$; interchange $x,z$ and use oddness to get $B(x+z,y)-B(x-z,y)=2B(z,y)$. Adding proves bilinearity. Since a nonzero isogeny has positive degree, $q$ is positive on every nonzero element. On every finite-dimensional rational span the matrix of $B$ is rational. Positivity on rational vectors implies nonnegativity on real vectors by density; a nontrivial kernel of a rational matrix would contain a nonzero rational vector. Hence the real extension is positive definite. This proves the [positive-definite quadratic form](positive-definite-quadratic-form.md) property, rather than only a parallelogram identity.

**Table of contents**

- [Bilinear degree pairing for elliptic-curve homomorphisms](bilinear-degree-pairing-for-elliptic-curve-homomorphisms.md)

## ↑ Ancestors (11)

1. [Degree of an isogeny](degree-of-an-isogeny.md)
2. [Isogeny of elliptic curves](isogeny-of-elliptic-curves.md)
3. [Elliptic curve](elliptic-curve.md)
4. [Genus one curve](genus-one-curve.md)
5. [Geometric genus](geometric-genus.md)
6. [Normalization of an algebraic curve](normalization-of-an-algebraic-curve-split.md)
7. [Algebraic geometry](algebraic-geometry-split.md)
8. [Geometry and topology](geometry-and-topology-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-21/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-27/3/a/solution.md)
