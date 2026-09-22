<h1 id="b4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a binary state, its [expected value](../../../../../expected-value-split.md) is its probability of being one. Hence the [Monte Carlo method](../../../../../monte-carlo-method-split.md) estimate of the [posterior methylation profile](../../../../../posterior-methylation-profile.md) under the chosen target is

$$
\widehat p_i=\frac{1}{N-B}\sum_{t=B}^{N-1}m_i^{(t)}.
$$

The averaging axis must be zero: average over sampled patterns while keeping the site index. A provisional choice for this particular trace is **$B=3000$**, retaining 2000 states:

```
def mean_methylation(meths, burnin):
    if not 0 <= burnin < len(meths):
        raise ValueError("burn-in must leave at least one state")
    return np.asarray(meths)[burnin:].mean(axis=0)

burnin = 3000
profile_estimate = mean_methylation(meths, burnin)
print(lls[burnin:].mean())
plt.plot(profile_estimate, label="retained-sample mean")
plt.scatter(np.arange(len(obs)), .2*obs, s=10, label="0.2 × observation")
plt.xlabel("Site index")
plt.ylabel("Methylation probability")
plt.legend()
plt.show()
```

**The retained mean log score is $-74.8895$**, and the profile is shown below the trace in part (b). The fixed endpoints have estimate exactly one; adjacent sites are often smoothed into methylated or unmethylated stretches despite individual conflicting observations. The rescaled observations are only a visual comparison and are not another estimate of the [posterior probability](../../../../../posterior-probability.md).

This is a finite-chain estimate for the conditional-product target defined in part (a). A [burn-in](../../../../../burn-in.md) chosen by inspection does not establish convergence, and the long excursions in this short [Markov chain](../../../../../markov-chain-split.md) leave substantial uncertainty in individual-site estimates; several longer runs would be needed for precise inference. To sample the coherent joint alternative instead, pass `score=joint_methylation_score` and inspect that new trace before choosing its own [burn-in](../../../../../burn-in.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [B4](../../b4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
