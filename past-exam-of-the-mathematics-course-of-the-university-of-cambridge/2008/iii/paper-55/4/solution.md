<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the [adjoint covariant derivative](../../../../../adjoint-covariant-derivative.md) $D_i=\partial_i+[A_i,\cdot]$, the [gauge curvature](../../../../../gauge-field-strength.md) is

$$
\boxed{F=dA+A\wedge A,\qquad
F_{ij}=\partial_iA_j-\partial_jA_i+[A_i,A_j].}
$$

The matrix-valued wedge product gives one commutator in each $dx^i\wedge dx^j$ coefficient; $[D_i,D_j]\Phi=[F_{ij},\Phi]$ follows directly. The given trace defines a real positive [inner product](../../../../../inner-product.md) on the anti-Hermitian algebra $\mathfrak{su}(2)$.

The additional terms in $\langle D_j\Phi,\Psi\rangle+\langle\Phi,D_j\Psi\rangle$, compared with ordinary differentiation, are

$$
-\frac12\operatorname{tr}\left([A_j,\Phi]\Psi+\Phi[A_j,\Psi]\right)
=-\frac12\operatorname{tr}[A_j,\Phi\Psi]=0.
$$

Thus trace cyclicity proves the compatibility identity

$$
\boxed{\partial_j\langle\Phi,\Psi\rangle
=\langle D_j\Phi,\Psi\rangle+\langle\Phi,D_j\Psi\rangle.}
$$

With compactly supported variations, this gives covariant integration by parts without boundary contributions.

Use $F_{ij}=\epsilon_{ijk}B_k$, so $|B|^2=\tfrac12\sum_{i,j}|F_{ij}|^2$. Write the independent variations as $\delta A_i=a_i$ and $\delta\Phi=\chi$. The curvature and Higgs derivative variations are

$$
\delta F_{ij}=D_i a_j-D_j a_i,\qquad
\delta(D_i\Phi)=D_i\chi+[a_i,\Phi].
$$

The variation of the [Yang-Mills theory](../../../../../yang-mills-theory.md) magnetic energy is

$$
\delta\int|B|^2d^3x
=2\int\sum_{i,j}\langle F_{ij},D_i a_j\rangle d^3x
=-2\int\sum_{i,j}\langle D_iF_{ij},a_j\rangle d^3x.
$$

For the [Higgs field](../../../../../higgs-field.md) derivative energy, trace cyclicity also gives $\langle X,[a,\Phi]\rangle=\langle[\Phi,X],a\rangle$. Hence

$$
\delta\int|D\Phi|^2d^3x
=-2\int\left\langle\sum_iD_iD_i\Phi,\chi\right\rangle d^3x
+2\int\sum_i\langle[\Phi,D_i\Phi],a_i\rangle d^3x.
$$

Arbitrariness of the variations proves the [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md)

$$
\boxed{\sum_iD_iD_i\Phi=0,\qquad
\sum_iD_iF_{ij}=[\Phi,D_j\Phi]\quad(j=1,2,3).}
$$

The gauge equation can equivalently be written $(D\times B)_j+[\Phi,D_j\Phi]=0$, where $(D\times B)_j=\epsilon_{jik}D_iB_k$. This equivalent form also checks the sign of the commutator source.

Now suppose the positive-sign [Bogomolny equations](../../../../../bogomolny-equations.md) $B_i=D_i\Phi$ hold. The [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) $D_iF_{jk}+D_jF_{ki}+D_kF_{ij}=0$ implies $\sum_iD_iB_i=0$, and therefore $\sum_iD_iD_i\Phi=0$. For the gauge equation,

$$
(D\times B)_i
=\epsilon_{ijk}D_jD_k\Phi
=\frac12\epsilon_{ijk}[D_j,D_k]\Phi
=\frac12\epsilon_{ijk}[F_{jk},\Phi]
=[B_i,\Phi].
$$

Consequently $(D\times B)_i+[\Phi,D_i\Phi]=[B_i,\Phi]+[\Phi,B_i]=0$. Thus **the first-order Bogomolny equations imply both second-order field equations**. The negative-sign convention works as well, with both occurrences of that sign tracked consistently.

Finally differentiate the norm twice, using the trace compatibility identity at each step:

$$
\Delta|\Phi|^2
=2\sum_i|D_i\Phi|^2+2\left\langle\Phi,\sum_iD_iD_i\Phi\right\rangle.
$$

The second term vanishes, and $|B|^2=|D\Phi|^2$ for the [Bogomolny equations](../../../../../bogomolny-equations.md). Thus the [Higgs norm identity for a Bogomolny monopole](../../../../../higgs-norm-identity-for-a-bogomolny-monopole.md) gives

$$
\boxed{\Delta|\Phi|^2=2|D\Phi|^2=|B|^2+|D\Phi|^2=v(A,\Phi).}
$$

There is no extra factor 2 multiplying $v$: the printed energy density already contains both equal terms without an overall $1/2$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
