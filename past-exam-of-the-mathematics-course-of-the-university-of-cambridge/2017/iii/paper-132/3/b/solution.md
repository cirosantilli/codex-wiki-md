<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In local [holomorphic coordinates](../../../../../../holomorphic-coordinate.md), write the two positive [singular values](../../../../../../singular-value.md) of $Df$ as $s_1\geq s_2$. Preservation of [orientation](../../../../../../orientation-of-a-simplex.md) gives $J_f=s_1s_2$, and [quasiconformality](../../../../../../quasiconformal-mapping.md) gives $s_1/s_2\leq K$.

For an admissible [conformal metric](../../../../../../conformal-metric.md) $\rho|dw|$ on $Y$, define a density on $X$ by $\sigma(z)=\rho(f(z))s_1(z)$. Along each path,

$$
\int_{f(\gamma)}\rho|dw|
\leq\int_\gamma\sigma|dz|,
$$

so $L_\rho(f(\Gamma))\leq L_\sigma(\Gamma)$. The [change of variables formula](../../../../../../change-of-variables-formula.md) and $s_1^2\leq KJ_f$ give

$$
A_\sigma=\int_X\rho(f(z))^2s_1(z)^2\,dx\,dy
\leq K\int_X\rho(f(z))^2J_f(z)\,dx\,dy
=KA_\rho.
$$

Also $s_1^2\geq J_f$, so $A_\sigma\geq A_\rho>0$. Thus $\sigma$ has positive finite area and is admissible, and

$$
\frac{L_\rho(f(\Gamma))^2}{A_\rho}
\leq K\,\frac{L_\sigma(\Gamma)^2}{A_\sigma}
\leq K\,\lambda(\Gamma,X).
$$

Taking the [supremum](../../../../../../supremum.md) over $\rho$ proves

$$
\boxed{\lambda(f(\Gamma),Y)\leq K\lambda(\Gamma,X).}
$$

Applying the same argument to $f^{-1}$, which has the same bound on its [maximal dilatation](../../../../../../maximal-dilatation.md), also gives $K^{-1}\lambda(\Gamma,X)\leq\lambda(f(\Gamma),Y)$. The inequalities remain valid for extended [extremal lengths](../../../../../../extremal-length.md); no extremizing density need exist.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
