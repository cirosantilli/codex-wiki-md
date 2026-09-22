<h1 id="16h/solution">Solution</h1>

↑ **Parent:** [16H](../16h.md)

An [isotropic tensor](../../../../../isotropic-tensor.md) has unchanged components under every proper orthogonal change of basis: $T_{i_1\ldots i_n}=R_{i_1j_1}\cdots R_{i_nj_n}T_{j_1\ldots j_n}$ for every $R\in SO(3)$. Orthogonality gives $R_{ia}R_{jb}\delta_{ab}=\delta_{ij}$, so the [Kronecker delta](../../../../../kronecker-delta.md) is isotropic. The determinant identity gives $R_{ia}R_{jb}R_{kc}\epsilon_{abc}=(\det R)\epsilon_{ijk}=\epsilon_{ijk}$, so the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) is isotropic too. If reflections are included, this last object is a pseudotensor: it changes sign. The question's isotropy convention therefore refers to proper rotations.

For the sphere moment $T_{i_1\ldots i_n}=\int_{S^2}\hat x_{i_1}\cdots\hat x_{i_n}\,dS$, change variables to $R\hat x$. Rotations preserve the sphere and its area measure; inserting the component transformation proves that $T$ is an [isotropic tensor](../../../../../isotropic-tensor.md). For the second moment, half-turns about coordinate axes kill the off-diagonal components, while rotations interchanging axes make the diagonal entries equal. Thus it is a multiple $a\delta_{ij}$. Contracting the indices gives $3a=\int_{S^2}|\hat x|^2dS=4\pi$. Odd moments vanish by $\hat x\mapsto-\hat x$, including the third moment. The supplied general fourth-rank form and symmetry under every permutation of the four indices make its three coefficients equal. A double contraction then gives $4\pi=b(9+3+3)$. Thus

$$
\boxed{\int\hat x_i\hat x_j\,dS=\frac{4\pi}{3}\delta_{ij},\qquad \int\hat x_i\hat x_j\hat x_k\,dS=0,}
$$



$$
\boxed{\int\hat x_i\hat x_j\hat x_k\hat x_l\,dS=\frac{4\pi}{15}(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}).}
$$

To explain the weighted volume integrals, put $v=(1,i,0)$; its bilinear square is $v\cdot v=1+i^2=0$, without complex conjugation. Separating radial and angular factors gives

$$
\int_{|x|<1}(x_1+ix_2)^nf(|x|)\,d^3x
=\left(\int_0^1r^{n+2}f(r)\,dr\right)\int_{S^2}(v\cdot\hat x)^n\,dS.
$$

For $n=2$ the angular factor is $(4\pi/3)v\cdot v=0$. For $n=3$ it is zero by oddness. For $n=4$ it is $(4\pi/15)3(v\cdot v)^2=0$. Therefore **all three requested integrals vanish**, assuming the radial integrals exist. More generally the [null-vector cancellation of radial moments](../../../../../null-vector-cancellation-of-radial-moments.md) follows from rotation about the third axis, which multiplies the integral by $e^{in\phi}$ without otherwise changing it.

## ↑ Ancestors (10)

1. [16H](../16h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
