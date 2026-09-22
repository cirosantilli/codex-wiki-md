<h1 id="15f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write derivatives with respect to $u$. The arc-length condition is $f'^2+g'^2=1$. The tangent vectors are

$$
\sigma_u=(f'\cos v,f'\sin v,g'),\qquad \sigma_v=(-f\sin v,f\cos v,0).
$$

Their scalar products give the [first fundamental form](../../../../../../first-fundamental-form.md)

$$
\boxed{I=du^2+f^2dv^2.}
$$

Choose the unit [normal vector](../../../../../../normal-vector.md) $N=(-g'\cos v,-g'\sin v,f')$, since $\sigma_u\times\sigma_v=fN$ and $f>0$. Scalar products of $N$ with the second [partial derivatives](../../../../../../partial-derivative.md) give

$$
\boxed{II=(f'g''-g'f'')\,du^2+fg'\,dv^2.}
$$

The mixed coefficient is zero. Reversing $N$ reverses the [second fundamental form](../../../../../../second-fundamental-form-split.md) but not the [Gaussian curvature](../../../../../../gaussian-curvature.md). Its formula is

$$
K=\frac{(f'g''-g'f'')fg'}{f^2}=\frac{f'g'g''-g'^2f''}{f}.
$$

Differentiating the arc-length identity gives $f'f''+g'g''=0$. Substitute it directly, without dividing by $g'$ (which may vanish), to obtain

$$
\boxed{K=-\frac{f''}{f}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15F](../../15f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
