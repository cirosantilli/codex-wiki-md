<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A Cartesian [tensor](../../../../tensor.md) of order $n$ is a multilinear geometric object whose components under an orthogonal change of axes obey the [tensor component transformation law](../../../../tensor-component-transformation-law.md),

$$
T'_{i_1\cdots i_n}=Q_{i_1j_1}\cdots Q_{i_nj_n}T_{j_1\cdots j_n},\qquad Q^TQ=I.
$$

An [isotropic tensor](../../../../isotropic-tensor.md) has the same components under every proper rotation. For the [Kronecker delta](../../../../kronecker-delta.md),

$$
\delta'_{ij}=Q_{ip}Q_{jq}\delta_{pq}=Q_{ip}Q_{jp}=\delta_{ij}.
$$

Thus **$\delta_{ij}$ is isotropic**, even under improper orthogonal transformations.

To prove [multiplicativity of the determinant](../../../../multiplicativity-of-the-determinant.md) from the given formula, first consider $C_{pqr}=\epsilon_{ijk}A_{ip}A_{jq}A_{kr}$. Exchanging any two of $p,q,r$ changes its sign, so it is proportional to the [Levi-Civita symbol](../../../../levi-civita-symbol.md). Its $123$ component is the determinant, as follows by expanding the given double-epsilon expression. Therefore

$$
\epsilon_{ijk}A_{ip}A_{jq}A_{kr}=(\det A)\epsilon_{pqr}.
$$

Substitute $(AB)_{il}=A_{ip}B_{pl}$ into that same determinant formula:

$$
\begin{aligned}
\det(AB)&=\frac16\epsilon_{ijk}\epsilon_{lmn}A_{ip}B_{pl}A_{jq}B_{qm}A_{kr}B_{rn}\\
&=\frac{\det A}{6}\epsilon_{pqr}\epsilon_{lmn}B_{pl}B_{qm}B_{rn}=(\det A)(\det B).
\end{aligned}
$$

Hence

$$
\boxed{\det(AB)=\det A\det B.}
$$

No invertibility assumption was used, so this identity includes singular matrices.

Now differentiate the double-epsilon formula for a differentiable $A(t)$. Its three differentiated terms are equal after renaming the paired dummy indices: the simultaneous swaps in both epsilon symbols cancel their signs. Thus

$$
\frac d{dt}\det A=\frac12\epsilon_{ijk}\epsilon_{lmn}\dot A_{il}A_{jm}A_{kn}=C_{il}\dot A_{il},
$$

where $C_{il}$ is the cofactor of entry $A_{il}$. For an invertible matrix, the [adjugate matrix](../../../../adjugate-matrix.md) identity gives $C_{il}=(\det A)(A^{-1})_{li}$. Consequently the [Jacobi determinant derivative formula](../../../../jacobi-determinant-derivative-formula.md) is

$$
\boxed{\frac d{dt}\det A=(\det A)\sum_{i,l}(A^{-1})_{li}\dot A_{il}=(\det A)\operatorname{tr}(A^{-1}\dot A).}
$$

The order of the factors inside the trace follows from the reversed cofactor indices; no commutativity of $A$ and $\dot A$ is assumed. The cofactor version is also [Jacobi's formula](../../../../jacobi-s-formula.md) and remains valid when $A$ is singular, although the inverse version then cannot be used.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [2012](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
