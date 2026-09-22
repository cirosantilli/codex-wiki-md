<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For one component with density $\rho_k=A_kr^{-2\beta_k}\Psi^{p_k}$, direct velocity integration, or the [Spherical Jeans equation](../../../../../../spherical-jeans-equation.md), gives

$$
P_{r,k}=\rho_k\sigma_{r,k}^2
=\frac{\rho_k\Psi}{p_k+1}.
$$

Each component has velocity-anisotropy parameter $\beta_k$. Therefore the combined coefficient is the radial-pressure-weighted mean

$$
\widehat\beta
=\frac{\beta_1P_{r,1}+\beta_2P_{r,2}}
{P_{r,1}+P_{r,2}}.
$$

Here

$$
q(r)=\frac{P_{r,2}}{P_{r,1}}
=\frac34\frac{\rho_2}{\rho_1}
=\frac{\sqrt{br}}{D(r)},
$$

so

$$
\boxed{
\widehat\beta(r)=
\frac{3+2q(r)}{4[1+q(r)]}}.
$$

Since $q\sim\sqrt{r/b}/2$ at the origin and $q\sim\sqrt{b/r}$ at infinity,

$$
\boxed{
\widehat\beta\longrightarrow\frac34
\quad\text{as }r\to0
\quad\text{and as }r\to\infty}.
$$

The second, less radial component reduces the anisotropy only at intermediate radii.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
