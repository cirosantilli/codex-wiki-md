<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Count oscillator polarizations at fixed center-of-mass [momentum](../../../../../../momentum.md). In a critical [closed bosonic string](../../../../../../closed-string.md), each chiral sector has 24 transverse oscillator species. A species at frequency $m$ can be occupied $0,1,2,\ldots$ times, so its contribution is $(1-q^m)^{-1}$. The full chiral [generating function](../../../../../../generating-function.md) is therefore

$$
F(q)=\sum_{N\ge0}d_Nq^N=\prod_{m\ge1}(1-q^m)^{-24}.
$$

The two sectors are independent, while [closed-string level matching](../../../../../../closed-string-level-matching.md) restricts their oscillator numbers to the same $N$. Thus the number of states at the closed-string mass level is $g_N=d_N^2$, not $d_{2N}$.

Put $q=e^{-\beta}$, with $\beta>0$. The [Dedekind eta function](../../../../../../dedekind-eta-function.md) obeys

$$
\eta\left(\frac{i\beta}{2\pi}\right)=e^{-\beta/24}\prod_{m\ge1}(1-e^{-\beta m}),\qquad \eta(-1/\tau)=\sqrt{-i\tau}\,\eta(\tau).
$$

The transformed argument $2\pi i/\beta$ has large [imaginary part](../../../../../../imaginary-part.md), so its product approaches one and $\eta(2\pi i/\beta)\sim e^{-\pi^2/(6\beta)}$. Hence

$$
F(e^{-\beta})\sim\left(\frac{\beta}{2\pi}\right)^{12}\exp\left(\frac{4\pi^2}{\beta}-\beta\right).
$$

This establishes the singular exponential as well as its power prefactor. The corrections to the transformed eta product are exponentially small in $1/\beta$.

The [Cauchy coefficient formula](../../../../../../cauchy-coefficient-formula.md), followed by $q=e^{-\beta}$, gives a steepest-descent integral with leading form

$$
d_N\sim\frac1{2\pi i}\int d\beta\,\left(\frac\beta{2\pi}\right)^{12}\exp\left((N-1)\beta+\frac{4\pi^2}{\beta}\right).
$$

Let $n=N-1$. The saddle of $S(\beta)=n\beta+4\pi^2/\beta$ is

$$
\beta_* =\frac{2\pi}{\sqrt n},\qquad S(\beta_*)=4\pi\sqrt n,\qquad S''(\beta_*)=\frac{n^{3/2}}\pi.
$$

Along the vertical steepest-descent direction $\beta=\beta_*+it$, the quadratic part is $-S''(\beta_*)t^2/2$. Thus the [saddle-point approximation](../../../../../../saddle-point-approximation.md) gives the Gaussian prefactor

$$
\frac{(\beta_*/2\pi)^{12}}{\sqrt{2\pi S''(\beta_*)}}=\frac1{\sqrt2}n^{-27/4}.
$$

The point $q=1$ supplies the largest exponential contribution. At another fixed [root of unity](../../../../../../root-of-unity.md) of order $k>1$, the corresponding modular singularity gives a smaller exponential $e^{4\pi\sqrt n/k}$, so it does not change this leading asymptotic. Squaring the chiral result gives the [large-level degeneracy of a closed bosonic string](../../../../../../large-level-degeneracy-of-a-closed-bosonic-string.md)

$$
\boxed{d_N\sim\frac1{\sqrt2}(N-1)^{-27/4}e^{4\pi\sqrt{N-1}},\qquad g_N\sim\frac12(N-1)^{-27/2}e^{8\pi\sqrt{N-1}}.}
$$

Replacing $N-1$ by $N$ gives the equivalent usual leading asymptotic. The power $-27/2$ matters: the two-sector degeneracy is not just an unspecified exponential.

Since $M=2\sqrt{(N-1)/\alpha'}$, the exponential is $e^{\beta_H M}$ with

$$
\boxed{\beta_H=4\pi\sqrt{\alpha'},\qquad T_H=\frac1{4\pi\sqrt{\alpha'}}.}
$$

Here Boltzmann's constant is one. Coarse-graining the levels into a density per unit [rest mass](../../../../../../invariant-mass.md) introduces the Jacobian $dN/dM=\alpha'M/2$. Consequently

$$
\rho(M)\sim C M^{-26}e^{\beta_HM},\qquad C=2^{25}\alpha'^{-25/2}.
$$

This is distinct from the degeneracy per level, whose power in $M$ is $-27$. The internal-state contribution to a [canonical partition function](../../../../../../canonical-partition-function.md) behaves at large mass as

$$
Z_{\mathrm{internal}}(\beta)\sim\int^\infty dM\,C M^{-26}e^{-(\beta-\beta_H)M}.
$$

It converges for $\beta>\beta_H$ and diverges for $\beta<\beta_H$. At $\beta=\beta_H$, this particular internal rest-mass integral converges because of the power $M^{-26}$; one should not discard the prefactor and claim divergence there without specifying the full thermodynamic ensemble. For example, including continuous [momenta](../../../../../../momentum.md) in 25 spatial dimensions multiplies the high-mass integrand by a factor proportional to $M^{25/2}$, still leaving convergence of this ideal one-string integral at the endpoint, although sufficiently high [derivatives](../../../../../../derivative.md) are singular. Multi-string effects, volume and interactions affect the detailed limiting thermodynamics.

The leading microcanonical entropy grows as $S(E)\sim\beta_HE$, with logarithmic corrections, so increasingly large energies are stored in increasingly excited, long strings rather than in an arbitrarily hot ordinary gas. The [Hagedorn temperature](../../../../../../hagedorn-temperature.md) is the boundary of canonical convergence from above in [inverse temperature](../../../../../../inverse-temperature.md); extrapolating the free-string canonical description to $T>T_H$ fails. This counting does not settle the interacting phase above that scale. Also, the bosonic ground-state [tachyon](../../../../../../tachyon.md) is a separate vacuum instability; the high-level asymptotic is meaningful as a formal spectrum calculation without asserting a stable bosonic thermal vacuum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
