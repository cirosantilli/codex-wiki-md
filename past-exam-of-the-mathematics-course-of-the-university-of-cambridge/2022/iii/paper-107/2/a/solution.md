<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Freeze the lower-order coefficients on a ball and apply the interior [Schauder estimate](../../../../../../schauder-estimates.md) for the [Poisson equation](../../../../../../poisson-equation.md) to a cutoff of $u$. The terms $b_iD_i u+cu$ are controlled by the [Hölder interpolation inequality](../../../../../../holder-interpolation-inequality.md)

$$
[Du]_{\alpha;B_r}+|u|_{\alpha;B_r}
\leq\eta[D^2u]_{\alpha;B}+C_\eta|u|_{2;B}.
$$

Choosing $\eta$ in terms of the prescribed $\delta$ yields

$$
\boxed{[D^2u]_{\alpha;B_{1/2}}
\leq\delta[D^2u]_{\alpha;B}+C(n,\alpha,\beta,\delta)|u|_{2;B}.}
$$

The standard iteration lemma for nested balls absorbs the first term. The remaining $C^2$ norm is bounded by the interior derivative estimate and interpolation, producing

$$
\boxed{|u|_{2,\alpha;B_{1/2}}
\leq C(n,\alpha,\beta)|u|_{0;B}.}
$$

Equivalently, a contradiction-and-rescaling proof would produce a globally Hölder harmonic limit forbidden by the [polynomial-growth Liouville theorem for harmonic functions](../../../../../../polynomial-growth-liouville-theorem-for-harmonic-functions.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
