<h1 id="6a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate the map:

$$
g'(x)=r+ke^{-\lambda x}(1-\lambda x).
$$

At the positive equilibrium, $ke^{-\lambda x_*}=1-r$, so

$$
g'(x_*)
=1-(1-r)\lambda x_*
=1-(1-r)\log\left(\frac{k}{1-r}\right).
$$

The [fixed point stability for an iteration](../../../../../../fixed-point-stability-for-an-iteration.md) requires $|g'(x_*)|<1$. Existence already makes the logarithm positive, so the upper inequality is automatic. The lower inequality gives

$$
(1-r)\log\left(\frac{k}{1-r}\right)<2.
$$

Combining it with existence yields the [stability interval of the survival-augmented Ricker equilibrium](../../../../../../stability-interval-of-the-survival-augmented-ricker-equilibrium.md):

$$
\boxed{1-r<k<(1-r)\exp\left(\frac2{1-r}\right)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6A](../../6a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
