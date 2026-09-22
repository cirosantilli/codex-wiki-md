<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Suppress the mode label temporarily and let $a,b$ be out-operators. With $q=v/u$, the commuting-mode identity

$$
a\,e^{-qa^\dagger b^\dagger}
=e^{-qa^\dagger b^\dagger}(a-qb^\dagger)
$$

shows that $(a+qb^\dagger)e^{-qa^\dagger b^\dagger}|0_{\rm out}\rangle=0$. The analogous relation for $b$ gives the [antiparticle](../../../../../antiparticle.md) condition. Thus in a finite regulated collection of modes,

$$
\boxed{|0_{\rm in}\rangle
=\mathcal N\prod_{\mathbf k}
\exp\!\left[-\frac{v_{\mathbf k}}{u_{\mathbf k}}
a_{\mathbf k}^{{\rm out}\dagger}
b_{-\mathbf k}^{{\rm out}\dagger}\right]
|0_{\rm out}\rangle.}
$$

For one particle-antiparticle mode pair, $(a^\dagger b^\dagger)^n|0,0\rangle=n!|n,n\rangle$. The exponential's factorial therefore cancels:

$$
|0_{\rm in}\rangle_{\mathbf k}
=\sqrt{1-|q_{\mathbf k}|^2}
\sum_{n=0}^{\infty}(-q_{\mathbf k})^n|n,n\rangle_{\rm out}.
$$

The resulting [particle-antiparticle two-mode squeezed vacuum](../../../../../particle-antiparticle-two-mode-squeezed-vacuum.md) has the [geometric pair-number distribution](../../../../../geometric-pair-number-distribution.md)

$$
\boxed{P_{\mathbf k}(n)
=(1-r_{\mathbf k})r_{\mathbf k}^{\,n},
\quad n=0,1,\ldots,\qquad
r_{\mathbf k}=\left|\frac{v_{\mathbf k}}{u_{\mathbf k}}\right|^2
=\left(\frac{\omega-\Omega}{\omega+\Omega}\right)^2.}
$$

Here one pair means one [particle](../../../../../particle-physics.md) in canonical mode $\mathbf k$ and one [antiparticle](../../../../../antiparticle.md) in mode $-\mathbf k$. They are distinct species, and the state has equal [particle](../../../../../particle-physics.md) and [antiparticle](../../../../../antiparticle.md) occupation. In particular,

$$
\langle n_{\mathbf k}\rangle
=\frac{r_{\mathbf k}}{1-r_{\mathbf k}}=|v_{\mathbf k}|^2,\qquad
\operatorname{var}n_{\mathbf k}
=|v_{\mathbf k}|^2(1+|v_{\mathbf k}|^2).
$$

For a finite set, $|\mathcal N|=\prod_{\mathbf k}\sqrt{1-r_{\mathbf k}}=\prod_{\mathbf k}|u_{\mathbf k}|^{-1}$. An overall [phase](../../../../../phase-waves.md) is arbitrary. With no pulse, $\Omega=\omega$, so $v=0$ and only the zero-pair state remains.

<a id="4/e/image-original-sudden-pulse-calculation-normalized-frequency-matching-coefficients-and-the-resulting-geometric-pair-number-distributions"></a>
![](../../../../../past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2016/paper-1-pair-creation.png)

**[Figure 4](#4/e/image-original-sudden-pulse-calculation-normalized-frequency-matching-coefficients-and-the-resulting-geometric-pair-number-distributions). Original sudden-pulse calculation: normalized frequency-matching coefficients and the resulting geometric pair-number distributions**.

The [ultraviolet divergence of an instantaneous vector-potential quench](../../../../../ultraviolet-divergence-of-an-instantaneous-vector-potential-quench.md) qualifies this formal product. For an exactly instantaneous vector-potential step in three spatial dimensions, at large $k$ the mixing behaves as $v_{\mathbf k}\sim e\mathbf A_0\cdot\widehat{\mathbf k}/(2\hbar k)$. Thus $\int\mathrm d^3k\,|v_{\mathbf k}|^2$ diverges in the ultraviolet. In a finite quantization box, a finite momentum cutoff makes the product a normalized Fock-space vector; a sufficiently smooth finite-duration pulse removes this particular instantaneous-quench pathology. The per-mode distribution remains the result above, while the unregulated infinite product should not be asserted to have a finite nonzero global normalization.

## ↑ Ancestors (15)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
