<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At a fixed height, first determine the stored quantities per unit vertical height and per unit length along the line source. With $\Delta\rho=\rho-\rho_0$, the [triangular-profile line plume](../../../../../../triangular-profile-line-plume.md) has the useful profile integral

$$
I_n=\int_{-b}^bf(x/b)^n\,dx=\frac{2b}{n+1},\qquad n\ge0.
$$

The geometric [volume](../../../../../../volume.md) is $\mathcal A=2b$; the [mass](../../../../../../mass.md) is $\mathcal D=\rho_0I_0+\Delta\rho I_1=b(\rho+\rho_0)$. The upward [momentum](../../../../../../momentum.md) is $\mathcal P=W(\rho_0I_1+\Delta\rho I_2)$, while the buoyancy force is $\mathcal B=-g\Delta\rho I_1$. Thus

$$
\boxed{\mathcal A=2b,\quad \mathcal D=b(\rho+\rho_0),\quad
\mathcal P=\frac{bW}{3}(\rho_0+2\rho),\quad \mathcal B=gb(\rho_0-\rho).}
$$

Here positive [buoyancy](../../../../../../buoyancy.md) corresponds to a rising light plume. If instead buoyancy is defined kinematically, divide $\mathcal B$ by $\rho_0$; the density-weighted convention here is the one matching the printed equations.

Multiply each local density by the vertical [velocity](../../../../../../velocity.md) to obtain the fluxes through a horizontal section, still per unit source length:

$$
\boxed{\begin{aligned}
V&=\int\widehat w\,dx=bW,\\
Q&=\int\widehat\rho\,\widehat w\,dx=\frac{bW}{3}(\rho_0+2\rho),\\
M&=\int\widehat\rho\,\widehat w^2\,dx=\frac{bW^2}{6}(\rho_0+3\rho),\\
F&=\int g(\rho_0-\widehat\rho)\widehat w\,dx=\frac23gbW(\rho_0-\rho).
\end{aligned}}
$$

In particular, the stored [momentum](../../../../../../momentum.md) equals the [mass flux](../../../../../../mass-flux.md) $Q$, and the [buoyancy flux](../../../../../../buoyancy-flux.md) is $F=g(\rho_0V-Q)$. The different triangular-profile factors in storage and flux must not be replaced by top-hat coefficients.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
