<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take a smooth [gauge transformation](../../../../../gauge-transformation.md) $g:\mathbb R^3\to SU(2)$. In the anti-Hermitian convention of the [adjoint covariant derivative](../../../../../adjoint-covariant-derivative.md), set

$$
\boxed{\Phi^g=g\Phi g^{-1},\qquad A_j^g=gA_jg^{-1}-(\partial_jg)g^{-1}.}
$$

Expanding $\partial_j(g\Phi g^{-1})$ shows that its two differentiated-$g$ terms cancel with the extra terms in $[A_j^g,\Phi^g]$. Thus $D_j^g\Phi^g=g(D_j\Phi)g^{-1}$. The [gauge field strength](../../../../../gauge-field-strength.md) is $F_{jk}=\partial_jA_k-\partial_kA_j+[A_j,A_k]$, and the same cancellation, or the commutator of covariant derivatives, gives $F_{jk}^g=gF_{jk}g^{-1}$.

The [matrix trace](../../../../../matrix-trace.md) is unchanged by conjugation, so

$$
\langle gXg^{-1},gYg^{-1}\rangle=-\operatorname{tr}(gXYg^{-1})=-\operatorname{tr}(XY)=\langle X,Y\rangle.
$$

Each field-strength norm, covariant-gradient norm and Higgs norm is therefore invariant pointwise. It follows that **$V_\lambda(A^g,\Phi^g)=V_\lambda(A,\Phi)$**. The displayed tensor made from these fields is also gauge invariant wherever $\Phi\ne0$.

There is a normalization problem in the requested final identity. With the ordinary defining $2\times2$ trace and the printed [inner product](../../../../../inner-product.md), an explicit orthonormal basis is

$$
e_a=-\frac{i\sigma_a}{\sqrt2},\qquad -\operatorname{tr}(e_ae_b)=\delta_{ab},\qquad
[e_a,e_b]=\kappa\varepsilon_{abc}e_c,\quad\kappa=\sqrt2.
$$

The last identity follows from the [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md). In particular it is not permissible to combine this orthonormality with unit [structure constants of a Lie algebra](../../../../../structure-constant-of-a-lie-algebra.md).

Write $A_j=a_j^ae_a$ and $\Phi=\varphi e_3$ with $\varphi\ne0$, and put $s=\operatorname{sgn}\varphi$. Define $C_{jk}=a_j^1a_k^2-a_j^2a_k^1$. Then

$$
\langle F_{jk},e_3\rangle=\partial_ja_k^3-\partial_ka_j^3+\kappa C_{jk},\qquad
D_j\Phi=(\partial_j\varphi)e_3+\kappa\varphi(a_j^2e_1-a_j^1e_2).
$$

Only the bracket of the transverse terms contributes in the $e_3$ direction, giving

$$
\langle\Phi,[D_j\Phi,D_k\Phi]\rangle=\kappa^3\varphi^3C_{jk}.
$$

Hence the literal tensor printed in the question is

$$
\boxed{f_{jk}=s\bigl[\partial_ja_k^3-\partial_ka_j^3+(\kappa-\kappa^3)C_{jk}\bigr]
=s\bigl[\partial_ja_k^3-\partial_ka_j^3-\sqrt2 C_{jk}\bigr].}
$$

The transverse term does not cancel with this [trace normalization of su(2)](../../../../../trace-normalization-of-su-2.md).

A concrete counterexample to the printed closure assertion is $\Phi=e_3$, $A_1=e_1$, $A_2=x_3e_2$, $A_3=0$ on a ball. Directly, $F_{12}=\sqrt2x_3e_3$, $F_{23}=-e_2$ and $F_{31}=0$, while $D_1\Phi=-\sqrt2e_2$, $D_2\Phi=\sqrt2x_3e_1$ and $D_3\Phi=0$. It follows that

$$
f_{12}=-\sqrt2x_3,\qquad f_{23}=f_{31}=0,\qquad
\boxed{\partial_3f_{12}+\partial_1f_{23}+\partial_2f_{31}=-\sqrt2\ne0.}
$$

The [Higgs field](../../../../../higgs-field.md) never vanishes. If global finite energy is desired, multiply both nonzero gauge-potential components by a smooth compactly supported cutoff equal to one on this ball and keep $\Phi=e_3$ everywhere. The energy is finite and the same local counterexample remains. Thus **the claimed closure is false with the ordinary trace normalization actually printed**; it is not a consequence of gauge invariance alone.

The consistent ['t Hooft electromagnetic tensor](../../../../../t-hooft-electromagnetic-tensor.md) for the printed inner product is instead

$$
\boxed{\mathcal F_{jk}=\left\langle F_{jk},\frac\Phi{|\Phi|}\right\rangle
-\frac1{2|\Phi|^3}\langle\Phi,[D_j\Phi,D_k\Phi]\rangle.}
$$

In the directional gauge, its commutator coefficient is $1/\kappa^2$, so the terms cancel exactly and

$$
\mathcal F_{jk}=s(\partial_ja_k^3-\partial_ka_j^3).
$$

On a connected region where $\varphi\ne0$, $s$ is constant. Commutation of ordinary partial derivatives proves

$$
\boxed{\partial_i\mathcal F_{jk}+\partial_j\mathcal F_{ki}+\partial_k\mathcal F_{ij}=0.}
$$

At any nonzero-Higgs point, use the permitted local [gauge transformation](../../../../../gauge-transformation.md) to align the field with a fixed internal direction. Since $\mathcal F$ is gauge invariant, the identity derived in that gauge holds in the original gauge on the same ball. These balls cover every nonzero-Higgs region, proving that the corrected tensor is a [closed differential form](../../../../../closed-differential-form.md) there.

Alternatively, keeping the tensor's printed coefficient one but replacing the inner product by $-2\operatorname{tr}(XY)$ gives the orthonormal basis $e_a=-i\sigma_a/2$ with $\kappa=1$. The same calculation then gives $f_{jk}=s(\partial_ja_k^3-\partial_ka_j^3)$ and the intended identity. Either repair makes the bracket and inner-product normalizations agree; they must not be silently mixed.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
