<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

Here [isotropic tensors](../../../../../isotropic-tensor.md) are invariant under proper [rotation matrices](../../../../../rotation-matrix.md), $R^TR=I$ and $\det R=1$. The [isotropic second-rank tensor](../../../../../isotropic-second-rank-tensor.md) and [isotropic third-rank tensor](../../../../../isotropic-third-rank-tensor.md) forms in three dimensions are

$$
\boxed{T_{ij}=A\delta_{ij},\qquad T_{ijk}=B\epsilon_{ijk},}
$$

with scalar coefficients $A,B$. One can see completeness directly. A half-turn about each coordinate axis kills every off-diagonal component of a rank-two [tensor](../../../../../tensor.md), and quarter-turns make its three diagonal components equal. For rank three, the half-turns require that each coordinate label occur an odd number of times in a nonzero component. Thus only permutations of $(1,2,3)$ survive. Quarter-turns interchange two labels while reversing one sign, forcing the surviving components to alternate with the [parity of a permutation](../../../../../parity-of-a-permutation.md). This gives a multiple of the [Levi-Civita symbol](../../../../../levi-civita-symbol.md).

The [tensor](../../../../../tensor.md) transformation law verifies invariance of these forms:

$$
T'_{ij}=AR_{ip}R_{jq}\delta_{pq}=A\delta_{ij},\qquad
T'_{ijk}=BR_{ip}R_{jq}R_{kr}\epsilon_{pqr}=B(\det R)\epsilon_{ijk}=B\epsilon_{ijk}.
$$

The first equality uses [orthogonality](../../../../../orthogonal-vectors.md) and the second uses the [determinant](../../../../../determinant.md) formula. If reflections were also required while using the ordinary [tensor](../../../../../tensor.md) transformation law, the rank-three coefficient would have to vanish. The proper-rotation convention is the one under which $B\epsilon_{ijk}$ is an [isotropic tensor](../../../../../isotropic-tensor.md).

The ball is unchanged by any [rotation matrix](../../../../../rotation-matrix.md), and rotating coordinates has [Jacobian determinant](../../../../../jacobian-determinant.md) one. Thus changing variables $\mathbf y=R\mathbf x$ gives

$$
R_{i_1j_1}\cdots R_{i_nj_n}\int_Vx_{j_1}\cdots x_{j_n}\,dV
=\int_Vy_{i_1}\cdots y_{i_n}\,dV=T_{i_1\cdots i_n}.
$$

These moments are therefore [isotropic tensor integrals](../../../../../isotropic-tensor-integral.md). For the [Cartesian moments of a three-dimensional ball](../../../../../cartesian-moments-of-a-three-dimensional-ball.md), the second moment is $\alpha\delta_{ij}$. Taking its [tensor contraction](../../../../../tensor-contraction.md) gives

$$
3\alpha=\int_Vr^2\,dV=4\pi\int_0^a r^4\,dr=\frac{4\pi a^5}{5},\qquad
\boxed{\alpha=\frac{4\pi a^5}{15}.}
$$

The third moment vanishes: $\mathbf x\mapsto-\mathbf x$ preserves the ball and changes the sign of its integrand. Equivalently, its symmetry under index interchange excludes a nonzero multiple of the antisymmetric [Levi-Civita symbol](../../../../../levi-civita-symbol.md).

The fourth moment is symmetric under every [permutation](../../../../../permutation.md) of its four indices. The general rank-four [isotropic tensor](../../../../../isotropic-tensor.md) form consequently has equal coefficients, yielding

$$
T_{ijkl}=\beta(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}).
$$

For example, comparing $T_{1122},T_{1212},T_{1221}$ shows that the three coefficients agree. Contracting $i=j$ and $k=l$ gives

$$
15\beta=\int_V r^4\,dV=4\pi\int_0^a r^6\,dr=\frac{4\pi a^7}{7},\qquad
\boxed{\beta=\frac{4\pi a^7}{105}.}
$$

Finally the [vector triple product identity](../../../../../vector-triple-product.md) gives $\mathbf x\times(\boldsymbol\Omega\times\mathbf x)=r^2\boldsymbol\Omega-(\boldsymbol\Omega\cdot\mathbf x)\mathbf x$. The first term integrates to $3\alpha\boldsymbol\Omega$ and the second to $\alpha\boldsymbol\Omega$, using the second moment. Hence

$$
\boxed{\int_V\mathbf x\times(\boldsymbol\Omega\times\mathbf x)\,dV=\frac{8\pi a^5}{15}\boldsymbol\Omega.}
$$

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
