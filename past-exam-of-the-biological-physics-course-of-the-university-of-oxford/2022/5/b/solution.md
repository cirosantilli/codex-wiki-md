<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Each Cartesian component of one link has zero [mean](../../../../expected-value-split.md) and [variance](../../../../variance-split.md) $b^2/3$, with zero cross-component [covariance](../../../../covariance.md). By the multivariate [central limit theorem](../../../../central-limit-theorem.md), for large $N$ on the coil scale the vector [probability density](../../../../probability-density.md) is

$$
\boxed{p(\mathbf r)=\left(\frac{3}{2\pi Nb^2}\right)^{3/2}
\exp\left(-\frac{3r^2}{2Nb^2}\right)}.
$$

It is normalized with respect to $d^3r$; the radial [probability density](../../../../probability-density.md) is $4\pi r^2p(\mathbf r)$. The [Gaussian limit of the end-to-end distribution of a freely jointed chain](../../../../gaussian-limit-of-the-end-to-end-distribution-of-a-freely-jointed-chain.md) is an approximation, not the exact finite-$N$ law near $r=Nb$.

At prescribed vector separation the configurational [entropy](../../../../entropy-split.md) is $S(\mathbf r)=k_B\ln p(\mathbf r)+\text{constant}$. The [ideal chain](../../../../ideal-chain.md) has no extension-dependent internal energy, so its [Helmholtz free energy](../../../../helmholtz-free-energy.md) is

$$
A(\mathbf r)=A(0)+\frac{3k_BT r^2}{2Nb^2}.
$$

The externally required [force](../../../../force-split.md) is $\nabla_{\mathbf r}A$, while the chain's restoring [force](../../../../force-split.md) has the opposite sign. Thus

$$
\boxed{\mathbf f_{\rm restore}=-\frac{3k_BT}{Nb^2}\mathbf r,\qquad
k_{\rm spring}=\frac{3k_BT}{Nb^2},\qquad
\langle z\rangle=\frac{Nb^2}{3k_BT}f}.
$$

The last equation also follows by multiplying $p(\mathbf r)$ by the [Boltzmann factor](../../../../boltzmann-factor.md) $e^{fz/(k_BT)}$ and completing the square. This [entropic spring](../../../../entropic-spring.md) resists extension because fewer link configurations realize a stretched chain. At the same small applied [force](../../../../force-split.md), increasing [temperature](../../../../temperature-split.md) reduces extension; at the same extension it increases the required [force](../../../../force-split.md). Do not differentiate $-k_BT\ln[4\pi r^2p(\mathbf r)]$ to obtain the fixed-vector Hooke law, since that radial measure includes an additional geometric multiplicity. The low-force condition is $fb/(k_BT)\ll1$, equivalently $\langle z\rangle\ll Nb$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
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
