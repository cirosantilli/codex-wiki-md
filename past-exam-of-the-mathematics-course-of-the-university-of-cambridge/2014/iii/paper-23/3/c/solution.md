<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The effective group is torsion free and every [modular cusp](../../../../../../cusp-of-a-modular-group.md) is regular in the preceding sense, so orders of a meromorphic weight-$k$ form are integers. At interior points use a local automorphy trivialization; at a [modular cusp](../../../../../../cusp-of-a-modular-group.md) use the Fourier order of the appropriate slash transform in its [cusp width](../../../../../../width-of-a-cusp.md) coordinate. Let $C$ be the sum of all [modular cusp](../../../../../../cusp-of-a-modular-group.md) points, each once, and set

$$
\boxed{D(f)=\sum_{P\in X(\Gamma_1(p))}\operatorname{ord}_P(f)P-C.}
$$

A [meromorphic function](../../../../../../meromorphic-function.md) $\varphi$ belongs to the [Riemann-Roch space](../../../../../../riemann-roch-space.md) $\mathcal L(D(f))$ exactly when $\operatorname{div}\varphi+D(f)\ge0$. In the interior this requires $f\varphi$ to have no [pole](../../../../../../pole.md); at a [modular cusp](../../../../../../cusp-of-a-modular-group.md) it requires order at least one. Conversely, the quotient of any weight-$k$ [cusp form](../../../../../../cusp-form.md) by $f$ is a meromorphic weight-zero function satisfying precisely those inequalities. This proves the [cusp-form divisor presentation](../../../../../../cusp-form-divisor-presentation.md)

$$
\boxed{S_k(\Gamma_1(p))=f\,\mathcal L(D(f)).}
$$

To compute the degree without imposing a valence formula as an extra assumption, use the meromorphic tensor differential $f^{12}(d\tau)^{6k}$. Its automorphy factors cancel. Its order at an interior point is $12\operatorname{ord}_P f$; at a [modular cusp](../../../../../../cusp-of-a-modular-group.md) it is $12\operatorname{ord}_P f-6k$, since $d\tau$ is a nonzero constant times $dq_c/q_c$. A meromorphic section of the $6k$th [tensor power](../../../../../../tensor-power.md) of the [canonical bundle](../../../../../../canonical-bundle.md) has total divisor degree $6k(2g-2)$. The [regular-cusp valence formula on a torsion-free modular curve](../../../../../../regular-cusp-valence-formula-on-a-torsion-free-modular-curve.md) is therefore

$$
\sum_P\operatorname{ord}_P f=\frac k2(2g-2+r_\infty)=\frac{kd}{12},\qquad
\deg D(f)=\frac{kd}{12}-r_\infty.
$$

For $k\ge3$, $\deg D(f)-(2g-2)=(k-2)d/12>0$. The [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) says $\ell(D)-\ell(K-D)=\deg D+1-g$, and a divisor of negative degree has no nonzero sections. Thus $\ell(K-D)=0$ and

$$
\dim S_k=\frac{kd}{12}-r_\infty+1-g=\frac{(k-1)d}{12}-\frac{r_\infty}{2}.
$$

Using $d=(p^2-1)/2$ and $r_\infty=p-1$ gives

$$
\boxed{\dim S_k(\Gamma_1(p))=\frac{p-1}{24}\bigl((p+1)(k-1)-12\bigr),\qquad k\ge3.}
$$

The canonical-degree and Riemann-Roch facts used here are general results for compact [Riemann surfaces](../../../../../../riemann-surfaces.md), as permitted.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
