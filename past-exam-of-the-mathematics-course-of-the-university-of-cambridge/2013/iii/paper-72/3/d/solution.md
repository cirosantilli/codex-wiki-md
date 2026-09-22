<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The independent, spatially homogeneous random-placement idealization gives a [Poisson process](../../../../../../poisson-process.md) of intersections along the sampling line. With line intensity $\mu$, an interval of length $s$ contains no ridge with probability $e^{-\mu s}$. The spacing $X$ thus has [exponential distribution](../../../../../../exponential-distribution.md)

$$
\boxed{f_X(s)=\mu e^{-\mu s},\qquad s\ge0,\qquad
\mathbb E[X]=\frac1\mu.}
$$

Random orientation changes the intersection intensity, which has already been represented by the measured $\mu$. Merely saying that positions are random does not prove a [Poisson process](../../../../../../poisson-process.md): independence and homogeneity are additional assumptions. Finite segments, clustering or excluded widths can invalidate them.

For a [shifted lognormal distribution](../../../../../../shifted-lognormal-distribution.md), write $Z=\log(X-\theta)\sim N(m,\sigma^2)$ with $\sigma>0$. Applying the [change of variables](../../../../../../change-of-variables-formula.md) formula, $dZ/dX=1/(X-\theta)$, gives

$$
\boxed{
f_X(x)=
\begin{cases}
\displaystyle\frac{1}{(x-\theta)\sigma\sqrt{2\pi}}
\exp\left[-\frac{(\log(x-\theta)-m)^2}{2\sigma^2}\right],
&x>\theta,\\
0,&x\le\theta .
\end{cases}}
$$

The threshold $\theta$ is a minimum observable separation. Finite keel widths impose geometric exclusion, and the [sonar](../../../../../../sonar.md)'s footprint and ridge-identification criterion can suppress a shallow peak near a deeper peak. This [sonar ridge shadowing](../../../../../../sonar-ridge-shadowing.md) or resolution effect means that $\theta$ need not be a universal physical distance between every pair of ridges; it can partly reflect how the profiles were processed.

A [lognormal distribution](../../../../../../log-normal-distribution.md) is compatible with products of many positive factors: taking logarithms turns multiplicative changes into sums, which can approach a [normal distribution](../../../../../../normal-distribution.md). Repeated deformation, breakup, convergence and merging across scales are plausible contributors. The observed form therefore suggests correlated or multistage ridging rather than the simplest independent-intersection model. **It does not identify a unique ridging mechanism.** For example, directly generating $X=\theta+\exp Z$ with a [normal distribution](../../../../../../normal-distribution.md) for $Z$ produces the same spacing law without specifying any particular mechanics. Distributional agreement must be supplemented by dynamical and spatial evidence.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
