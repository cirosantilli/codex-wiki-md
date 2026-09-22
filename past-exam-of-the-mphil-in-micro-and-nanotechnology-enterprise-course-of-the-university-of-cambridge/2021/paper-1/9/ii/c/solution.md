<h1 id="9/ii/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taking room [temperature](../../../../../../temperature-split.md) as $300\,\mathrm K$, the [thermal voltage](../../../../../../thermal-voltage.md) is $V_T=k_BT/q=0.025852\,\mathrm V$. For the stated [ideal diode](../../../../../../ideal-diode-model.md), $n=1$, so

$$
J=10^{-12}\left[\exp\!\left(\frac{0.75}{0.025852}\right)-1\right]
=\boxed{3.98\,\mathrm{A\,cm^{-2}}}.
$$

The $-1$ term is negligible here. A different precise interpretation of room [temperature](../../../../../../temperature-split.md) changes the result noticeably because of the exponential; the calculation above states its [temperature](../../../../../../temperature-split.md) explicitly.

For a lower-bandgap material, the [intrinsic carrier concentration](../../../../../../intrinsic-carrier-concentration.md) generally rises, increasing the reverse saturation [current density](../../../../../../current-density.md), approximately through $J_0\propto n_i^2$ with $n_i^2\propto\exp(-E_g/k_BT)$ when other parameters are held comparable. Thus **the forward [electric current](../../../../../../electric-current.md) at the same [voltage](../../../../../../voltage.md) would normally increase**. If $J_0$ were artificially held fixed at the supplied numerical value, however, the ideal-diode equation would give the same [electric current](../../../../../../electric-current.md): the [band gap](../../../../../../band-gap.md) dependence enters through the material parameters rather than as a separate term in that equation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [Ii](../../ii.md)
3. [9](../../../9.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
