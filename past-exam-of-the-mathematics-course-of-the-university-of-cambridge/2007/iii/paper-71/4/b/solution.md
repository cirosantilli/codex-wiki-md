<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $M$ interior points in each direction and spacing $h=1/(M+1)$. The one-dimensional [Dirichlet discrete Laplacian](../../../../../../dirichlet-discrete-laplacian.md) has sine eigenvectors $v_i^{(j)}=\sin(j\pi i h)$, because

$$
\frac{v_{i-1}^{(j)}-2v_i^{(j)}+v_{i+1}^{(j)}}{h^2}=-\frac4{h^2}\sin^2\left(\frac{j\pi h}{2}\right)v_i^{(j)}.
$$

The [five-point Dirichlet Laplacian as a Kronecker sum](../../../../../../five-point-dirichlet-laplacian-as-a-kronecker-sum.md) therefore has product eigenvectors $v_i^{(j)}v_r^{(\ell)}$. Adding the reaction term gives modal growth rates

$$
\lambda_{j\ell}=\kappa-\frac4{h^2}\left[\sin^2\left(\frac{j\pi h}{2}\right)+\sin^2\left(\frac{\ell\pi h}{2}\right)\right],\qquad1\leq j,\ell\leq M.
$$

The semidiscrete matrix is real symmetric, so these modes are orthogonal in the mesh-weighted [discrete L2 norm](../../../../../../discrete-l2-norm.md). Non-growth for all times is equivalent to every rate being nonpositive. The largest is $\lambda_{11}$, giving the [five-point heat-reaction stability threshold](../../../../../../five-point-heat-reaction-stability-threshold.md)

$$
\boxed{\kappa\leq\frac8{h^2}\sin^2\left(\frac{\pi h}{2}\right)=\frac4{h^2}(1-\cos\pi h).}
$$

At equality the first grid mode is neutral; above it that mode grows exponentially. This criterion concerns the spatially semidiscrete, continuous-time evolution. Any subsequent time integrator has an additional stability requirement.

The threshold expands as $2\pi^2-\pi^4h^2/6+O(h^4)$ and is below the continuum threshold for every finite mesh. Thus at the continuum neutral value the grid first mode has a small positive $O(h^2)$ rate. This is compatible with finite-time convergence, although it prevents an all-time contraction on that fixed mesh. In the weaker finite-time mesh-uniform sense, all fixed $\kappa$ have the bound $\|U(t)\|_h\leq e^{\kappa t}\|U(0)\|_h$ because the discrete Laplacian is nonpositive. The boxed range is the natural non-growing stability range, matching the threshold comparison in the preceding part; [finite-time stability versus power boundedness](../../../../../../finite-time-stability-versus-power-boundedness.md) is a distinct question.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
