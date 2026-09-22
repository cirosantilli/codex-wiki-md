# Regular conditional distribution

↑ **Parent:** [Conditional distribution](conditional-distribution.md)

A regular conditional distribution of a [random variable](random-variable-split.md) $X$ given $Y$ is a [Markov kernel](markov-kernel.md) $K$ such that, for all measurable sets $A,B$,

$$
P(X\in B,Y\in A)=\int_A K(y,B)\,P_Y(dy).
$$

For each $y$, $K(y,\cdot)$ is a [probability measure](probability-measure.md); for each $B$, $K(\cdot,B)$ is measurable. Thus it assigns an actual probability distribution to a specified observation even when $P(Y=y)=0$. Such kernels exist for standard Borel state spaces, including real-valued variables, and their uniqueness is only up to $P_Y$-null sets. With a joint density and positive marginal density, the ratio of the two densities defines the usual conditional density kernel. Values outside the marginal support or on a null set are not uniquely determined by the joint law.

## ↑ Ancestors (7)

1. [Conditional distribution](conditional-distribution.md)
2. [Conditional probability](conditional-probability.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Conditional inference in a location-scale family](conditional-inference-in-a-location-scale-family.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38/6/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2/10f/b/solution.md)
