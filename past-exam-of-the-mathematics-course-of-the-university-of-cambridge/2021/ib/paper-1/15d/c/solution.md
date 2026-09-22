<h1 id="15d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Substituting the wire potential from part (b) into the flux formula from part (a) gives [Neumann's mutual-inductance formula](../../../../../../neumann-s-mutual-inductance-formula.md)

$$
L_{12}
=\frac{\Phi_{12}}{I_2}
=\frac{\mu_0}{4\pi}
\oint_{C_1}\oint_{C_2}
\frac{dx_1\mathbin{\cdot}dx_2}{|x_1-x_2|}.
$$

Interchanging the two curves proves $L_{12}=L_{21}$.

Parametrize the coaxial circles by

$$
x_1=(a\cos\phi,a\sin\phi,0),
\qquad
x_2=(b\cos\psi,b\sin\psi,c).
$$

Then, with $\theta=\phi-\psi$ and $R=\sqrt{a^2+b^2+c^2}$,

$$
dx_1\mathbin{\cdot}dx_2
=ab\cos\theta\,d\phi\,d\psi,
\qquad
|x_1-x_2|=R\sqrt{1-q\cos\theta},
$$

where $q=2ab/R^2$. One angular integration contributes $2\pi$, so

$$
L_{12}
=\frac{\mu_0ab}{2R}
\int_0^{2\pi}\frac{\cos\theta\,d\theta}
{\sqrt{1-q\cos\theta}}.
$$

Since $ab=qR^2/2$, this is

$$
\boxed{
L_{12}=\frac{\mu_0R}{4}f(q)
=\frac{\mu_0}{4}\sqrt{a^2+b^2+c^2}\,f(q)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15D](../../15d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
