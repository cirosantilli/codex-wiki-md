<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Treat $n^2=N^2/\Omega^2$ as a signed small parameter, with $|n^2|\ll1$, as printed in the original PDF. At $n^2=0$, the [dispersion relation](../../../../../../dispersion-relation.md) factors as

$$
(s+\beta)(s^2+\Omega^2)=0.
$$

Thus the two [epicyclic motion](../../../../../../epicyclic-motion.md) modes have $s_0=\pm i\Omega$, while the [thermal energy mode of a shearing sheet](../../../../../../thermal-energy-mode-of-a-shearing-sheet.md) has

$$
\boxed{s_{E,0}=-\beta=-\xi k^2.}
$$

It decays on the [thermal diffusion time](../../../../../../thermal-diffusion-time.md) $\beta^{-1}$. For completeness, its next correction is $s_E=-\beta+\beta N^2/(\beta^2+\Omega^2)+O(\Omega n^4)$ at fixed $\beta/\Omega$.

For either [epicyclic motion](../../../../../../epicyclic-motion.md) root, the [implicit function theorem](../../../../../../implicit-function-theorem.md) applied to the [dispersion relation](../../../../../../dispersion-relation.md) gives

$$
2s_0(s_0+\beta)s_1+\Omega^2s_0=0,\qquad
\boxed{s_1=-\frac{\Omega^2}{2(\beta+s_0)}.}
$$

Hence

$$
s_\pm=\pm i\Omega-\frac{N^2}{2(\beta\pm i\Omega)}+O(\Omega n^4),\qquad
\operatorname{Re}s_\pm=-\frac{N^2\beta}{2(\beta^2+\Omega^2)}+O(\Omega n^4).
$$

Since $\beta>0$, the oscillations undergo [overstability](../../../../../../overstability.md) precisely when

$$
\boxed{N^2<0.}
$$

The [convective overstability growth rate](../../../../../../convective-overstability-growth-rate.md) tends to zero both for very slow diffusion and for very fast diffusion. Differentiating $\beta/(\beta^2+\Omega^2)$ shows that its maximum occurs at $\beta=\Omega$, corresponding to $k^2=\Omega/\xi$. Therefore

$$
\boxed{\operatorname{Re}s_{\rm max}=-\frac{N^2}{4\Omega}+O(\Omega n^4),\qquad\xi k_{\rm max}^2=\Omega.}
$$

This is the growth rate of the perturbation amplitude; a quadratic perturbation energy grows at twice that rate. The [convective overstability](../../../../../../convective-overstability.md) arises when an adverse radial [specific entropy](../../../../../../specific-entropy.md) gradient couples to [epicyclic motion](../../../../../../epicyclic-motion.md) with a finite [thermal conduction](../../../../../../thermal-conduction.md) lag.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
