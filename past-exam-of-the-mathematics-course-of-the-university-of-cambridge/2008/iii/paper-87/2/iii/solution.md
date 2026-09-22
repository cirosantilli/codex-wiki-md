<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Measure the cloud radius about its moving centre, so uniform sweeping does not count as spreading. In the [inertial range](../../../../../../inertial-range.md), an eddy of size $R$ has [velocity](../../../../../../velocity.md) difference $u_R\sim(\epsilon R)^{1/3}$ and turnover time $t_R\sim R/u_R$. A scale-local relative diffusivity is therefore

$$
D_R\sim u_R^2t_R\sim u_RR\sim\epsilon^{1/3}R^{4/3},
$$

giving the estimate

$$
\boxed{\frac{dR^2}{dt}\sim\epsilon^{1/3}R^{4/3}.}
$$

It requires separation from the molecular and viscous cutoffs and from the [integral scale of turbulence](../../../../../../integral-scale-of-turbulence.md), high [Reynolds number](../../../../../../reynolds-number.md), approximately steady energy supply, and scale-local relative motion. Mean shear, walls, particle inertia or coherent large-scale strain can invalidate this simple diffusivity model. At very short times a pair retains its initial relative [velocity](../../../../../../velocity.md), so a [diffusion](../../../../../../diffusion.md) closure is not yet appropriate.

Let $s(t)=\langle|\delta\boldsymbol x(t)|^2\rangle$. A self-similar pair-separation distribution, together with the relative-diffusivity estimate, gives

$$
\frac{ds}{dt}=A\epsilon^{1/3}s^{2/3}.
$$

Self-similarity is needed to replace a separation-dependent moment such as $\langle r^{4/3}\rangle$ by a fixed multiple of $s^{2/3}$; stationarity alone does not do that. Integrating this model gives

$$
s^{1/3}(t)=s^{1/3}(0)+\frac A3\epsilon^{1/3}t.
$$

After loss of initial-separation memory, it reduces to the [Richardson pair dispersion](../../../../../../richardson-pair-dispersion.md) law

$$
\boxed{\langle|\delta\boldsymbol x(t)|^2\rangle\sim g\epsilon t^3,
\qquad g=(A/3)^3.}
$$

The required time window is $t\gg t_0\sim(r_0^2/\epsilon)^{1/3}$ while the separation remains far below the integral scale. The stated stationarity and inertial-range separation conditions alone cannot imply the displayed $t^3$ law at every time: a nonzero release separation already gives $s(0)=r_0^2$, whereas $g\epsilon t^3$ vanishes at zero. At sufficiently short times, $\delta\boldsymbol x(t)-\delta\boldsymbol x_0\simeq\delta\boldsymbol u_0t$, so its mean-square change is ballistic and remembers $r_0$.

The [Richardson constant](../../../../../../richardson-constant.md) might be universal if the inertial-range relative dynamics, including the normalized separation distribution, become independent of release details and forcing at sufficiently high Reynolds number. This is an additional universality hypothesis. As evidence available before 2008, [Boffetta and Sokolov's numerical study](https://arxiv.org/abs/nlin/0107061) estimated a coefficient near $0.55$ and reported agreement with experimental estimates, alongside small deviations from ideal Richardson scaling. [Bourgoin and collaborators' 2006 experiment](https://pubmed.ncbi.nlm.nih.gov/16469922) showed substantial dependence on initial separation in the accessible laboratory regime. **Values of order $0.5$ are supported in suitable regimes, but finite-time fits do not establish one universally observed $t^3$ coefficient for all releases.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 87](../../../paper-87-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
