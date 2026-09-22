# Negative entropy production over finite durations

↑ **Parent:** [Biased-step entropy production model](biased-step-entropy-production-model.md)

A single step has negative [entropy production](entropy-production.md) with [probability](probability.md) $q$, independent of how long an observation lasts. A whole window is negative only if negative steps outnumber positive ones:

$$
\Pr(S_n<0)=\sum_{k=0}^{\lfloor(n-1)/2\rfloor}\binom nkp^kq^{n-k}.
$$

For even $n$, the tie $K=n/2$ has zero [entropy production](entropy-production.md) and is excluded. At $p=3/4$, the negative-window [probabilities](probability.md) for $n=1,9,21$ are approximately $0.25$, $0.04893$, and $0.00642$. Longer windows still contain negative increments: their expected number is $nq$. Their total is usually positive because the expected number of positive increments is $np$.

<a id="image-exact-biased-step-model-negative-totals-become-rare-with-duration-while-negative-increments-remain-frequent"></a>
![](negative-entropy-window-duration.png)

**[Figure 18](#image-exact-biased-step-model-negative-totals-become-rare-with-duration-while-negative-increments-remain-frequent). Exact biased-step model: negative totals become rare with duration while negative increments remain frequent**.

Only odd window lengths are plotted to avoid alternating tie effects. The left panel gives the exact negative-window [probability](probability.md) and the upper bound $(2\sqrt{pq})^n$; the right gives expected counts $np$ and $nq$. For steps of fixed duration $\delta t$, physical duration is $n\delta t$. These are counts and [probabilities](probability.md) predicted by the model, not bead traces. The bound follows from $\Pr(S_n<0)\le\langle e^{-S_n/2}\rangle=(2\sqrt{pq})^n$. Since $2\sqrt{pq}<1$ for $p\ne q$, negative totals are exponentially suppressed even though the negative-step fraction stays $q$.

## ↑ Ancestors (9)

1. [Biased-step entropy production model](biased-step-entropy-production-model.md)
2. [Fluctuation theorem](fluctuation-theorem.md)
3. [Entropy production](entropy-production.md)
4. [Stochastic thermodynamics](stochastic-thermodynamics.md)
5. [Thermodynamics](thermodynamics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)
