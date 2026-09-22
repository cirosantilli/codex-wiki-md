<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the [homologous spherical flow](../../../../../../homologous-spherical-flow.md) $\mathbf u=q\mathbf r$, the [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) and $\nabla\mathbin\cdot\mathbf B=0$ give the [material derivative](../../../../../../material-derivative.md)

$$
\frac{D\mathbf B}{Dt}
=(\mathbf B\mathbin\cdot\nabla)\mathbf u
-\mathbf B\nabla\mathbin\cdot\mathbf u
=-2q\mathbf B.
$$

Let $x=r/R(t)$ and use the [self-similar ansatz](../../../../../../self-similar-ansatz.md)

$$
B_r=B_0f(x)\cos\theta,
\qquad
B_\theta=-B_0g(x)\sin\theta.
$$

Part (b) gives $q=3\dot R/(4R)$, and therefore

$$
\frac{Dx}{Dt}=x\left(q-\frac{\dot R}{R}\right)
=-\frac14\frac{\dot R}{R}x.
$$

The radial induction equation becomes $xf'=6f$. The boundary value $f(1)=1$ gives $f=x^6$. The [solenoidal vector field](../../../../../../solenoidal-vector-field.md) condition requires

$$
g=f+\frac x2f'=4x^6,
$$

which also matches the tangential shock value in part (c). Hence the interior field is

$$
\boxed{B_r=B_0\left(\frac rR\right)^6\cos\theta,
\qquad
B_\theta=-4B_0\left(\frac rR\right)^6\sin\theta,
\qquad B_\phi=0}.
$$

Outside the shock, the uniform-field lines obey $r\sin\theta=\text{constant}$. Inside, the [magnetic-field-line equation](../../../../../../magnetic-field-line-equation.md) gives

$$
\frac{dr}{r\,d\theta}=\frac{B_r}{B_\theta}
=-\frac14\cot\theta,
$$

so

$$
\boxed{r^4\sin\theta=\text{constant}}.
$$

A sketch therefore shows straight exterior lines refracting at the spherical shock into north-south symmetric curves that bow toward the equatorial interior before leaving through the opposite hemisphere. The field strength falls as $r^6$ toward the centre.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
