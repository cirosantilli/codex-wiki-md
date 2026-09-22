<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An optically thick annulus radiates as a [blackbody](../../../../../../blackbody.md) from both faces, so

$$
2\sigma_{\rm SB}T_{\rm BB}^4=F_{\rm diss}.
$$

For a steady [Keplerian accretion disk](../../../../../../keplerian-accretion-disk.md) with a [zero-torque inner boundary condition](../../../../../../zero-torque-inner-boundary-condition.md),

$$
\nu\Sigma=\frac{\dot M}{3\pi}
\left[1-\left(\frac{R_{\rm in}}R\right)^{1/2}\right],
\qquad
R^2\left(\frac{d\Omega}{dR}\right)^2=\frac94\Omega_K^2.
$$

Consequently

$$
F_{\rm diss}=\frac{3GM\dot M}{4\pi R^3}
\left[1-\left(\frac{R_{\rm in}}R\right)^{1/2}\right]
$$

and

$$
\boxed{T_{\rm BB}(R)=
\left\{\frac{3GM\dot M}{8\pi\sigma_{\rm SB}R^3}
\left[1-\left(\frac{R_{\rm in}}R\right)^{1/2}\right]\right\}^{1/4}.}
$$

Away from the inner edge, $T\propto R^{-3/4}$.

Ignoring inclination and distance factors, the [multitemperature blackbody disk](../../../../../../multitemperature-blackbody-disk.md) spectrum is

$$
S_{\bar\nu}\propto\int_{R_{\rm in}}^{R_{\rm out}}
2\pi R B_{\bar\nu}[T(R)]\,dR.
$$

Set $x=h\bar\nu/(k_BT)$. Since $T\propto R^{-3/4}$, $R\,dR\propto\bar\nu^{-8/3}x^{5/3}dx$, whereas the [Planck function](../../../../../../planck-function.md) contributes $\bar\nu^3/(e^x-1)$. In the stated intermediate-frequency range the radial endpoints become $0$ and $\infty$, leaving a frequency-independent convergent integral. Therefore

$$
\boxed{S_{\bar\nu}\propto\bar\nu^{1/3}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
