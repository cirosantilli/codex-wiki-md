<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a uniform distribution of phases along one period, average the ensemble [force](../../../../force-split.md) $BF_{\rm bound}$:

$$
\langle F\rangle=\frac{G_0}{P}\left[
\frac1{x_1}\int_0^{x_1}B(x)\,dx-
\frac1{P-x_1}\int_{x_1}^P B(x)\,dx\right].
$$

Using the negligible-carry-over form in [b](../b.md) gives

$$
\int_0^{x_1}B\,dx=B_0\left[x_1-\frac{1-e^{-\alpha x_1}}\alpha\right],\qquad
\int_{x_1}^PB\,dx=\frac{B_0(1-e^{-\alpha x_1})}{\beta}
\left[1-e^{-\beta(P-x_1)}\right].
$$

Consequently

$$
\boxed{\langle F\rangle\simeq\frac{G_0B_0}{P}\left[
1-\frac{1-e^{-\alpha x_1}}{\alpha x_1}
-\frac{1-e^{-\alpha x_1}}{\beta(P-x_1)}
\left(1-e^{-\beta(P-x_1)}\right)\right]},
$$

where $\boxed{B_0=k_1/(k_1+k_2),\ \alpha=(k_1+k_2)/v,\ \beta=k_2/v}$. This is the printed expression to the accuracy justified by the velocity condition.

It is not an exact identity for the periodic problem at arbitrary $v$. Keeping $b_{\rm in}$ instead gives

$$
\langle F\rangle_{\rm exact}=\frac{G_0B_0}{P}\left[
1-\frac{(1-a)(1-q)}{(1-aq)\alpha x_1}
-\frac{(1-a)(1-q)}{(1-aq)\beta(P-x_1)}\right].
$$

For a concrete counterexample outside the small-velocity approximation, choose $k_1=k_2=P=G_0=v=1$ and $x_1=1/2$. Then the exact periodic value is about $+0.01976$, whereas the printed reset expression is about $-0.06478$. The discrepancy is due to nonzero incoming occupancy, not an integration sign change.

As $v\to0^+$, both $\alpha$ and $\beta$ diverge, and both formulas give

$$
\boxed{\lim_{v\to0^+}\langle F\rangle=\frac{G_0}{P}\frac{k_1}{k_1+k_2}}.
$$

The bound population occupies the downhill binding region, while occupancy on the uphill region is confined to a vanishing boundary layer. A nonzero limiting stall [force](../../../../force-split.md) is compatible with zero mechanical power $v\langle F\rangle$. The spatially restricted binding and uniform unbinding do not obey local [detailed balance](../../../../detailed-balance.md) for this sawtooth [free energy](../../../../thermodynamic-free-energy.md): a passive equilibrium model would require $k_1(x)/k_2(x)$ to reflect the local energy difference and not vanish on an interval of finite energy. This is a driven or prescribed-kinetics motor model; the equilibrium relation in [a](../a.md) cannot be imposed on it without an energy supply and additional states.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
