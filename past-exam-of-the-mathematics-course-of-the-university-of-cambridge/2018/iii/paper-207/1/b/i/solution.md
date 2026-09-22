<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use an irreversible [continuous-time multi-state model](../../../../../../../continuous-time-multi-state-model.md) $1\to2\to3$, with state 3 absorbing. Let $a=q_{12}(50)$ and $b=q_{23}(50)$, and define log-linear age effects by

$$
q_{12}(A)=a e^{\beta_{12}(A-50)},\qquad
q_{23}(A)=b e^{\beta_{23}(A-50)}.
$$

For a closed-form [panel-observed multi-state likelihood](../../../../../../../panel-observed-multi-state-likelihood.md), freeze the age covariate at the start of each observation interval. The [transition intensities](../../../../../../../transition-intensity.md) are then $(a,b)$ over the first interval and $(\lambda,\mu)=(ae^{5\beta_{12}},be^{5\beta_{23}})$ over the second. Conditional on the initial state, the [likelihood contribution](../../../../../../../likelihood-contribution.md) is

$$
\boxed{L(a,b,\beta_{12},\beta_{23})
=e^{-5a}\left[1-e^{-ae^{5\beta_{12}}}
-p_{12}\!\left(1\mid ae^{5\beta_{12}},be^{5\beta_{23}}\right)\right].}
$$

Indeed, $p_{11}(5)=e^{-5a}$ and $p_{13}(1)=1-p_{11}(1)-p_{12}(1)$. In this irreversible [continuous-time Markov chain](../../../../../../../continuous-time-markov-chain.md), the intermediate state has probability

$$
p_{12}(u\mid\lambda,\mu)=
\begin{cases}
\displaystyle\frac{\lambda(e^{-\lambda u}-e^{-\mu u})}{\mu-\lambda},&\lambda\ne\mu,\\
\lambda u e^{-\lambda u},&\lambda=\mu.
\end{cases}
$$

The second expression is the continuous limit of the first and handles equal rates. The observed two-state jump across an interval is compatible with adjacent instantaneous transitions: an unobserved visit to state 2 occurs between the examinations.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
