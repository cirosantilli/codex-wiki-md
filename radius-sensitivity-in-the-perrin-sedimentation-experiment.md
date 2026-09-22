# Radius sensitivity in the Perrin sedimentation experiment

↑ **Parent:** [Perrin sedimentation experiment](perrin-sedimentation-experiment.md)

At fixed measured count [slope](slope.md), $N_A^{\rm sed}\propto a^{-3}$, whereas at fixed measured [diffusion coefficient](diffusion-coefficient.md), $N_A^{\rm diff}\propto a^{-1}$. First-order [propagation of uncertainty](propagation-of-uncertainty.md) follows by taking [logarithmic derivatives](logarithmic-derivative.md):

$$
\frac{dN_A^{\rm sed}}{N_A^{\rm sed}}=\frac{dT}{T}+\frac{db}{b}-\frac{d\Delta\rho}{\Delta\rho}-3\frac{da}{a}-\frac{dg}{g},\qquad
\frac{dN_A^{\rm diff}}{N_A^{\rm diff}}=\frac{dT}{T}-\frac{d\eta}{\eta}-\frac{da}{a}-\frac{dD}{D}.
$$

For [independent](independent-random-variables.md) small errors, the radius contributes $9(\sigma_a/a)^2$ to the relative [variance](variance-split.md) of $N_A^{\rm sed}$, compared with $(\sigma_a/a)^2$ for $N_A^{\rm diff}$. Shared radius and [temperature](temperature-split.md) calibrations make the two estimates correlated; their agreement is therefore not two wholly independent determinations. As a finite-error example, overestimating $a$ by $5\%$ multiplies the respective answers by $1.05^{-3}\simeq0.8638$ and $1.05^{-1}\simeq0.9524$.

This explains the importance of the radius cross-checks in the 1909 memoir: testing the [Stokes drag law](stokes-s-law.md) through an independent radius estimate helps prevent circular inference.[1909 memoir, §§20–21, scan pp. 41–46](mouvement-brownien-et-realite-moleculaire-by-jean-baptiste-perrin.md) [Convection](convection-split.md) must also be excluded: a residual horizontal speed $u$ adds $u^2\tau^2$ to an uncentred [mean squared displacement](mean-squared-displacement.md), making a linear fit misleading.

## ↑ Ancestors (8)

1. [Perrin sedimentation experiment](perrin-sedimentation-experiment.md)
2. [Brownian motion](brownian-motion-split.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
