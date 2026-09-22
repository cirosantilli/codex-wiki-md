<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The consistent missing-data interpretation is that each never-recaptured individual either dies in an interval $j<J$ or survives unobserved through the final occasion. Define the known never-recaptured total and its allocation by

$$
N_i=R_i-\sum_{s=i+1}^Jm_{is},\qquad
\sum_{j=i}^{J-1}n_{ij}+n_{iJ}=N_i.
$$

The terminal cell $n_{iJ}$ is the source's separately named $n_i$. The printed identity equating that cell to the total observed recaptures is inconsistent with the supplied multinomial law. In particular, with no observed recaptures its printed value would be zero even though the terminal-cell probability is positive at interior parameters. The displayed accounting identity repairs that notation and makes all sums through $J$ well-defined.

For an individual released at $i$, define the unnormalized probabilities

$$
w_{ij}=(1-\phi_j)\prod_{\ell=i}^{j-1}\phi_\ell(1-P_{\ell+1})\quad(i\le j<J),\qquad
w_{iJ}=\prod_{\ell=i}^{J-1}\phi_\ell(1-P_{\ell+1}).
$$

The empty product is one. Each intermediate factor means surviving an interval and avoiding its subsequent detection; the death weight additionally includes failure to survive interval $j$. Let $K_i=\sum_{j=i}^Jw_{ij}$. This is the probability of never being recaptured. It is the source's normalizing constant $C_i$, renamed to avoid confusion with the detection-success counts above. Conditional on no recapture, division by $K_i$ gives precisely the supplied [multinomial distribution](../../../../../../multinomial-distribution.md) cell probabilities.

Initialize an interior parameter vector $(\phi^{(0)},P^{(0)})$. At iteration $r$, the E step of [missing-count EM for capture-recapture](../../../../../../missing-count-em-for-capture-recapture.md) computes, for every cohort and missing cell,

$$
\boxed{\overline n_{ij}^{(r)}
=\mathbb E[n_{ij}\mid m,\phi^{(r)},P^{(r)}]
=N_i\frac{w_{ij}(\phi^{(r)},P^{(r)})}{K_i(\phi^{(r)},P^{(r)})},\quad i\le j\le J.}
$$

If $N_i=0$, set every missing count to zero without dividing, even if $K_i=0$. If $N_i>0$ and $K_i=0$, that parameter vector gives zero probability to the observations and cannot be used in the E step. These expected counts sum to $N_i$, preserving each cohort's observed accounting. The E step is [conditional expectation](../../../../../../conditional-expectation.md), not replacement by the modal missing counts or a single random imputation.

The expected complete-data log likelihood is linear in the missing counts, apart from count-only terms irrelevant to the new parameter values. In the M step substitute these expectations into the success/failure ratios from part (a):

$$
\boxed{\phi_j^{(r+1)}=
\frac{\sum_{i=1}^j\sum_{s=j+1}^J(m_{is}+\overline n_{is}^{(r)})}
{\sum_{i=1}^j(\sum_{s=j+1}^Jm_{is}+\sum_{s=j}^J\overline n_{is}^{(r)})},}
$$

and

$$
\boxed{P_j^{(r+1)}=
\frac{\sum_{i=1}^{j-1}m_{ij}}
{\sum_{i=1}^{j-1}\sum_{s=j}^J(m_{is}+\overline n_{is}^{(r)})}.}
$$

If an exposure denominator vanishes, retain any admissible value of the unidentifiable parameter. Repeat until the observed likelihood and parameter updates stabilize. The conditional normalizers in the E step are evaluated at the old parameters; maximizing a newly normalized conditional missing-data distribution instead of the expected complete-data log likelihood would be the wrong M step.

One can monitor the observed likelihood directly. The probability of a first recapture at $s>i$ is

$$
p_{is}=\left[\prod_{\ell=i}^{s-2}\phi_\ell(1-P_{\ell+1})\right]\phi_{s-1}P_s,
$$

and successive death, detection and continuation alternatives partition the possibilities, giving $K_i+\sum_{s=i+1}^Jp_{is}=1$. Thus, up to count-only factors,

$$
L_{\mathrm{obs}}\propto\prod_i K_i^{N_i}\prod_{s=i+1}^Jp_{is}^{m_{is}}.
$$

The usual conditional Jensen argument for the [EM algorithm](../../../../../../expectation-maximization-algorithm.md) makes this likelihood nondecreasing at each exact M step. It does not guarantee a unique global maximum. In this observation scheme the final survival and detection probabilities enter through the product $\phi_{J-1}P_J$ only, so these two probabilities cannot generally be estimated separately without a further constraint. The algorithm remains valid, but may converge to different points on the same likelihood ridge.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
