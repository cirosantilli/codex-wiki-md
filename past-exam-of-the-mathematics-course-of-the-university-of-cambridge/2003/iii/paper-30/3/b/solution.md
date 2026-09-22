<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work [edge](../../../../../../edge-of-a-graph.md) by [edge](../../../../../../edge-of-a-graph.md). Let $\omega,\eta$ have two-bit restrictions to an [edge](../../../../../../edge-of-a-graph.md). If these restrictions are comparable, taking their [meet in a lattice](../../../../../../meet-in-a-lattice.md) and [join in a lattice](../../../../../../join-in-a-lattice.md) only reorders the two pairs, so their total equality indicators do not change. If they are incomparable, they are $01$ and $10$, while their [meet in a lattice](../../../../../../meet-in-a-lattice.md) and [join in a lattice](../../../../../../join-in-a-lattice.md) are $00$ and $11$. In that case the sum of equality indicators increases from zero to two. Consequently

$$
\Delta_e=\delta_{(\omega\vee\eta)(x),(\omega\vee\eta)(y)}
+\delta_{(\omega\wedge\eta)(x),(\omega\wedge\eta)(y)}
-\delta_{\omega(x),\omega(y)}-\delta_{\eta(x),\eta(y)}\ge0.
$$

The [partition functions](../../../../../../canonical-partition-function.md) cancel from the required ratio, leaving

$$
\frac{\mu_\Lambda(\omega\vee\eta)\mu_\Lambda(\omega\wedge\eta)}
{\mu_\Lambda(\omega)\mu_\Lambda(\eta)}
=\exp\left(\beta\sum_e\Delta_e\right)\ge1.
$$

This is the [ferromagnetic Ising lattice inequality](../../../../../../ferromagnetic-ising-lattice-inequality.md) in binary-spin normalization, so **the measure satisfies the [FKG lattice condition](../../../../../../fkg-lattice-condition.md) and is [positively associated](../../../../../../positive-association-of-random-variables.md)**. If $\sigma(x)=2\omega(x)-1$, then $\delta_{\omega(x),\omega(y)}=(1+\sigma(x)\sigma(y))/2$: the conventional $\{-1,1\}$ coupling is $\beta/2$, which explains the factor two in the [edge](../../../../../../edge-of-a-graph.md) calculation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
