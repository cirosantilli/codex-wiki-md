<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The reference to part (f) within this part is a printed self-reference; the needed product estimate is part (e). Since both masses are one, subtracting the [Bobylev identities](../../../../../../bobylev-identity.md) gives, for $\xi\ne0$,

$$
\partial_t\frac{\widehat f(\xi)-\widehat g(\xi)}{|\xi|^2}
+\frac{\widehat f(\xi)-\widehat g(\xi)}{|\xi|^2}
=\frac1{|\mathbb S^2|}\int_{\mathbb S^2}
\frac{\widehat f(\xi^+)\widehat f(\xi^-)-\widehat g(\xi^+)\widehat g(\xi^-)}{|\xi|^2}\,d\sigma.
$$

The normalized angular average and part (e) give

$$
\boxed{\left|\partial_t\frac{\widehat f-\widehat g}{|\xi|^2}+\frac{\widehat f-\widehat g}{|\xi|^2}\right|\leq d(f,g)}.
$$

For completeness, the [Duhamel principle](../../../../../../duhamel-s-principle.md) for this scalar equation yields $d(t)\leq e^{-t}d(0)+\int_0^te^{-(t-s)}d(s)\,ds$. Apply the [Gronwall inequality](../../../../../../gronwall-inequality.md) to $e^td(t)$ to obtain the [Fourier nonexpansion for Maxwell molecules](../../../../../../fourier-nonexpansion-for-maxwell-molecules.md), $\boxed{d(f_t,g_t)\leq d(f_0,g_0)}$. This estimate is nonexpansion; by itself it does not prove strict decay or convergence to a specified equilibrium.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [4](../../4.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
