<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Polar deformation reduces maps from the circle into $GL_N$ to maps into $U(N)$. Define their integer invariant by the [winding number](../../../../../../winding-number.md) of the determinant. It is unchanged under [homotopy](../../../../../../homotopy.md) and stabilization, and determinants multiply under block sum, so it gives a homomorphism $K^1(S^1)\to\mathbb Z$. Every integer occurs, via $z\mapsto\operatorname{diag}(z^m,1,\ldots,1)$.

To prove injectivity, first consider a map with determinant winding zero. Its determinant has a continuous logarithm $ih(z)$ on the circle. Multiplying the first row by $e^{-ith(z)}$ gives a [homotopy](../../../../../../homotopy.md) into $SU(N)$ at $t=1$. If $N=1$ that endpoint is already the identity. For $N\geq2$, $SU(N)$ is simply connected: $SU(2)\cong S^3$, and the last-column fibration

$$
SU(N-1)\longrightarrow SU(N)\longrightarrow S^{2N-1}
$$

with locally trivializations from orthonormal completion, together with its [homotopy](../../../../../../homotopy.md) exact sequence, proves this inductively because the sphere has zero first and second [homotopy](../../../../../../homotopy.md) groups. Thus the remaining circle map is null-homotopic. For a map of winding $m$, multiply by $\operatorname{diag}(z^{-m},1,\ldots,1)$ and apply the zero-winding argument. This proves

$$
\boxed{K^1(S^1)\cong\mathbb Z.}
$$

For higher spheres, stable unitary [homotopy](../../../../../../homotopy.md) gives $K^1(S^n)=\pi_n(U)$: a map can be normalized by multiplying by the inverse of its value at the basepoint, a free [homotopy](../../../../../../homotopy.md) because the [unitary group](../../../../../../unitary-group.md) is path connected. A free [homotopy](../../../../../../homotopy.md) between based maps can be made based by replacing $H(x,t)$ with $H(x_0,t)^{-1}H(x,t)$, without altering its endpoints. The [Bott periodicity theorem](../../../../../../bott-isomorphism.md), in its unitary form $\pi_{j+2}(U)\cong\pi_j(U)$ with $\pi_0(U)=0$ and $\pi_1(U)=\mathbb Z$, gives

$$
\boxed{K^1(S^n)\cong\begin{cases}\mathbb Z,&n\text{ odd},\\0,&n\text{ even}.\end{cases}}
$$

The circle case was proved directly above; the higher-sphere values use the stated general periodicity theorem.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [7](../../7.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
