<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For coordinate $i$, keep the other coordinates fixed and propose $y_i$ from the full conditional $\pi(\cdot\mid x_{-i})$. This is a [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) proposal on that coordinate fibre, with deterministic equality $y_{-i}=x_{-i}$. Its acceptance ratio is

$$
\frac{\pi(y_i,x_{-i})\pi(x_i\mid x_{-i})}{\pi(x_i,x_{-i})\pi(y_i\mid x_{-i})}=1.
$$

Thus the coordinate update has **acceptance probability one** and is exactly a single-coordinate [Gibbs sampler](../../../../../../gibbs-sampler.md) update.

A systematic sweep through coordinates $1,\ldots,p$ is the composition of these kernels. Its joint transition density is

$$
\boxed{K(x,y)=\prod_{i=1}^p\pi(y_i\mid y_1,\ldots,y_{i-1},x_{i+1},\ldots,x_p).}
$$

The already updated coordinates are new values, and the not-yet-updated coordinates are old values. Each coordinate kernel preserves $\pi$, so their composition also preserves it. [Systematic Gibbs sampling need not be reversible](../../../../../../systematic-gibbs-sampling-need-not-be-reversible.md): each individual coordinate kernel is reversible, but their ordered composition need not be reversible; invariance is the property needed here. A random-scan mixture of the coordinate kernels is reversible.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
