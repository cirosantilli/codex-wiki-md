<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If $E$ has local frame transition matrices $g_{ab}$ and the cotangent bundle has transitions $J_{ab}^{-T}$, then $E\otimes\Lambda^rT^*B$ has local trivializations with transitions

$$
g_{ab}\otimes\Lambda^r(J_{ab}^{-T}),
$$

which satisfy the cocycle condition. Thus it is a well-defined [tensor product of vector bundles](../../../../../../tensor-product-of-vector-bundles.md).

A [connection on a vector bundle](../../../../../../connection-vector-bundle.md) is a linear map

$$
\nabla:\Gamma(E)\to\Omega^1(B;E)
$$

satisfying $\nabla(fs)=df\otimes s+f\nabla s$. Contracting with a vector field gives the covariant derivative $\nabla_Xs$. In a local frame, $\nabla=d+A$ for a matrix-valued one-form $A$; under a frame change $g$ the matrix transforms as

$$
A'=g^{-1}Ag+g^{-1}dg.
$$

Its [covariant exterior derivative](../../../../../../exterior-covariant-derivative.md) is defined by

$$
d_A(s\otimes\alpha)=\nabla s\wedge\alpha+s\otimes d\alpha,
$$

and locally

$$
d_A\eta=d\eta+A\wedge\eta.
$$

This formula and the graded Leibniz rule show that definitions in different frames agree.

The [curvature form of a connection](../../../../../../curvature-form.md) is $F(A)=d_A^2$. Locally,

$$
F(A)=dA+A\wedge A.
$$

Its covariant derivative satisfies the [Bianchi identity](../../../../../../bianchi-identity.md)

$$
d_AF=dF+A\wedge F-F\wedge A=0.
$$

Indeed, substituting $F=dA+A\wedge A$, using $d^2=0$, and applying the graded Leibniz rule leaves equal and opposite terms.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
