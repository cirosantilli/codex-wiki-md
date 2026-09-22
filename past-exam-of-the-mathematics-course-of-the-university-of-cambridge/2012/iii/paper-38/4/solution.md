<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [Gibbs sampler](../../../../../gibbs-sampler.md) updates one coordinate by drawing from its [full conditional distribution](../../../../../full-conditional-distribution.md), leaving the others unchanged and using their current values. Each coordinate kernel $K_i$ preserves the target joint law $P$: integrate first over the unchanged coordinates, then over the old coordinate, and finally draw the new coordinate from the same [conditional distribution](../../../../../conditional-distribution.md). The resulting joint law is again $P$. In the discrete notation, if two states share the remaining coordinates,

$$
P(x)K_i(x,x')
=P_{-i}(x_{-i})P(x_i\mid x_{-i})P(x_i'\mid x_{-i}),
$$

which is symmetric in $x_i,x_i'$. Thus a coordinate update satisfies [detailed balance](../../../../../detailed-balance.md). A systematic full sweep has kernel $K_1\cdots K_k$ and remains invariant because each factor preserves $P$. A fixed-probability random-scan mixture also preserves $P$; the mixture is reversible, whereas a systematic composition need not be.

In the [autologistic binary-image model](../../../../../autologistic-binary-image-model.md), count each neighboring pair once. Changing one pixel from zero to one raises $n_1$ by one and $n_2$ by the number $z_{ij}$ of neighboring ones. The ratio of its two conditional weights is $\exp(\alpha+\beta z_{ij})$. Therefore

$$
\boxed{p_{ij}=\frac{e^{\alpha+\beta z_{ij}}}{1+e^{\alpha+\beta z_{ij}}}
=\operatorname{logistic}(\alpha+\beta z_{ij}).}
$$

For single-site [Gibbs sampling](../../../../../gibbs-sampler.md), select a pixel, compute its current neighbor sum and replace it by a draw from a [Bernoulli distribution](../../../../../bernoulli-distribution.md) with this probability. One may use random scans or complete ordered sweeps. The [normalizing constant](../../../../../normalizing-constant.md) is not needed. For finite $\alpha,\beta$, every [conditional probability](../../../../../conditional-probability.md) lies strictly between zero and one; the finite chain is irreducible and has self-transitions, so its stationary law is unique and iterating converges to it.

For [checkerboard Gibbs sampling](../../../../../checkerboard-gibbs-sampling.md), no edge joins two black pixels or two white pixels. Conditional on the whites, the black-pixel law factorizes:

$$
P(B=b\mid W=w)=
\prod_{v\in B}p_v(w)^{b_v}(1-p_v(w))^{1-b_v}.
$$

Draw all black pixels independently with these probabilities, then draw all white pixels independently conditional on the newly drawn blacks. Each color block is a full conditional update, so the two-block sweep preserves the joint target. Pixels of the same color can be updated together because their [conditional distribution](../../../../../conditional-distribution.md) factorizes.

For the noisy image, the log likelihood contributes $-\tfrac12\sum_v(y_v-x_v)^2$. Since $x_v^2=x_v$, dropping terms independent of $x$ gives

$$
P(x\mid y)\ \propto\
\exp\!\left\{\sum_v(\alpha+y_v-\tfrac12)x_v
+\beta\sum_{\{v,w\}\text{ edge}}x_vx_w\right\}.
$$

The [Gaussian-noise posterior for an autologistic image](../../../../../gaussian-noise-posterior-for-an-autologistic-image.md) therefore has [conditional probabilities](../../../../../conditional-probability.md)

$$
\boxed{P(X_{ij}=1\mid X_{-(ij)},Y=y)
=\operatorname{logistic}\!\left(\alpha+\beta z_{ij}+y_{ij}-\tfrac12\right).}
$$

Use this probability in both single-pixel and sequential color-block schemes. The independent observation factors change only the local field, so conditional independence within each color is retained. The same invariance proof then targets the [posterior distribution](../../../../../bayesian-posterior.md) rather than the prior.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
