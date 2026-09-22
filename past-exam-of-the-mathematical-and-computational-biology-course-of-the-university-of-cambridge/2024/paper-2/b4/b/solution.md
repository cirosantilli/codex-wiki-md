<h1 id="b4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A single randomly chosen internal-site flip is a symmetric proposal: the reverse flip has the same probability $1/98$. Therefore the [Metropolis–Hastings algorithm](../../../../../metropolis-hastings-algorithm.md) accepts with

$$
\boxed{\alpha=\min\{1,\exp(s(m';o)-s(m;o))\}}.
$$

Comparing logarithms avoids overflow. On rejection the old state must be retained, including a repeated copy in the stored [Markov chain](../../../../../markov-chain-split.md); retaining only accepted states would sample a different distribution. This implementation also stores the actual initial state at row zero:

```
def sample_methylation(observed, nsteps=5000, seed=2024, score=methylation_score):
    rng=np.random.default_rng(seed)
    state=rng.integers(0,2,size=len(observed));state[[0,-1]]=1
    states=np.empty((nsteps,len(state)),dtype=int);values=np.empty(nsteps)
    states[0]=state;values[0]=score(state,observed)
    accepted=0
    for t in range(1,nsteps):
        candidate=state.copy();site=rng.integers(1,len(state)-1)
        candidate[site]=1-candidate[site]
        trial=score(candidate,observed)
        if np.log(rng.random())<min(0.,trial-values[t-1]):
            state=candidate;values[t]=trial;accepted+=1
        else:values[t]=values[t-1]
        states[t]=state
    return values,states,accepted/(nsteps-1)

lls, meths, acceptance = sample_methylation(obs, nsteps=5000, seed=2024)
import matplotlib.pyplot as plt
plt.plot(lls)
plt.xlabel("Stored state index")
plt.ylabel("Conditional-product log score")
plt.show()
```

For this random-number convention, **the acceptance fraction is approximately $0.157$**. The trace climbs substantially during its first several thousand updates, so a small fixed [burn-in](../../../../../burn-in.md) such as 100 iterations would discard too little of the initial transient. Five thousand single-site proposals are only about fifty updates per site on average.

<a id="b4/b/image-conditional-product-sampling-trace-and-retained-sample-methylation-profile-with-a-provisional-burn-in-of-3000-stored-states"></a>
![](../../../../../past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2024/paper-2-methylation.png)

**[Figure 3](#b4/b/image-conditional-product-sampling-trace-and-retained-sample-methylation-profile-with-a-provisional-burn-in-of-3000-stored-states). Conditional-product sampling trace and retained-sample methylation profile, with a provisional burn-in of 3000 stored states**.

## ↑ Ancestors (13)

1. [B](../b.md)
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
