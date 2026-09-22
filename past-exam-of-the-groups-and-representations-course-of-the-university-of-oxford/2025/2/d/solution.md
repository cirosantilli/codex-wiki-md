<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the normalization $c(\mathbf8)=1$ of [c](../c.md), the [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md) of $D_4$ has [highest weight](../../../../highest-weight-of-a-representation.md) $\lambda_{\mathrm{adj}}=(0,1,0,0)$, the [highest root](../../../../highest-root.md). The supplied [Gram matrix](../../../../gram-matrix.md) has second row $(1,2,1,1)$, whose sum is five. Hence

$$
C_2(\mathrm{adj})=\frac12(2+2\cdot5)=6.
$$

The [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md) has the same dimension as the [Lie algebra](../../../../lie-algebra-split.md), so its [Dynkin index](../../../../dynkin-index.md) is also $c(\mathrm{adj})=6$. The $k$ [Weyl fermions](../../../../weyl-spinor.md) form a [direct sum](../../../../direct-sum.md) of $k$ vector [representations](../../../../group-representation.md); additivity of the [trace](../../../../matrix-trace.md) gives $c(r_W)=k$.

Substitution into the given one-loop [renormalization-group beta function](../../../../beta-function-physics.md) yields

$$
\boxed{\beta(g)=-\frac{g^3}{16\pi^2}\left(22-\frac{2k}{3}\right)
=-\frac{33-k}{24\pi^2}g^3.}
$$

For positive $g$, [asymptotic freedom](../../../../asymptotic-freedom.md) at this order requires a negative [beta function](../../../../beta-function.md), equivalently

$$
\boxed{k<33;\quad\text{for a nonnegative integer number of fermions, }k=0,1,\ldots,32.}
$$

Indeed, if $b_0=22-2k/3>0$, integrating $\mu\,dg/d\mu=-b_0g^3/(16\pi^2)$ gives

$$
\frac1{g^2(\mu)}=\frac1{g^2(\mu_0)}+\frac{b_0}{8\pi^2}\log\frac\mu{\mu_0},
$$

so the [gauge coupling](../../../../gauge-coupling.md) decreases towards zero as the energy scale increases. At $k=33$ the one-loop coefficient vanishes and the given equation cannot decide [asymptotic freedom](../../../../asymptotic-freedom.md); $k>33$ has the opposite one-loop running.

With the alternative convention $C(\lambda)=\lambda^TG(\lambda+2\mathbf1)$ described in [c](../c.md), $c(\mathbf8)=2$, $c(\mathrm{adj})=12$, and the same source formula reads $\beta(g)=-(44-4k/3)g^3/(16\pi^2)$. Rescaling the [gauge coupling](../../../../gauge-coupling.md) together with the [Lie algebra generators](../../../../lie-algebra-generator.md) relates the conventions; the bound $k<33$ is identical.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
