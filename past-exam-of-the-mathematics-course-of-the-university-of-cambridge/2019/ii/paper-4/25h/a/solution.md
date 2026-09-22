<h1 id="25h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write

$$
q(v)=\sqrt{f'(v)^2+g'(v)^2}.
$$

The regularity of the profile makes $q>0$. The coordinate tangent vectors are

$$
\phi_u=(-f\sin u,f\cos u,0),
\qquad
\phi_v=(f'\cos u,f'\sin u,g'),
$$

so the [first fundamental form of a surface of revolution](../../../../../../first-fundamental-form-of-a-surface-of-revolution.md) has coefficients

$$
E=f^2,
\qquad F=0,
\qquad G=q^2.
$$

Choose the [unit normal](../../../../../../unit-normal.md)

$$
N=\frac1q(-g'\cos u,-g'\sin u,f').
$$

Taking scalar products with the second derivatives of $\phi$ gives the [second fundamental form](../../../../../../second-fundamental-form-split.md) coefficients

$$
e=\frac{fg'}q,
\qquad f_{\mathrm{II}}=0,
\qquad g_{\mathrm{II}}=\frac{f'g''-g'f''}q.
$$

Thus the coordinate directions are [principal directions](../../../../../../principal-direction.md), with [principal curvatures](../../../../../../principal-curvature.md)

$$
k_1=\frac{g'}{fq},
\qquad
k_2=\frac{f'g''-g'f''}{q^3}.
$$

The [curvatures of a parametrized surface of revolution](../../../../../../curvatures-of-a-parametrized-surface-of-revolution.md) are therefore

$$
\boxed{H=\frac12\left(\frac{g'}{fq}+\frac{f'g''-g'f''}{q^3}\right),
\qquad
K=\frac{g'(f'g''-g'f'')}{fq^4}.}
$$

Reversing the [orientation of a surface](../../../../../../orientation-of-a-surface.md) reverses the sign of $H$ but leaves $K$ unchanged.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [25H](../../25h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
