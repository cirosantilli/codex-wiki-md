<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For Keplerian angular velocity, $R^2(d\Omega/dR)^2=9GM/(4R^3)$. The stated $F_{\rm diss}$ is the dissipation summed over both disk faces, so $F_{\rm diss}=2\sigma_{\rm SB}T_{\rm eff}^4$. Inside $R_0$ this gives

$$
\boxed{T_{\rm eff}^4(R)=\frac{3GM\dot m_0}{8\pi\sigma_{\rm SB}R^3}
\left[1-\left(\frac{R_{\rm ISCO}}R\right)^{1/2}\right].}
$$

Differentiating the factor $R^{-3}[1-(R_{\rm ISCO}/R)^{1/2}]$ shows that the maximum occurs at

$$
\boxed{R_{T,\max}=\frac{49}{36}R_{\rm ISCO}}
$$

when this radius lies below $R_0$. In the ordinary inflowing region far from its inner edge, $T_{\rm eff}\propto R^{-3/4}$.

For the static angular-momentum sink outside $R_0$, part c instead gives

$$
\boxed{T_{\rm eff}^4(R)=\frac{3GM\dot m_0}{8\pi\sigma_{\rm SB}R^3}
\left[\left(\frac{R_0}R\right)^{1/2}
-\left(\frac{R_{\rm ISCO}}R\right)^{1/2}\right],}
$$

so the genuinely large-radius behavior of the complete injected disk is $T_{\rm eff}\propto R^{-7/8}$.

Integrating $2\pi R F_{\rm diss}\,dR$ over both regions gives

$$
L_{<R_0}=GM\dot m_0\left[
\frac1{2R_{\rm ISCO}}-\frac3{2R_0}
+\frac{\sqrt{R_{\rm ISCO}}}{R_0^{3/2}}\right]
$$

and

$$
L_{>R_0}=\frac{GM\dot m_0}{R_0}
\left[1-\left(\frac{R_{\rm ISCO}}{R_0}\right)^{1/2}\right].
$$

Hence

$$
\boxed{L_{\rm disk}=\frac{GM\dot m_0}{2}
\left(\frac1{R_{\rm ISCO}}-\frac1{R_0}\right),}
$$

which is exactly the loss of Keplerian orbital energy as matter moves from its injection orbit to the inner edge.

For a standard disk extending through a radius $R\gg R_{\rm ISCO}$,

$$
L(>R)=\frac{3GM\dot m}{2R}
\left[1-\frac23\left(\frac{R_{\rm ISCO}}R\right)^{1/2}\right]
\simeq\frac{3GM\dot m}{2R}.
$$

This is three times the binding-energy release $GM\dot m/(2R)$ available outside $R$. The excess is energy carried outward by the [viscous torque in an accretion disk](../../../../../../viscous-torque-in-an-accretion-disk.md) and dissipated at larger radii. In the injected model the nonaccreting outer disk is an especially direct example: it radiates despite having zero mean radial mass flux because it absorbs the angular momentum and mechanical work exported by the inner disk.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
