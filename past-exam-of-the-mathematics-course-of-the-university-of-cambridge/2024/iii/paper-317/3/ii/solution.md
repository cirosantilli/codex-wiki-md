<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the [ideal gas](../../../../../../ideal-gas.md) law as $P=\mathcal R\rho T/\mu$. Since $P=g\Sigma$,

$$
\rho=B\frac{\Sigma}{T},
\qquad
B=\frac{\mu g}{\mathcal R}.
$$

The prescribed opacity and burning laws become

$$
\kappa=\kappa_0B\Sigma T^{-3},
\qquad
\epsilon=\epsilon_0B\Sigma T^{14}.
$$

The radiative equation is consequently

$$
\frac{dT}{d\Sigma}=K\Sigma F T^{-6},
\qquad
K=\frac{3\kappa_0B}{4ac}.
$$

With $y=T^7$ and $x=\Sigma^2/2$,

$$
\frac{dy}{dx}=7KF\equiv AF.
$$

The energy equation similarly gives

$$
\frac{dF}{dx}=-\epsilon_0B y^2.
$$

Differentiating the first relation therefore produces the [nonlinear ordinary differential equation](../../../../../../nonlinear-ordinary-differential-equation.md)

$$
\boxed{\frac{d^2y}{dx^2}=-\omega^2y^2},
\qquad
\boxed{\omega^2=A\epsilon_0B\gt0}.
$$

At the idealized zero-temperature surface, $x=0$ and $y=0$. The outward flux there is $F_s=L/(4\pi R^2)$, so

$$
\boxed{y(0)=0,
\qquad
y'(0)=\frac{AL}{4\pi R^2}}.
$$

At the base, $x_0=\Sigma_0^2/2$ and $y=T_0^7$. The core supplies no luminosity in this model, so all flux has been generated in the overlying hydrogen envelope and $F(x_0)=0$. Hence

$$
\boxed{y(x_0)=T_0^7,
\qquad
y'(x_0)=0}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
