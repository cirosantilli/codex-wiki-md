<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [finite-thickness disk relaxation](../../../../../../finite-thickness-disk-relaxation.md), assume a well-separated range $b_{\min}\ll z_0\ll R$ and approximately virialized self-gravity. The three factors have distinct origins. Replacing the characteristic encounter [speed](../../../../../../speed.md) by $u=\lambda v$ shortens the diffusion [time](../../../../../../time-in-physics.md) by $\lambda^3$: the variance-production rate has one inverse power of [speed](../../../../../../speed.md), and the target random [velocity](../../../../../../velocity.md) squared has two powers. Concentrating the same number of [stars](../../../../../../star.md) into [volume](../../../../../../volume.md) of order $R^2z_0$, rather than $R^3$, raises the number [volume](../../../../../../volume.md) density by $R/z_0$ and shortens the [time](../../../../../../time-in-physics.md) by $z_0/R$. Finally, only separations below the thickness sample a three-dimensional encounter geometry. The logarithmic upper cutoff becomes $z_0$, and therefore the inverse-logarithm [time](../../../../../../time-in-physics.md) acquires $\log(R/b_{\min})/\log(z_0/b_{\min})$. More distant encounters have the planar geometry and provide a convergent, non-logarithmic correction. A smaller [Coulomb logarithm in stellar dynamics](../../../../../../coulomb-logarithm-in-stellar-dynamics.md) actually partly offsets the first two shortenings.

Thus, using the same cutoff for this comparison,

$$
\boxed{\frac{t_{\rm disk}}{t_{\rm sphere}}\sim\lambda^3\frac{z_0}{R}\frac{\log(R/b_{\min})}{\log(z_0/b_{\min})}.}
$$

For actual point particles the disk cutoff is $Gm/(\lambda v)^2$, whereas the spherical one is $Gm/v^2$; one must use the appropriate cutoff in each logarithm rather than silently identifying them. For a softened calculation it is instead of order the larger of the weak-deflection scale and the softening length. The formula is not valid when $z_0$ approaches that cutoff.

Write $h=z_0/R$ and $q=K/\varepsilon$, with simulation duration $K t_{\rm dyn}$ and allowed fractional diffusion $\varepsilon$. Combining the paper's spherical normalization and its comparison formula gives the leading criterion

$$
\boxed{\frac{\lambda^3hN}{8\log(z_0/b_{\min})}\gtrsim q.}
$$

The spherical comparison logarithm cancels when its numerical convention and a common comparison cutoff are used; order-one shape factors remain approximate. In an unsoftened disk with $v^2\sim GNm/R$, $z_0/b_{\min}\sim h\lambda^2N$. Hence the implicit requirement is $N/\log(h\lambda^2N)\gtrsim8q/(\lambda^3h)$, in the regime $h\lambda^2N\gg1$. For $\lambda=h=0.1$, the [stellar relaxation time](../../../../../../stellar-relaxation-time.md) is of order $10^{-4}$ of the spherical value apart from logarithms; $N\sim10^8$ gives a [time](../../../../../../time-in-physics.md) of order 100 crossing times in this estimate. Negligible relaxation over that duration requires an additional margin. **A disk generally needs far more particles than a round [galaxy](../../../../../../galaxy-split.md) for the same relaxation tolerance; no universal minimum follows without duration, thickness and softening.** Collective spiral or bending responses are a separate source of evolution even in a [collisionless stellar system](../../../../../../collisionless-stellar-system.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
