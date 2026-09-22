<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [nematic director](../../../../../../nematic-director.md) is an unoriented axis: $\mathbf n$ and $-\mathbf n$ describe the same molecular alignment. A vector average cannot represent this head-tail symmetry. The orientational second moment $\langle n_in_j\rangle$ is a [symmetric second-rank tensor](../../../../../../symmetric-second-rank-tensor.md), and removing its isotropic part gives the [traceless second-rank tensor](../../../../../../traceless-second-rank-tensor.md) $Q_{ij}\propto\langle n_in_j-\delta_{ij}/2\rangle$. It vanishes for an isotropic angular distribution and transforms correctly under [rotation matrices](../../../../../../rotation-matrix.md).

Every nonzero real symmetric traceless $2\times2$ matrix has [eigenvalues](../../../../../../eigenvalue.md) $\lambda/2,-\lambda/2$ and can be written $Q=\lambda(\mathbf n\mathbf n^{\mathsf T}-I/2)$ by choosing the eigenvector of the positive eigenvalue as director and $\lambda\ge0$. Consequently $\operatorname{Tr}Q^2=\lambda^2/2$. The bulk [Landau-de Gennes free energy](../../../../../../landau-de-gennes-free-energy.md) becomes

$$
f_{\rm bulk}=\frac a2\lambda^2+\frac b4\lambda^4=\frac b4\left(\lambda^2+\frac ab\right)^2-\frac{a^2}{4b}.
$$

For $a<0$, its minimum occurs at $\lambda^2=-a/b$. The elastic density $K|\nabla\cdot Q|^2/2$ is nonnegative and vanishes for a uniform field. Thus, with no [boundary condition](../../../../../../boundary-condition.md) imposing a texture, the pointwise lower bound is attained by

$$
\boxed{\lambda_0=\sqrt{-a/b},\qquad Q_{ij}=\lambda_0(n_in_j-\delta_{ij}/2),\qquad f_{\min}=-a^2/(4b).}
$$

The negative-amplitude representation is equivalent in two dimensions to rotating the director by $\pi/2$, so the positive choice loses no tensor minima. This is minimization of the specified coarse-grained functional, not a claim of true thermodynamic long-range nematic order at every [temperature](../../../../../../temperature.md) in an infinite two-dimensional system. The PDF explicitly uses the divergence elastic term; the TeX's $|\nabla Q|^2$ loses the dot and would give different elastic coefficients.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
