<h1 id="11b/solution">Solution</h1>

↑ **Parent:** [11B](../11b.md)

Using the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) and the [epsilon-delta identity](../../../../../contraction-of-two-levi-civita-symbols.md),

$$
[\nabla\times(\nabla\times A)]_i
=\epsilon_{ijk}\epsilon_{klm}\partial_j\partial_lA_m
=\partial_i(\partial_jA_j)-\partial_j\partial_jA_i.
$$

Therefore

$$
\boxed{\nabla\times(\nabla\times A)=\nabla(\nabla\mathbin\cdot A)-\nabla^2A}.
$$

One particularly simple [vector potential](../../../../../vector-potential.md) for $u$ is

$$
\boxed{A=\frac13(z^3,x^3,y^3)}.
$$

Direct differentiation gives $\nabla\mathbin\cdot A=0$ and $\nabla\times A=(y^2,z^2,x^2)=u$.

Parametrize the curved cone by

$$
R(z,\varphi)=(z\tan\alpha\cos\varphi,
z\tan\alpha\sin\varphi,z).
$$

The outward [oriented surface element](../../../../../oriented-surface-element.md) is

$$
d\mathbf S=(R_\varphi\times R_z)\,d\varphi\,dz
=z(\tan\alpha\cos\varphi,\tan\alpha\sin\varphi,-\tan^2\alpha)\,d\varphi\,dz.
$$

Substitution and integration over $0\leq z\leq h$, $0\leq\varphi<2\pi$ give

$$
\boxed{\int_{S_1}u\mathbin\cdot d\mathbf S
=-\frac{\pi h^4\tan^4\alpha}{4}}.
$$

Because $\nabla\mathbin\cdot u=0$, the [divergence theorem](../../../../../divergence-theorem.md) predicts that the two outward fluxes sum to zero. On the top disk $S_2$, $d\mathbf S=(0,0,1)\,dx\,dy$ and $u_z=x^2$, so, with $R=h\tan\alpha$,

$$
\int_{S_2}u\mathbin\cdot d\mathbf S
=\int_{x^2+y^2\leq R^2}x^2\,dx\,dy
=\boxed{\frac{\pi R^4}{4}}
=\frac{\pi h^4\tan^4\alpha}{4},
$$

as predicted.

The outward orientation on $S_2$ induces the stated anticlockwise orientation on $C$, whereas the outward orientation on $S_1$ induces the reverse orientation. Since $u=\nabla\times A$, [Stokes theorem](../../../../../stokes-theorem.md) predicts

$$
\int_{S_2}u\mathbin\cdot d\mathbf S=\oint_CA\mathbin\cdot d\mathbf l,
\qquad
\int_{S_1}u\mathbin\cdot d\mathbf S=-\oint_CA\mathbin\cdot d\mathbf l.
$$

On $C$, put $(x,y,z)=(R\cos\varphi,R\sin\varphi,h)$. Then

$$
\oint_CA\mathbin\cdot d\mathbf l
=\frac13\int_0^{2\pi}
\left[-h^3R\sin\varphi+R^4\cos^4\varphi\right]d\varphi
=\boxed{\frac{\pi R^4}{4}},
$$

verifying both identities.

## ↑ Ancestors (10)

1. [11B](../11b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
