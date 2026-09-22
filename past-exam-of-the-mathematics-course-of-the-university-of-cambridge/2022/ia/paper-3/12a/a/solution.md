<h1 id="12a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let a change of orthonormal coordinates be represented by a [rotation matrix](../../../../../../rotation-matrix.md) $R$. Since both [angular momentum](../../../../../../angular-momentum.md) and [angular velocity](../../../../../../angular-velocity.md) are vectors,

$$
L'_i=R_{ip}L_p,
\qquad
\omega'_j=R_{jq}\omega_q.
$$

Using $L_i=I_{ij}\omega_j$ in both frames gives

$$
I'_{ij}R_{jq}\omega_q=R_{ip}I_{pq}\omega_q
$$

for every vector $\boldsymbol\omega$. Multiplication by $R^{-1}=R^T$ yields

$$
\boxed{I'_{ij}=R_{ip}R_{jq}I_{pq}},
$$

which is exactly the transformation law for a rank-two [tensor](../../../../../../tensor.md). Thus $I_{ij}$ is a rank-two tensor.

Put $\mathbf r=\mathbf x-\mathbf a$. The [vector triple product](../../../../../../vector-triple-product.md) gives

$$
\mathbf r\times(\boldsymbol\omega\times\mathbf r)
=r^2\boldsymbol\omega
-\mathbf r(\mathbf r\cdot\boldsymbol\omega).
$$

Therefore

$$
\boxed{
I_{ij}(\mathbf a)
=\rho\int_B
\left[(x_k-a_k)(x_k-a_k)\delta_{ij}
-(x_i-a_i)(x_j-a_j)\right]dV}.
$$

At the centre of mass,

$$
\boxed{
I_{ij}(\mathbf0)
=\rho\int_B(x_kx_k\delta_{ij}-x_ix_j)\,dV}.
$$

Expanding the first formula, the terms linear in $x_i$ vanish because the centre of mass is the origin, while $\rho\int_BdV=M$. Hence the [parallel axis theorem](../../../../../../parallel-axis-theorem.md) in tensor form is

$$
\boxed{
I_{ij}(\mathbf a)
=I_{ij}(\mathbf0)
+M(a_ka_k\delta_{ij}-a_ia_j)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12A](../../12a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
