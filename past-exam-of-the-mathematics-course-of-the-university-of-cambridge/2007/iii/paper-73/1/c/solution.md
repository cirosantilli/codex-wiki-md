<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

One useful starting point is reverse correlation, implemented as a [spike-triggered average](../../../../../../spike-triggered-average.md). Present a long stimulus record and retain the stimulus history before each observed spike. After subtracting the stimulus mean, estimate

$$
\widehat k(u)=\frac1K\sum_{i=1}^K s(t_i-u),\qquad 0\leq u\leq T_k,
$$

where $K$ is the number of spikes and $T_k$ is the history window. This identifies a candidate temporal [receptive field](../../../../../../receptive-field.md). For white Gaussian stimulation and a one-filter encoding model, the average is proportional to the relevant filter, provided the response nonlinearity does not make that average vanish. For example an even response to the projection can have zero average despite strong stimulus dependence. Colored inputs require accounting for stimulus covariance, and more than one relevant stimulus direction may require a richer fitted model.

Use the candidate filter in an [LNP model](../../../../../../linear-nonlinear-poisson-cascade-model.md):

$$
z(t)=b+\int_0^{T_k} k(u)s(t-u)\,du,\qquad r(t)=g(z(t))\geq0.
$$

Estimate the static nonlinearity $g$ by binning filter projections and dividing spike counts by exposure time in each bin. Equivalently, Bayes' rule gives $g(z)=\overline r\,p(z\mid\text{spike})/p(z)$ under this model. Refine the filter and nonlinearity by maximizing the conditional Poisson [log-likelihood](../../../../../../log-likelihood.md)

$$
\ell=\sum_i\log r(t_i)-\int r(t)\,dt,
$$

with suitable regularization. Simulate an [Inhomogeneous Poisson process](../../../../../../inhomogeneous-poisson-process.md) at the fitted rate using integrated-intensity inversion from the previous solution. This gives a statistical encoding model, not a claim to reconstruct the neuron's ion channels.

Use [cross-validation](../../../../../../cross-validation.md): estimate parameters on one set of trials and test them on independent held-out trials. Under repeated identical stimuli, compare the observed and simulated trial-averaged firing rates, spike-count distributions, interspike-interval distributions and [autocorrelations](../../../../../../autocorrelation.md). Compare held-out likelihoods and predictive errors with simpler baseline models and with the variability between real repeats. Exact spike-by-spike agreement is not expected from two independent realizations of a stochastic model. Large rate agreement accompanied by incorrect short-interval or correlation statistics reveals missing dynamics. Adding a spike-history term, for example in a point-process [generalized linear model](../../../../../../generalized-linear-model.md), can account for refractoriness or bursting when the basic Poisson cascade fails.

**A good model predicts held-out response distributions, not just its training spike train.** Such a model summarizes what stimulus features affect the neuron, permits controlled simulated changes of those features, and tests whether the proposed computation is sufficient. Its failures can suggest further experiments or additional stimulus and history variables.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
