<h1 id="8a/solution">Solution</h1>

↑ **Parent:** [8A](../8a.md)

Let $\Delta=\theta_1-\theta_0>0$, with $\alpha,\beta_{\max}>0$. [Newton law of cooling](../../../../../newton-s-law-of-cooling.md) gives the warming and cooling profiles

$$
\theta(t)-\theta_0=\begin{cases}
\Delta(1-e^{-\alpha t}),&0\leq t\leq T,\\
\Delta(1-e^{-\alpha T})e^{-\alpha(t-T)},&T\leq t\leq2T.
\end{cases}
$$

In the stipulated linear model, $\beta(t)=\beta_{\max}(\theta(t)-\theta_0)/\Delta$. The bacterial count obeys $\dot N=-\beta(t)N$, so its logarithmic reduction is the [cumulative thermal destruction under exponential warming and cooling](../../../../../cumulative-thermal-destruction-under-exponential-warming-and-cooling.md):

$$
\log\frac{N(0)}{N(2T)}=\int_0^{2T}\beta(t)\,dt.
$$

Writing $q=e^{-\alpha T}$, the warming integral divided by $\beta_{\max}$ is $T-(1-q)/\alpha$ and the cooling contribution is $(1-q)^2/\alpha$. Hence the required implicit equation is

$$
\boxed{\beta_{\max}\left[T-\frac{e^{-\alpha T}(1-e^{-\alpha T})}{\alpha}\right]=20\log10}.
$$

The bracket is zero at zero and has [derivative](../../../../../derivative.md) $(1-q)(1+2q)>0$ for $T>0$, tending to infinity with $T$. There is therefore one positive solution.

**For the hardier species, $T$ is unchanged in this model if $\alpha$ and the achieved $\beta_{\max}$ remain the same.** Raising the oven temperature changes $\Delta$, but its factor cancels against the changed slope of the linear destruction law. The entire normalized temperature history and hence the destruction integral remain the same; the comparison uses both the warming and equal-duration cooling stages.

## ↑ Ancestors (10)

1. [8A](../8a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
