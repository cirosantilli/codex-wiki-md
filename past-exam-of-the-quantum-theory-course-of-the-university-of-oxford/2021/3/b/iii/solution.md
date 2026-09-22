<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Continue with the initial [quantum state](../../../../../quantum-state.md) $\psi_1$ from part (ii), and let $\Delta t=T/N$. Conditional on every preceding outcome being $+\hbar/2$, the [post-measurement state](../../../../../post-measurement-state.md) after each ideal [projective measurement](../../../../../projective-measurement.md) is again $\psi_1$, up to [global phase](../../../../../global-phase.md). Part (ii) therefore gives the same [conditional probability](../../../../../conditional-probability.md) $\cos^2(\omega\Delta t)$ for each successive outcome. Multiplying these [conditional probabilities](../../../../../conditional-probability.md) yields the [repeated projective-measurement survival probability](../../../../../repeated-projective-measurement-survival-probability.md)

$$
\boxed{\mathbb P_N(T)=\left[\cos^2\left(\frac{\omega T}{N}\right)\right]^N.}
$$

This multiplication uses the [quantum state](../../../../../quantum-state.md) reset at each successful [projective measurement](../../../../../projective-measurement.md); the outcomes need not be assumed statistically independent.

For fixed $T$, put $z=\omega T$. The [Taylor expansion](../../../../../taylor-expansion.md) $\cos^2u=1-u^2+O(u^4)$ gives the [quadratic short-time quantum survival probability](../../../../../quadratic-short-time-quantum-survival-probability.md). For sufficiently large $N$, taking logarithms gives

$$
\log\mathbb P_N(T)=N\log\left(1-\frac{z^2}{N^2}+O(N^{-4})\right)
=-\frac{z^2}{N}+O(N^{-3})\longrightarrow0.
$$

Here the remainder uses [Big O notation](../../../../../big-o-notation.md). Exponentiating proves

$$
\boxed{\lim_{N\to\infty}\mathbb P_N(T)=1,\qquad
\mathbb P_N(T)=1-\frac{(\omega T)^2}{N}+O(N^{-2}).}
$$

This is the [quantum Zeno effect](../../../../../quantum-zeno-effect.md): increasingly frequent ideal [projective measurements](../../../../../projective-measurement.md) inhibit the transition away from the initial [quantum state](../../../../../quantum-state.md). The departure [probability](../../../../../probability.md) in a short interval is quadratic in its duration, so $N$ intervals of duration $T/N$ produce a total leading departure [probability](../../../../../probability.md) proportional to $T^2/N$. Without intervening measurements, the return [probability](../../../../../probability.md) at time $T$ would be $\cos^2(\omega T)$. The result concerns obtaining $+\hbar/2$ at every measurement in the ideal limit of instantaneous measurements with [unitary time evolution](../../../../../unitary-time-evolution.md) between them.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
