<h1 id="35c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
x=\beta\mu B.
$$

The one-spin partition function is

$$
z_1=e^{-x}+1+e^x=1+2\cosh x.
$$

The spins are independent, so the [spin-1 paramagnet](../../../../../../spin-1-paramagnet.md) has

$$
Z=z_1^N
$$

and free energy

$$
\boxed{
F=-\frac N\beta\log(1+2\cosh(\beta\mu B))}.
$$

The canonical heat capacity can be obtained from the energy variance:

$$
C=k_B\beta^2\frac{\partial^2}{\partial\beta^2}\log Z.
$$

Because

$$
\frac{d^2}{dx^2}\log(1+2\cosh x)
=\frac{2(\cosh x+2)}{(1+2\cosh x)^2},
$$

we obtain

$$
\boxed{
C=Nk_B(\beta\mu B)^2
\frac{2(\cosh(\beta\mu B)+2)}
{(1+2\cosh(\beta\mu B))^2}}.
$$

At high temperature, $x\to0$, and hence

$$
\boxed{-\beta F\longrightarrow N\log3},
\qquad
\boxed{C\sim\frac23Nk_B(\beta\mu B)^2\longrightarrow0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [35C](../../35c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
