<h1 id="24i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an [affine variety](../../../../../../affine-algebraic-set.md) $X\subseteq\mathbb A_k^n$ with [vanishing ideal](../../../../../../vanishing-ideal.md) $I(X)$, its [Zariski tangent space](../../../../../../zariski-tangent-space.md) at $p$ is

$$
T_pX=\left\{v\in k^n:
\sum_{i=1}^n\frac{\partial h}{\partial x_i}(p)v_i=0
\text{ for every }h\in I(X)\right\}.
$$

The [dimension from minimum tangent dimension](../../../../../../dimension-from-minimum-tangent-dimension.md) is

$$
\dim X=\min_{p\in X}\dim_kT_pX.
$$

Now let $X=Z(f)$ with $f$ irreducible. The [Strong Hilbert Nullstellensatz](../../../../../../strong-hilbert-nullstellensatz.md) gives $I(X)=(f)$, so

$$
T_pX=\ker\left(v\mapsto\nabla f(p)\mathbin\cdot v\right).
$$

Its dimension is at least $n-1$, and it is exactly $n-1$ wherever $\nabla f(p)\ne0$.

It remains to find such a point in positive characteristic $q$. If every partial derivative of $f$ were the zero polynomial, every exponent occurring in $f$ would be divisible by $q$. Since the algebraically closed field $k$ is [perfect](../../../../../../perfect-field.md), all coefficients have $q$th roots and $f$ would be a $q$th power, contradicting irreducibility. Thus some partial derivative $f_{x_i}$ is nonzero. If the gradient nevertheless vanished at every point of $Z(f)$, the Nullstellensatz would imply $f_{x_i}\in(f)$. This is impossible because $0\leq\deg f_{x_i}<\deg f$. The [smooth point on an irreducible hypersurface in positive characteristic](../../../../../../smooth-point-on-an-irreducible-hypersurface-in-positive-characteristic.md) therefore exists, and

$$
\boxed{\dim Z(f)=n-1.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [24I](../../24i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
